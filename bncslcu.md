代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://pe.huanxung.cn

[R32] 参数个数校验
来源：http://jx.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cv.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://kz.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kj.szxytkj.cn

[R34] 退出时清理
来源：http://bk.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lg.newstarts.cn

[R35] 后台执行并等待
来源：http://fc.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dj.gzmigu.cn

[R36] 并发执行多个任务
来源：http://rq.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hd.huanxung.cn

[R37] 把输出赋给变量
来源：http://ub.lnxyls.cn

files=$(ls -1)
来源：http://qa.wgjwhj.cn

[R38] 管道串联
来源：http://qc.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://yc.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://hy.haigaiapp.cn

cmd > out.log 2>&1
来源：http://fc.szxytkj.cn

[R40] 追加写日志
来源：http://dk.panjiajie.cn

echo "log" >> out.log
来源：http://lr.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://zw.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://qb.haigaiapp.cn

[R42] 输入重定向
来源：http://xs.huixinmuqiang.cn

wc -l < a.txt
来源：http://fs.asd995.cn

[R43] 按名字查找文件
来源：http://hf.colortex.cn

find . -name "*.log" -type f
来源：http://sw.szxytkj.cn

[R44] 按修改时间查找
来源：http://dx.szxytkj.cn

find . -mtime -7 -type f
来源：http://ea.yuexingan06.cn

[R45] 批量删除
来源：http://pv.asd995.cn

find . -name "*.tmp" -delete
来源：http://nk.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://jn.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hf.wgjwhj.cn

[R47] sed 单行替换
来源：http://uc.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ci.huanxung.cn

[R48] awk 取指定列
来源：http://kw.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://qa.nicolike.cn

[R49] awk 带条件
来源：http://pd.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gi.szsharing.cn

[R50] awk 求和
来源：http://fi.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ro.yuexingan06.cn

[R51] 排序去重取前几
来源：http://hq.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lf.huanxung.cn

[R52] 统计行数
来源：http://vv.chemitech.net.cn

wc -l a.txt
来源：http://cx.521024.cn

[R53] 查看文件头与实时尾
来源：http://wt.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ns.hnjuh.cn

[R54] 比较两个文件
来源：http://lt.yuexingan06.cn

diff a.txt b.txt
来源：http://fm.jctech888.com.cn

[R55] 压缩与解压
来源：http://se.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vn.jctech888.com.cn

[R56] 远程拷贝
来源：http://ou.asd995.cn

scp file user@host:/path/
来源：http://in.hnjuh.cn

[R57] 远程执行命令
来源：http://mz.huixiangedu.cn

ssh user@host 'uptime'
来源：http://ta.asd995.cn

[R58] 下载文件
来源：http://vx.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ka.yuexingan06.cn

[R59] 发 POST JSON
来源：http://vo.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jb.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://tm.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cd.yuexingan06.cn

[R61] 磁盘占用
来源：http://nk.nszjky.cn

df -h;  du -sh *
来源：http://bk.asd995.cn

[R62] 找最占空间的文件
来源：http://hg.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://ja.shxzukj.cn

[R63] 内存与进程
来源：http://rf.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://jv.jctech888.com.cn

[R64] 结束进程
来源：http://us.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://qx.jctech888.com.cn

[R65] 查看端口占用
来源：http://ls.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qx.szsharing.cn

[R66] 定时任务
来源：http://xw.hnjuh.cn

crontab -e;  crontab -l
来源：http://uo.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://zk.521024.cn

openssl rand -hex 16
来源：http://xm.huixiangedu.cn

[R68] 计算文件校验值
来源：http://wo.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vc.yuexingan06.cn

[R69] 生成随机密码
来源：http://he.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://ub.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://br.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://fq.jctech888.com.cn

[R71] 日期格式化
来源：http://lm.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ri.hahajie.cn

[R72] 等待端口就绪
来源：http://ib.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ud.colortex.cn

[R73] 分割大日志
来源：http://fy.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://qj.9csxet.cn

[R74] 批量重命名
来源：http://zf.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gg.hahajie.cn

[R75] 导出环境变量
来源：http://dv.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://gx.shxzskj.cn

[R76] 使用临时文件
来源：http://db.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sa.hnjuh.cn

[R77] 读取用户输入
来源：http://ok.panjiajie.cn

