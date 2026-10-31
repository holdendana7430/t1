代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hq.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://bx.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xa.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://nf.colortex.cn

files=$(ls -1)
来源：http://ma.hnjuh.cn

[R38] 管道串联
来源：http://hb.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://cq.colortex.cn

[R39] 重定向标准输出与错误
来源：http://nf.panjiajie.cn

cmd > out.log 2>&1
来源：http://yr.haigaiapp.cn

[R40] 追加写日志
来源：http://wm.wgjwhj.cn

echo "log" >> out.log
来源：http://wo.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://mf.szsharing.cn

cmd >/dev/null 2>&1
来源：http://er.szxytkj.cn

[R42] 输入重定向
来源：http://sw.hnjuh.cn

wc -l < a.txt
来源：http://yc.huixiangedu.cn

[R43] 按名字查找文件
来源：http://en.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://kk.huixiangedu.cn

[R44] 按修改时间查找
来源：http://pu.panjiajie.cn

find . -mtime -7 -type f
来源：http://vq.haigaiapp.cn

[R45] 批量删除
来源：http://jy.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://qo.lnxyls.cn

[R46] 递归替换文件内容
来源：http://zc.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ao.yuexingan06.cn

[R47] sed 单行替换
来源：http://qe.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://we.newstarts.cn

[R48] awk 取指定列
来源：http://wr.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://se.szsharing.cn

[R49] awk 带条件
来源：http://mg.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sp.shtwfgs.cn

[R50] awk 求和
来源：http://mv.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ac.shxzukj.cn

[R51] 排序去重取前几
来源：http://no.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fu.shxzskj.cn

[R52] 统计行数
来源：http://cr.jianghongdianzi.cn

wc -l a.txt
来源：http://ez.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://na.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pr.9csxet.cn

[R54] 比较两个文件
来源：http://yu.yuexingan06.cn

diff a.txt b.txt
来源：http://ex.9csxet.cn

[R55] 压缩与解压
来源：http://jz.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tb.nicolike.cn

[R56] 远程拷贝
来源：http://ce.9csxet.cn

scp file user@host:/path/
来源：http://yc.nszjky.cn

[R57] 远程执行命令
来源：http://gq.haigaiapp.cn

ssh user@host 'uptime'
来源：http://dh.yuntaijiaju.cn

[R58] 下载文件
来源：http://iy.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cd.panjiajie.cn

[R59] 发 POST JSON
来源：http://em.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vo.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://jp.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jd.nicolike.cn

[R61] 磁盘占用
来源：http://pm.colortex.cn

df -h;  du -sh *
来源：http://pi.asd995.cn

[R62] 找最占空间的文件
来源：http://uq.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://zf.yuntaijiaju.cn

[R63] 内存与进程
来源：http://oe.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://em.lnxyls.cn

[R64] 结束进程
来源：http://wu.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://sy.nszjky.cn

[R65] 查看端口占用
来源：http://dv.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lk.wgjwhj.cn

[R66] 定时任务
来源：http://pt.gzmigu.cn

crontab -e;  crontab -l
来源：http://la.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://xp.shxzukj.cn

openssl rand -hex 16
来源：http://ej.9csxet.cn

[R68] 计算文件校验值
来源：http://cg.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lm.chemitech.net.cn

[R69] 生成随机密码
来源：http://ga.521024.cn

head -c 16 /dev/urandom | base64
来源：http://ig.lnxyls.cn

[R70] 时间戳与互转
来源：http://fy.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://xc.colortex.cn

[R71] 日期格式化
来源：http://vp.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pa.hnjuh.cn

[R72] 等待端口就绪
来源：http://tk.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uf.hahajie.cn

[R73] 分割大日志
来源：http://qm.shxzskj.cn

split -l 1000 big.log part_
来源：http://vq.bookmarksfly.cn

[R74] 批量重命名
来源：http://ka.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oz.asd995.cn

[R75] 导出环境变量
来源：http://nn.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://gb.bookmarksfly.cn

[R76] 使用临时文件
来源：http://hn.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ee.gzmigu.cn

[R77] 读取用户输入
来源：http://br.colortex.cn

read -rp "请输入: " ans
来源：http://rs.gzmigu.cn

[R78] 交互式菜单
来源：http://uo.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rl.yuexingan06.cn

[R79] 解析命令行选项
来源：http://jd.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wt.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://qz.szsharing.cn

time ./run.sh
来源：http://ot.nicolike.cn

================================================================================
来源：http://eh.wgjwhj.cn

