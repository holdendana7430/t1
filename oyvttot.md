代发 wailian999

cmd > out.log 2>&1
来源：http://yp.gzmigu.cn

[R40] 追加写日志
来源：http://gw.wgjwhj.cn

echo "log" >> out.log
来源：http://rv.bjjhwx.cn

[R41] 丢弃输出
来源：http://sk.521024.cn

cmd >/dev/null 2>&1
来源：http://au.szsharing.cn

[R42] 输入重定向
来源：http://cs.colortex.cn

wc -l < a.txt
来源：http://th.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://bt.jctech888.com.cn

find . -name "*.log" -type f
来源：http://jb.newstarts.cn

[R44] 按修改时间查找
来源：http://fq.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://ey.huanxung.cn

[R45] 批量删除
来源：http://oa.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://jz.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://me.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hj.panjiajie.cn

[R47] sed 单行替换
来源：http://zg.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sn.nicolike.cn

[R48] awk 取指定列
来源：http://fk.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://so.nszjky.cn

[R49] awk 带条件
来源：http://gx.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mu.yuexingan06.cn

[R50] awk 求和
来源：http://yl.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wm.szsharing.cn

[R51] 排序去重取前几
来源：http://zw.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sy.bjjhwx.cn

[R52] 统计行数
来源：http://bm.szsharing.cn

wc -l a.txt
来源：http://zl.521024.cn

[R53] 查看文件头与实时尾
来源：http://uw.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ii.asd995.cn

[R54] 比较两个文件
来源：http://jp.bjjhwx.cn

diff a.txt b.txt
来源：http://rp.shxzukj.cn

[R55] 压缩与解压
来源：http://wt.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tt.hahajie.cn

[R56] 远程拷贝
来源：http://an.shxzskj.cn

scp file user@host:/path/
来源：http://gt.hahajie.cn

[R57] 远程执行命令
来源：http://dy.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://fi.bjjhwx.cn

[R58] 下载文件
来源：http://bn.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bq.chemitech.net.cn

[R59] 发 POST JSON
来源：http://uk.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ji.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://yw.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bl.colortex.cn

[R61] 磁盘占用
来源：http://mv.szsharing.cn

df -h;  du -sh *
来源：http://fe.lnxyls.cn

[R62] 找最占空间的文件
来源：http://fu.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://te.huixinmuqiang.cn

[R63] 内存与进程
来源：http://od.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://tj.szxytkj.cn

[R64] 结束进程
来源：http://vj.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://oj.lnxyls.cn

[R65] 查看端口占用
来源：http://ur.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bc.panjiajie.cn

[R66] 定时任务
来源：http://as.gzmigu.cn

crontab -e;  crontab -l
来源：http://ck.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://jg.521024.cn

openssl rand -hex 16
来源：http://ty.asd995.cn

[R68] 计算文件校验值
来源：http://bv.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jw.521024.cn

[R69] 生成随机密码
来源：http://qb.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://xj.lnxyls.cn

[R70] 时间戳与互转
来源：http://et.szsharing.cn

date +%s;  date -d @1700000000
来源：http://qj.muxihuayi.cn

[R71] 日期格式化
来源：http://be.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zs.colortex.cn

[R72] 等待端口就绪
来源：http://zy.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zp.nicolike.cn

[R73] 分割大日志
来源：http://yi.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://od.huixiangedu.cn

[R74] 批量重命名
来源：http://ti.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://td.asd995.cn

[R75] 导出环境变量
来源：http://yl.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://fw.lnxyls.cn

[R76] 使用临时文件
来源：http://if.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yb.szsharing.cn

[R77] 读取用户输入
来源：http://go.szxytkj.cn

read -rp "请输入: " ans
来源：http://bk.wgjwhj.cn

[R78] 交互式菜单
来源：http://uo.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mq.bjjhwx.cn

[R79] 解析命令行选项
来源：http://xa.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oh.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://ml.lnxyls.cn

time ./run.sh
来源：http://bi.huanxung.cn

================================================================================
来源：http://sd.gzmigu.cn

S. C / C++ 专题
来源：http://ga.bjjhwx.cn

================================================================================
来源：http://iz.huanxung.cn

[S01] C：Hello World
来源：http://bw.lnxyls.cn

#include <stdio.h>
来源：http://hd.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://no.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://jj.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://gf.shxzukj.cn

[S03] C：读入整数
来源：http://zu.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://lp.shxzukj.cn

[S04] C：字符串复制
来源：http://ls.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jy.asd995.cn