read -rp "请输入: " ans
来源：http://jx.szsharing.cn

[R78] 交互式菜单
来源：http://xy.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rf.shtwfgs.cn

[R79] 解析命令行选项
来源：http://mh.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dm.521024.cn

[R80] 查看脚本执行耗时
来源：http://vy.shxzskj.cn

time ./run.sh
来源：http://xa.yuexingan06.cn

================================================================================
来源：http://zu.jctech888.com.cn

S. C / C++ 专题
来源：http://at.newstarts.cn

================================================================================
来源：http://fq.bjjhwx.cn

[S01] C：Hello World
来源：http://an.hnjuh.cn

#include <stdio.h>
来源：http://zm.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zn.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://as.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://dp.shxzskj.cn

[S03] C：读入整数
来源：http://yl.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://cu.asd995.cn

[S04] C：字符串复制
来源：http://ng.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zb.panjiajie.cn

[S05] C：字符串长度
来源：http://my.huixiangedu.cn

strlen(s)
来源：http://rn.shxzukj.cn

[S06] C：字符串比较
来源：http://ua.chemitech.net.cn

strcmp(a, b) == 0
来源：http://aj.9csxet.cn

[S07] C：数组遍历求和
来源：http://rv.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kh.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://ek.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pg.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://sn.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sy.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://wp.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://we.9csxet.cn

[S11] C：逐行读文件
来源：http://nb.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://nr.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dh.shxzskj.cn

fclose(f);
来源：http://il.huixiangedu.cn

[S12] C：写文件
来源：http://je.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sd.9csxet.cn

[S13] C：宏定义
来源：http://lq.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tq.bjjhwx.cn

[S14] C：枚举
来源：http://jk.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://py.yuexingan06.cn

[S15] C：类型转换
来源：http://pc.colortex.cn

(double) a / b
来源：http://se.shtwfgs.cn

[S16] C：位操作置位
来源：http://wx.muxihuayi.cn

x |= (1 << 3);
来源：http://em.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://nt.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ie.yuexingan06.cn

[S18] C：命令行参数
来源：http://ap.jctech888.com.cn

int main(int argc, char **argv)
来源：http://ec.yuexingan06.cn

[S19] C：快速排序
来源：http://qu.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jd.szxytkj.cn

[S20] C：二分查找
来源：http://mb.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dt.hnjuh.cn

[S21] C：字符类别判断
来源：http://mw.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hu.9csxet.cn

[S22] C：字符串转数字
来源：http://kc.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xf.asd995.cn

[S23] C：随机数
来源：http://aa.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cu.wgjwhj.cn

[S24] C：获取本地时间
来源：http://ek.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://st.szsharing.cn

[S25] C：内存拷贝
来源：http://lp.huixiangedu.cn

memcpy(dst, src, n);
来源：http://tm.szxytkj.cn

[S26] C：内存清零
来源：http://wm.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://mk.asd995.cn

[S27] C：定义常量
来源：http://ln.yuexingan06.cn

const double PI = 3.14159;
来源：http://jg.jctech888.com.cn

[S28] C：静态变量
来源：http://zh.gzmigu.cn

static int counter = 0;
来源：http://pn.colortex.cn

[S29] C：变参函数
来源：http://kl.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eu.shxzskj.cn

[S30] C：头文件保护
来源：http://hk.wgjwhj.cn

#ifndef X_H
来源：http://gr.shxzskj.cn

#define X_H
来源：http://qm.hahajie.cn

#endif
来源：http://ki.shxzskj.cn

[S31] C++：Hello World
来源：http://ob.szxytkj.cn

#include <iostream>
来源：http://go.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://gk.jianghongdianzi.cn

[S32] C++：字符串
来源：http://pu.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://mz.szxytkj.cn

[S33] C++：vector 增删
来源：http://rc.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hr.hahajie.cn

[S34] C++：遍历 vector
来源：http://zz.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://ra.huixiangedu.cn

[S35] C++：map
来源：http://ee.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dp.haigaiapp.cn

[S36] C++：unordered_map
来源：http://dq.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nf.521024.cn

[S37] C++：set
来源：http://ae.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oh.shtwfgs.cn

[S38] C++：排序
来源：http://su.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://rr.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://dn.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xg.szsharing.cn

[S40] C++：查找元素
来源：http://uh.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qj.hahajie.cn

