代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mt.asd995.cn

[R34] 退出时清理
来源：http://eq.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qv.huixiangedu.cn

[R35] 后台执行并等待
来源：http://sd.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zf.newstarts.cn

[R36] 并发执行多个任务
来源：http://ul.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bm.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://xm.shxzskj.cn

files=$(ls -1)
来源：http://hc.shxzukj.cn

[R38] 管道串联
来源：http://bx.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://na.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://ci.huanxung.cn

cmd > out.log 2>&1
来源：http://kh.yuntaijiaju.cn

[R40] 追加写日志
来源：http://rv.lnxyls.cn

echo "log" >> out.log
来源：http://he.yuexingan06.cn

[R41] 丢弃输出
来源：http://cg.9csxet.cn

cmd >/dev/null 2>&1
来源：http://hr.bjjhwx.cn

[R42] 输入重定向
来源：http://rc.yuntaijiaju.cn

wc -l < a.txt
来源：http://uz.nicolike.cn

[R43] 按名字查找文件
来源：http://bv.haigaiapp.cn

find . -name "*.log" -type f
来源：http://yi.521024.cn

[R44] 按修改时间查找
来源：http://gr.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://bj.huixiangedu.cn

[R45] 批量删除
来源：http://wn.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://rk.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://zt.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hk.szsharing.cn

[R47] sed 单行替换
来源：http://nh.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fm.521024.cn

[R48] awk 取指定列
来源：http://ox.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://ev.shtwfgs.cn

[R49] awk 带条件
来源：http://vv.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://il.huixinmuqiang.cn

[R50] awk 求和
来源：http://gd.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ij.nszjky.cn

[R51] 排序去重取前几
来源：http://mk.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lj.hnjuh.cn

[R52] 统计行数
来源：http://hy.huixiangedu.cn

wc -l a.txt
来源：http://rm.colortex.cn

[R53] 查看文件头与实时尾
来源：http://bt.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xn.shxzukj.cn

[R54] 比较两个文件
来源：http://mt.szsharing.cn

diff a.txt b.txt
来源：http://wh.bookmarksfly.cn

[R55] 压缩与解压
来源：http://ov.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sb.shtwfgs.cn

[R56] 远程拷贝
来源：http://cp.521024.cn

scp file user@host:/path/
来源：http://lg.panjiajie.cn

[R57] 远程执行命令
来源：http://ml.hnjuh.cn

ssh user@host 'uptime'
来源：http://hj.yuexingan06.cn

[R58] 下载文件
来源：http://vc.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wt.newstarts.cn

[R59] 发 POST JSON
来源：http://ee.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dz.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://yy.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ra.9csxet.cn

[R61] 磁盘占用
来源：http://bz.gzmigu.cn

df -h;  du -sh *
来源：http://sc.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://qc.colortex.cn

du -ah . | sort -rh | head -10
来源：http://yk.haigaiapp.cn

[R63] 内存与进程
来源：http://et.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://dt.huanxung.cn

[R64] 结束进程
来源：http://xe.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://es.shxzskj.cn

[R65] 查看端口占用
来源：http://hy.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hf.nicolike.cn

[R66] 定时任务
来源：http://uj.asd995.cn

crontab -e;  crontab -l
来源：http://zs.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://tm.huixinmuqiang.cn

openssl rand -hex 16
来源：http://ru.shxzukj.cn

[R68] 计算文件校验值
来源：http://cc.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://io.muxihuayi.cn

[R69] 生成随机密码
来源：http://ma.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://es.newstarts.cn

[R70] 时间戳与互转
来源：http://ok.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://ay.newstarts.cn

[R71] 日期格式化
来源：http://rg.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tm.nszjky.cn

[R72] 等待端口就绪
来源：http://pm.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yl.yuntaijiaju.cn

[R73] 分割大日志
来源：http://sp.szsharing.cn

split -l 1000 big.log part_
来源：http://zb.lnxyls.cn

[R74] 批量重命名
来源：http://wl.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://it.haigaiapp.cn

[R75] 导出环境变量
来源：http://wt.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://aw.hnjuh.cn

[R76] 使用临时文件
来源：http://dz.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xv.jctech888.com.cn

[R77] 读取用户输入
来源：http://zg.szxytkj.cn

read -rp "请输入: " ans
来源：http://ur.muxihuayi.cn