S. C / C++ 专题
来源：http://dh.yuexingan06.cn

================================================================================
来源：http://yy.521024.cn

[S01] C：Hello World
来源：http://bq.huixiangedu.cn

#include <stdio.h>
来源：http://fw.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fp.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://bw.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://sl.haigaiapp.cn

[S03] C：读入整数
来源：http://hs.asd995.cn

int x; scanf("%d", &x);
来源：http://os.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://ks.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://op.lnxyls.cn

[S05] C：字符串长度
来源：http://ze.colortex.cn

strlen(s)
来源：http://ug.gzmigu.cn

[S06] C：字符串比较
来源：http://it.hnjuh.cn

strcmp(a, b) == 0
来源：http://kh.lnxyls.cn

[S07] C：数组遍历求和
来源：http://fk.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oo.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://hq.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aw.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://aa.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tt.gzmigu.cn

[S10] C：指针与解引用
来源：http://ud.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://cu.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://ql.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://wk.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ba.nicolike.cn

fclose(f);
来源：http://ld.chemitech.net.cn

[S12] C：写文件
来源：http://jh.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ne.chemitech.net.cn

[S13] C：宏定义
来源：http://re.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fi.shxzukj.cn

[S14] C：枚举
来源：http://th.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ax.shtwfgs.cn

[S15] C：类型转换
来源：http://ra.yuexingan06.cn

(double) a / b
来源：http://if.nicolike.cn

[S16] C：位操作置位
来源：http://uz.shtwfgs.cn

x |= (1 << 3);
来源：http://oj.521024.cn

[S17] C：安全拼接字符串
来源：http://zx.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xu.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://dj.haigaiapp.cn

int main(int argc, char **argv)
来源：http://ov.colortex.cn

[S19] C：快速排序
来源：http://zk.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ye.521024.cn

[S20] C：二分查找
来源：http://oz.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jh.szxytkj.cn

[S21] C：字符类别判断
来源：http://ff.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dm.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://ca.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dw.gzmigu.cn

[S23] C：随机数
来源：http://cb.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fb.colortex.cn

[S24] C：获取本地时间
来源：http://sq.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://va.szsharing.cn

[S25] C：内存拷贝
来源：http://wg.9csxet.cn

memcpy(dst, src, n);
来源：http://gk.gzmigu.cn

[S26] C：内存清零
来源：http://qh.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://tx.yuntaijiaju.cn

[S27] C：定义常量
来源：http://eu.szxytkj.cn

const double PI = 3.14159;
来源：http://xq.huixiangedu.cn

[S28] C：静态变量
来源：http://kk.hnjuh.cn

static int counter = 0;
来源：http://yr.yuntaijiaju.cn

[S29] C：变参函数
来源：http://jd.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hw.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://td.9csxet.cn

#ifndef X_H
来源：http://kz.szxytkj.cn

#define X_H
来源：http://mu.hahajie.cn

#endif
来源：http://ra.wgjwhj.cn

[S31] C++：Hello World
来源：http://ba.muxihuayi.cn

#include <iostream>
来源：http://bv.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://qw.shxzukj.cn

[S32] C++：字符串
来源：http://jx.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://mg.nicolike.cn

[S33] C++：vector 增删
来源：http://xn.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tl.szsharing.cn

[S34] C++：遍历 vector
来源：http://mk.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://wi.bjjhwx.cn

[S35] C++：map
来源：http://gf.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eq.newstarts.cn

[S36] C++：unordered_map
来源：http://zu.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mo.nicolike.cn

[S37] C++：set
来源：http://bv.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cc.haigaiapp.cn

[S38] C++：排序
来源：http://df.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://xv.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://uq.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bf.szxytkj.cn

[S40] C++：查找元素
来源：http://id.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ho.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://ws.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://af.521024.cn

[S42] C++：继承与虚函数
来源：http://hx.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://tz.shxzukj.cn

[S43] C++：智能指针
来源：http://dt.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://xg.haigaiapp.cn

[S44] C++：引用传参
来源：http://am.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://sd.9csxet.cn

[S45] C++：lambda
来源：http://fb.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uo.shtwfgs.cn

[S46] C++：函数模板
来源：http://wb.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jb.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://zc.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ia.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://nt.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tr.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://mp.hnjuh.cn

[S49] C++：写文件
来源：http://ns.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lo.hnjuh.cn

[S50] C++：格式化数字
来源：http://pd.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jk.gzmigu.cn

[S51] C++：显式类型转换
来源：http://ab.newstarts.cn