[S05] C：字符串长度
来源：http://gv.9csxet.cn

strlen(s)
来源：http://wa.asd995.cn

[S06] C：字符串比较
来源：http://ww.muxihuayi.cn

strcmp(a, b) == 0
来源：http://ot.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://sm.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xn.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://gl.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ck.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://lu.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fz.newstarts.cn

[S10] C：指针与解引用
来源：http://bx.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://vq.yuexingan06.cn

[S11] C：逐行读文件
来源：http://ch.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://pu.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bz.colortex.cn

fclose(f);
来源：http://nz.shtwfgs.cn

[S12] C：写文件
来源：http://mo.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qz.9csxet.cn

[S13] C：宏定义
来源：http://pk.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xe.nicolike.cn

[S14] C：枚举
来源：http://qr.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://lo.nszjky.cn

[S15] C：类型转换
来源：http://ss.nszjky.cn

(double) a / b
来源：http://fe.szsharing.cn

[S16] C：位操作置位
来源：http://vv.shxzskj.cn

x |= (1 << 3);
来源：http://lu.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://yu.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fi.nszjky.cn

[S18] C：命令行参数
来源：http://qm.muxihuayi.cn

int main(int argc, char **argv)
来源：http://sp.bookmarksfly.cn

[S19] C：快速排序
来源：http://bo.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ue.szxytkj.cn

[S20] C：二分查找
来源：http://zu.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://se.szxytkj.cn

[S21] C：字符类别判断
来源：http://gf.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ak.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://hb.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ss.hahajie.cn

[S23] C：随机数
来源：http://eu.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jt.asd995.cn

[S24] C：获取本地时间
来源：http://hj.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ma.lnxyls.cn

[S25] C：内存拷贝
来源：http://uy.shtwfgs.cn

memcpy(dst, src, n);
来源：http://md.jianghongdianzi.cn

[S26] C：内存清零
来源：http://ka.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://nr.wgjwhj.cn

[S27] C：定义常量
来源：http://ri.hnjuh.cn

const double PI = 3.14159;
来源：http://kh.jianghongdianzi.cn

[S28] C：静态变量
来源：http://jh.wgjwhj.cn

static int counter = 0;
来源：http://fm.szsharing.cn

[S29] C：变参函数
来源：http://sc.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yd.lnxyls.cn

[S30] C：头文件保护
来源：http://hf.panjiajie.cn

#ifndef X_H
来源：http://hl.huanxung.cn

#define X_H
来源：http://dd.szxytkj.cn

#endif
来源：http://pe.521024.cn

[S31] C++：Hello World
来源：http://sn.huanxung.cn

#include <iostream>
来源：http://xs.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://st.szxytkj.cn

[S32] C++：字符串
来源：http://iv.521024.cn

std::string s = "hi";  s += "!";
来源：http://ws.colortex.cn

[S33] C++：vector 增删
来源：http://dy.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nx.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://xy.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://ib.wgjwhj.cn

[S35] C++：map
来源：http://zp.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fe.9csxet.cn

[S36] C++：unordered_map
来源：http://rc.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://km.wgjwhj.cn

[S37] C++：set
来源：http://tg.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eh.huixinmuqiang.cn

[S38] C++：排序
来源：http://ia.colortex.cn

std::sort(v.begin(), v.end());
来源：http://ig.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://qw.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kt.hahajie.cn

[S40] C++：查找元素
来源：http://ah.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dz.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://ax.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tt.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://uz.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://ml.hnjuh.cn

[S43] C++：智能指针
来源：http://va.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://wl.haigaiapp.cn

[S44] C++：引用传参
来源：http://ue.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://oa.huixinmuqiang.cn

[S45] C++：lambda
来源：http://yk.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xl.wgjwhj.cn

[S46] C++：函数模板
来源：http://eo.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://id.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://wp.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ut.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://cz.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tw.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://fs.panjiajie.cn

[S49] C++：写文件
来源：http://fv.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pq.huanxung.cn

[S50] C++：格式化数字
来源：http://ag.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xr.nicolike.cn

[S51] C++：显式类型转换
来源：http://sq.szsharing.cn

static_cast<double>(a) / b
来源：http://ru.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://if.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://nc.jctech888.com.cn

[S53] C++：移动语义
来源：http://ad.asd995.cn

std::vector<int> w = std::move(v);
来源：http://yy.nszjky.cn

[S54] C++：异常处理
来源：http://fy.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rm.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://ky.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mj.wgjwhj.cn