[S41] C++：类与构造函数
来源：http://zb.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://el.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://gz.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://js.shxzukj.cn

[S43] C++：智能指针
来源：http://lk.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://pp.jctech888.com.cn

[S44] C++：引用传参
来源：http://bd.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://cm.muxihuayi.cn

[S45] C++：lambda
来源：http://tg.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tc.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://he.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pz.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://oc.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ur.shxzukj.cn

[S48] C++：逐行读文件
来源：http://gz.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ms.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://tk.chemitech.net.cn

[S49] C++：写文件
来源：http://oj.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tx.gzmigu.cn

[S50] C++：格式化数字
来源：http://zr.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mb.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://ya.hahajie.cn

static_cast<double>(a) / b
来源：http://kc.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://pc.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://jj.colortex.cn

[S53] C++：移动语义
来源：http://by.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://gi.asd995.cn

[S54] C++：异常处理
来源：http://ph.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://al.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://pl.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ht.huixinmuqiang.cn

[S56] C++：optional
来源：http://gz.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zz.asd995.cn

[S57] C++：编译期常量
来源：http://ji.nszjky.cn

constexpr int N = 10;
来源：http://fs.haigaiapp.cn

[S58] C++：命名空间
来源：http://au.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://tb.gzmigu.cn

[S59] C++：静态断言
来源：http://oc.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://vd.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hg.shtwfgs.cn

================================================================================
来源：http://yf.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xe.521024.cn

================================================================================
来源：http://ae.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://ou.muxihuayi.cn

println("Hello")
来源：http://qs.shxzukj.cn

[T02] Kotlin：变量
来源：http://rk.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uc.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://ls.9csxet.cn

"值: $b"
来源：http://go.lnxyls.cn

[T04] Kotlin：空安全
来源：http://ag.colortex.cn

val n: String? = null;  n?.length
来源：http://lw.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://zg.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dk.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://zp.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ki.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://uz.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yn.gzmigu.cn

[T08] Kotlin：数据类
来源：http://cz.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://zr.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://bm.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://va.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://ad.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hb.huixiangedu.cn

[T11] Kotlin：协程
来源：http://lk.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ab.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://rh.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://ko.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://un.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://im.newstarts.cn

[T14] Kotlin：循环
来源：http://rj.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://iq.9csxet.cn

[T15] Kotlin：接口
来源：http://ys.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://ys.shxzukj.cn

[T16] Swift：Hello World
来源：http://gt.bjjhwx.cn

print("Hello")
来源：http://hx.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://oo.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://ao.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://vh.hnjuh.cn

"值: \(b)"
来源：http://ao.shxzskj.cn

[T19] Swift：可选绑定
来源：http://ka.szsharing.cn

if let n = opt { print(n) }
来源：http://kb.nicolike.cn

[T20] Swift：数组操作
来源：http://tj.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nn.newstarts.cn

[T21] Swift：遍历
来源：http://bk.newstarts.cn

for x in a { print(x) }
来源：http://mc.jianghongdianzi.cn

[T22] Swift：字典
来源：http://js.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://si.gzmigu.cn

[T23] Swift：函数
来源：http://xs.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vm.nszjky.cn

[T24] Swift：闭包
来源：http://ah.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ql.asd995.cn

[T25] Swift：结构体
来源：http://lm.nicolike.cn

struct P { var x: Int }
来源：http://pa.lnxyls.cn

[T26] Swift：类与重写
来源：http://yl.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://uv.chemitech.net.cn

[T27] Swift：错误处理
来源：http://op.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://oz.shxzskj.cn

[T28] Swift：枚举
来源：http://iq.shtwfgs.cn

enum Color { case red, green }
来源：http://be.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://hk.lnxyls.cn

guard let x = opt else { return }
来源：http://rx.asd995.cn

[T30] Swift：协议
来源：http://nx.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://aj.chemitech.net.cn

[T31] Lua：Hello World
来源：http://sp.gzmigu.cn

print("Hello")
来源：http://hw.gzmigu.cn

[T32] Lua：局部变量
来源：http://wd.gzmigu.cn

local a = 1
来源：http://yx.shxzskj.cn

[T33] Lua：表（数组）
来源：http://km.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wf.521024.cn

[T34] Lua：遍历表
来源：http://br.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rh.newstarts.cn


<!-- 参考信息 -->