[R78] 交互式菜单
来源：http://if.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rw.jctech888.com.cn

[R79] 解析命令行选项
来源：http://vx.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mn.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://ke.yuexingan06.cn

time ./run.sh
来源：http://cm.jianghongdianzi.cn

================================================================================
来源：http://kl.szxytkj.cn

S. C / C++ 专题
来源：http://em.panjiajie.cn

================================================================================
来源：http://xw.colortex.cn

[S01] C：Hello World
来源：http://mt.newstarts.cn

#include <stdio.h>
来源：http://up.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cd.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://uc.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://ei.asd995.cn

[S03] C：读入整数
来源：http://lb.lnxyls.cn

int x; scanf("%d", &x);
来源：http://pi.yuexingan06.cn

[S04] C：字符串复制
来源：http://fk.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zp.gzmigu.cn

[S05] C：字符串长度
来源：http://np.shtwfgs.cn

strlen(s)
来源：http://wy.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://fy.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://uf.9csxet.cn

[S07] C：数组遍历求和
来源：http://qe.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ib.colortex.cn

[S08] C：动态内存分配与释放
来源：http://rt.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qh.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://ki.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ds.huanxung.cn

[S10] C：指针与解引用
来源：http://fo.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ms.nicolike.cn

[S11] C：逐行读文件
来源：http://ph.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://gg.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sp.colortex.cn

fclose(f);
来源：http://aj.shxzskj.cn

[S12] C：写文件
来源：http://cu.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hx.nszjky.cn

[S13] C：宏定义
来源：http://gl.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ss.haigaiapp.cn

[S14] C：枚举
来源：http://zf.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://hg.asd995.cn

[S15] C：类型转换
来源：http://lc.huanxung.cn

(double) a / b
来源：http://mm.huanxung.cn

[S16] C：位操作置位
来源：http://hg.newstarts.cn

x |= (1 << 3);
来源：http://wx.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://sy.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ke.panjiajie.cn

[S18] C：命令行参数
来源：http://ta.nszjky.cn

int main(int argc, char **argv)
来源：http://fg.huixiangedu.cn

[S19] C：快速排序
来源：http://di.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qk.jianghongdianzi.cn

[S20] C：二分查找
来源：http://ti.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pa.521024.cn

[S21] C：字符类别判断
来源：http://cr.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kw.panjiajie.cn

[S22] C：字符串转数字
来源：http://uz.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://go.shxzskj.cn

[S23] C：随机数
来源：http://no.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ne.shtwfgs.cn

[S24] C：获取本地时间
来源：http://mq.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bj.asd995.cn

[S25] C：内存拷贝
来源：http://ir.shxzskj.cn

memcpy(dst, src, n);
来源：http://ig.shxzskj.cn

[S26] C：内存清零
来源：http://yo.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://mj.haigaiapp.cn

[S27] C：定义常量
来源：http://hf.bjjhwx.cn

const double PI = 3.14159;
来源：http://gd.hnjuh.cn

[S28] C：静态变量
来源：http://aw.wgjwhj.cn

static int counter = 0;
来源：http://uq.gzmigu.cn

[S29] C：变参函数
来源：http://ns.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://js.nicolike.cn

[S30] C：头文件保护
来源：http://lf.bjjhwx.cn

#ifndef X_H
来源：http://rs.newstarts.cn

#define X_H
来源：http://ap.lnxyls.cn

#endif
来源：http://tr.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://fx.hnjuh.cn

#include <iostream>
来源：http://dr.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://fa.nszjky.cn

[S32] C++：字符串
来源：http://pm.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://lz.colortex.cn

[S33] C++：vector 增删
来源：http://pe.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jq.szxytkj.cn

[S34] C++：遍历 vector
来源：http://fc.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://as.huixinmuqiang.cn

[S35] C++：map
来源：http://dg.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vh.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://cn.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ds.gzmigu.cn

[S37] C++：set
来源：http://ro.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zd.hahajie.cn

[S38] C++：排序
来源：http://rw.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://gc.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://cq.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ir.yuexingan06.cn

[S40] C++：查找元素
来源：http://ij.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bn.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://nf.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rl.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://tx.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://cg.asd995.cn

[S43] C++：智能指针
来源：http://gp.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://eq.shxzskj.cn