static_cast<double>(a) / b
来源：http://ka.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://ml.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://ox.muxihuayi.cn

[S53] C++：移动语义
来源：http://cw.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ob.521024.cn

[S54] C++：异常处理
来源：http://kz.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bd.asd995.cn

[S55] C++：结构化绑定
来源：http://qf.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wl.yuntaijiaju.cn

[S56] C++：optional
来源：http://bb.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mb.nszjky.cn

[S57] C++：编译期常量
来源：http://tp.huixinmuqiang.cn

constexpr int N = 10;
来源：http://iz.yuexingan06.cn

[S58] C++：命名空间
来源：http://hl.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://wn.shxzskj.cn

[S59] C++：静态断言
来源：http://fl.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fg.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://cc.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yh.bookmarksfly.cn

================================================================================
来源：http://sv.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hj.hahajie.cn

================================================================================
来源：http://el.hahajie.cn

[T01] Kotlin：Hello World
来源：http://jp.chemitech.net.cn

println("Hello")
来源：http://ma.wgjwhj.cn

[T02] Kotlin：变量
来源：http://sp.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mq.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://tl.shtwfgs.cn

"值: $b"
来源：http://zh.panjiajie.cn

[T04] Kotlin：空安全
来源：http://fl.szsharing.cn

val n: String? = null;  n?.length
来源：http://mz.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://lk.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jk.9csxet.cn

[T06] Kotlin：集合映射
来源：http://vi.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bd.asd995.cn

[T07] Kotlin：集合过滤
来源：http://hk.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hc.newstarts.cn

[T08] Kotlin：数据类
来源：http://ih.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://mm.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://yp.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://vh.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://gz.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bz.asd995.cn

[T11] Kotlin：协程
来源：http://nh.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hj.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://hq.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://ll.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://uh.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://ax.haigaiapp.cn

[T14] Kotlin：循环
来源：http://eh.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://hh.wgjwhj.cn

[T15] Kotlin：接口
来源：http://jy.hahajie.cn

interface Shape { fun area(): Double }
来源：http://ow.chemitech.net.cn

[T16] Swift：Hello World
来源：http://rx.huixiangedu.cn

print("Hello")
来源：http://qy.521024.cn

[T17] Swift：变量与常量
来源：http://ts.nszjky.cn

var a = 1;  let b = 2
来源：http://pj.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://xi.wgjwhj.cn

"值: \(b)"
来源：http://ab.lnxyls.cn

[T19] Swift：可选绑定
来源：http://vs.gzmigu.cn

if let n = opt { print(n) }
来源：http://te.szxytkj.cn

[T20] Swift：数组操作
来源：http://xu.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oz.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://kd.huixinmuqiang.cn

for x in a { print(x) }
来源：http://ua.panjiajie.cn

[T22] Swift：字典
来源：http://ft.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ci.gzmigu.cn

[T23] Swift：函数
来源：http://cf.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kf.nszjky.cn

[T24] Swift：闭包
来源：http://qb.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://no.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://yy.bookmarksfly.cn

struct P { var x: Int }
来源：http://az.wgjwhj.cn

[T26] Swift：类与重写
来源：http://zh.szsharing.cn

class A: Base { override func f() {} }
来源：http://sz.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://xb.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://be.jctech888.com.cn

[T28] Swift：枚举
来源：http://ww.asd995.cn

enum Color { case red, green }
来源：http://go.asd995.cn

[T29] Swift：guard 提前返回
来源：http://ad.nszjky.cn

guard let x = opt else { return }
来源：http://oc.hahajie.cn

[T30] Swift：协议
来源：http://fl.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://so.9csxet.cn

[T31] Lua：Hello World
来源：http://uj.hahajie.cn

print("Hello")
来源：http://hn.nszjky.cn

[T32] Lua：局部变量
来源：http://hd.shxzskj.cn

local a = 1
来源：http://rb.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://rw.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mj.9csxet.cn

[T34] Lua：遍历表
来源：http://cp.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xa.shxzskj.cn

[T35] Lua：字典表
来源：http://ds.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://jq.muxihuayi.cn

[T36] Lua：函数
来源：http://ux.szsharing.cn

function add(a, b) return a + b end
来源：http://zp.9csxet.cn

[T37] Lua：字符串拼接
来源：http://vx.bookmarksfly.cn

"a" .. "b"
来源：http://gr.szxytkj.cn

[T38] Lua：条件
来源：http://mw.panjiajie.cn

if x > 0 then print("正") end
来源：http://wo.nszjky.cn


<!-- 参考信息 -->