[S56] C++：optional
来源：http://vr.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ib.jctech888.com.cn

[S57] C++：编译期常量
来源：http://um.nicolike.cn

constexpr int N = 10;
来源：http://up.gzmigu.cn

[S58] C++：命名空间
来源：http://nr.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://rl.huanxung.cn

[S59] C++：静态断言
来源：http://le.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ki.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://wc.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zo.huixinmuqiang.cn

================================================================================
来源：http://ra.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xu.521024.cn

================================================================================
来源：http://lw.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://sj.asd995.cn

println("Hello")
来源：http://ou.szxytkj.cn

[T02] Kotlin：变量
来源：http://ec.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kk.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://yr.521024.cn

"值: $b"
来源：http://hl.huanxung.cn

[T04] Kotlin：空安全
来源：http://tp.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://zn.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://bt.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lm.asd995.cn

[T06] Kotlin：集合映射
来源：http://ii.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wf.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://ck.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wu.shxzukj.cn

[T08] Kotlin：数据类
来源：http://yz.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://sp.colortex.cn

[T09] Kotlin：扩展函数
来源：http://ph.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://yy.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://lb.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://na.panjiajie.cn

[T11] Kotlin：协程
来源：http://oe.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bh.9csxet.cn

[T12] Kotlin：解构声明
来源：http://ij.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://nj.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://bi.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://tl.huanxung.cn

[T14] Kotlin：循环
来源：http://tm.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://ab.521024.cn

[T15] Kotlin：接口
来源：http://kr.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://yz.lnxyls.cn

[T16] Swift：Hello World
来源：http://gj.521024.cn

print("Hello")
来源：http://mj.hahajie.cn

[T17] Swift：变量与常量
来源：http://wl.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ej.szxytkj.cn

[T18] Swift：字符串插值
来源：http://ji.shtwfgs.cn

"值: \(b)"
来源：http://ed.nszjky.cn

[T19] Swift：可选绑定
来源：http://bq.haigaiapp.cn

if let n = opt { print(n) }
来源：http://st.panjiajie.cn

[T20] Swift：数组操作
来源：http://ys.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oc.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://kh.haigaiapp.cn

for x in a { print(x) }
来源：http://ts.chemitech.net.cn

[T22] Swift：字典
来源：http://st.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zn.521024.cn

[T23] Swift：函数
来源：http://md.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qo.jctech888.com.cn

[T24] Swift：闭包
来源：http://yw.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ei.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://bs.wgjwhj.cn

struct P { var x: Int }
来源：http://af.panjiajie.cn

[T26] Swift：类与重写
来源：http://ju.hahajie.cn

class A: Base { override func f() {} }
来源：http://dt.szsharing.cn

[T27] Swift：错误处理
来源：http://on.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://gn.bookmarksfly.cn

[T28] Swift：枚举
来源：http://yh.shxzukj.cn

enum Color { case red, green }
来源：http://cr.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://zh.yuexingan06.cn

guard let x = opt else { return }
来源：http://mb.nicolike.cn

[T30] Swift：协议
来源：http://yp.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://ww.shtwfgs.cn

[T31] Lua：Hello World
来源：http://ax.nicolike.cn

print("Hello")
来源：http://yz.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://ai.9csxet.cn

local a = 1
来源：http://lo.nicolike.cn

[T33] Lua：表（数组）
来源：http://sn.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mg.muxihuayi.cn

[T34] Lua：遍历表
来源：http://di.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sd.nszjky.cn

[T35] Lua：字典表
来源：http://cn.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://oq.nicolike.cn

[T36] Lua：函数
来源：http://rn.chemitech.net.cn

function add(a, b) return a + b end
来源：http://nb.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://jg.bjjhwx.cn

"a" .. "b"
来源：http://nu.hahajie.cn

[T38] Lua：条件
来源：http://jx.shtwfgs.cn

if x > 0 then print("正") end
来源：http://ho.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://zl.szsharing.cn

string.find(s, "%d+")
来源：http://ss.yuntaijiaju.cn

[T40] Lua：元表
来源：http://yd.nszjky.cn

setmetatable({}, { __index = base })
来源：http://ts.muxihuayi.cn

[T41] Perl：Hello World
来源：http://zf.muxihuayi.cn

print "Hello\n";
来源：http://vn.shxzskj.cn

[T42] Perl：变量类型
来源：http://xq.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rp.colortex.cn


<!-- 参考信息 -->