[S44] C++：引用传参
来源：http://hj.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://cz.yuntaijiaju.cn

[S45] C++：lambda
来源：http://fq.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gc.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://ll.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kg.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://hq.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ty.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://vr.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kz.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://ij.huixinmuqiang.cn

[S49] C++：写文件
来源：http://ze.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fv.lnxyls.cn

[S50] C++：格式化数字
来源：http://jn.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vf.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://os.shxzukj.cn

static_cast<double>(a) / b
来源：http://si.521024.cn

[S52] C++：const 与 noexcept
来源：http://om.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://al.jctech888.com.cn

[S53] C++：移动语义
来源：http://wl.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://ah.chemitech.net.cn

[S54] C++：异常处理
来源：http://va.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lw.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://wo.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wp.panjiajie.cn

[S56] C++：optional
来源：http://cd.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mn.shxzukj.cn

[S57] C++：编译期常量
来源：http://mz.huixiangedu.cn

constexpr int N = 10;
来源：http://fj.shtwfgs.cn

[S58] C++：命名空间
来源：http://bh.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://xn.shxzskj.cn

[S59] C++：静态断言
来源：http://ji.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yy.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://hi.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fr.jctech888.com.cn

================================================================================
来源：http://la.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pr.newstarts.cn

================================================================================
来源：http://ul.nicolike.cn

[T01] Kotlin：Hello World
来源：http://nx.colortex.cn

println("Hello")
来源：http://cx.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://ms.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://if.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://cp.newstarts.cn

"值: $b"
来源：http://fi.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://wp.szsharing.cn

val n: String? = null;  n?.length
来源：http://mz.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://as.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ci.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://of.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fq.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://bv.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://px.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://sp.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://pi.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://zh.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://iw.newstarts.cn

[T10] Kotlin：默认参数
来源：http://op.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vw.wgjwhj.cn

[T11] Kotlin：协程
来源：http://ee.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://so.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://jn.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://ze.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://tq.szsharing.cn

val m = mapOf("a" to 1)
来源：http://qh.yuexingan06.cn

[T14] Kotlin：循环
来源：http://qc.9csxet.cn

for (i in 1..10) println(i)
来源：http://rl.asd995.cn

[T15] Kotlin：接口
来源：http://xs.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://dl.szxytkj.cn

[T16] Swift：Hello World
来源：http://lk.shxzskj.cn

print("Hello")
来源：http://gb.huanxung.cn

[T17] Swift：变量与常量
来源：http://fu.colortex.cn

var a = 1;  let b = 2
来源：http://da.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://go.521024.cn

"值: \(b)"
来源：http://hk.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://mu.colortex.cn

if let n = opt { print(n) }
来源：http://dn.yuexingan06.cn

[T20] Swift：数组操作
来源：http://yi.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zg.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://bi.9csxet.cn

for x in a { print(x) }
来源：http://yz.panjiajie.cn

[T22] Swift：字典
来源：http://ey.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bh.shxzukj.cn

[T23] Swift：函数
来源：http://ve.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qm.szsharing.cn

[T24] Swift：闭包
来源：http://kr.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ii.newstarts.cn

[T25] Swift：结构体
来源：http://wl.jianghongdianzi.cn

struct P { var x: Int }
来源：http://qe.nszjky.cn

[T26] Swift：类与重写
来源：http://ib.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://hn.nszjky.cn

[T27] Swift：错误处理
来源：http://xd.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://aq.521024.cn

[T28] Swift：枚举
来源：http://tw.yuexingan06.cn

enum Color { case red, green }
来源：http://sp.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://wu.9csxet.cn

guard let x = opt else { return }
来源：http://ha.jctech888.com.cn

[T30] Swift：协议
来源：http://do.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://ei.wgjwhj.cn

[T31] Lua：Hello World
来源：http://ja.9csxet.cn

print("Hello")
来源：http://cd.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://fj.wgjwhj.cn

local a = 1
来源：http://hm.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://qz.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fb.9csxet.cn

[T34] Lua：遍历表
来源：http://rg.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mu.haigaiapp.cn

[T35] Lua：字典表
来源：http://lz.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://ip.asd995.cn

[T36] Lua：函数
来源：http://cy.panjiajie.cn

function add(a, b) return a + b end
来源：http://be.haigaiapp.cn


<!-- 参考信息 -->