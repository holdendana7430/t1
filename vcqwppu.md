代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://ok.jctech888.com.cn

[R32] 参数个数校验
来源：http://hd.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xp.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://ol.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hl.szxytkj.cn

[R34] 退出时清理
来源：http://gd.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lx.huixiangedu.cn

[R35] 后台执行并等待
来源：http://pn.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lu.colortex.cn

[R36] 并发执行多个任务
来源：http://zd.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hw.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://rl.asd995.cn

files=$(ls -1)
来源：http://au.colortex.cn

[R38] 管道串联
来源：http://nf.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://pw.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://ov.shtwfgs.cn

cmd > out.log 2>&1
来源：http://pv.muxihuayi.cn

[R40] 追加写日志
来源：http://ob.haigaiapp.cn

echo "log" >> out.log
来源：http://hn.jctech888.com.cn

[R41] 丢弃输出
来源：http://dz.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://kj.hnjuh.cn

[R42] 输入重定向
来源：http://jh.wgjwhj.cn

wc -l < a.txt
来源：http://nm.panjiajie.cn

[R43] 按名字查找文件
来源：http://jf.haigaiapp.cn

find . -name "*.log" -type f
来源：http://lu.shtwfgs.cn

[R44] 按修改时间查找
来源：http://wa.panjiajie.cn

find . -mtime -7 -type f
来源：http://ik.521024.cn

[R45] 批量删除
来源：http://gs.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://cu.panjiajie.cn

[R46] 递归替换文件内容
来源：http://tr.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pw.panjiajie.cn

[R47] sed 单行替换
来源：http://pk.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://od.shtwfgs.cn

[R48] awk 取指定列
来源：http://zi.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://dv.wgjwhj.cn

[R49] awk 带条件
来源：http://uw.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zw.bjjhwx.cn

[R50] awk 求和
来源：http://bk.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dj.521024.cn

[R51] 排序去重取前几
来源：http://rq.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yg.huixiangedu.cn

[R52] 统计行数
来源：http://hk.nicolike.cn

wc -l a.txt
来源：http://rr.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://lh.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://br.hahajie.cn

[R54] 比较两个文件
来源：http://uw.shtwfgs.cn

diff a.txt b.txt
来源：http://dw.muxihuayi.cn

[R55] 压缩与解压
来源：http://lm.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dx.gzmigu.cn

[R56] 远程拷贝
来源：http://or.muxihuayi.cn

scp file user@host:/path/
来源：http://fn.jctech888.com.cn

[R57] 远程执行命令
来源：http://li.shxzskj.cn

ssh user@host 'uptime'
来源：http://zr.lnxyls.cn

[R58] 下载文件
来源：http://dc.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ey.wgjwhj.cn

[R59] 发 POST JSON
来源：http://ok.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tj.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://ea.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yk.hahajie.cn

[R61] 磁盘占用
来源：http://oi.jctech888.com.cn

df -h;  du -sh *
来源：http://ec.shxzukj.cn

[R62] 找最占空间的文件
来源：http://we.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://hn.jctech888.com.cn

[R63] 内存与进程
来源：http://mi.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://ft.szsharing.cn

[R64] 结束进程
来源：http://yf.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://jm.huixiangedu.cn

[R65] 查看端口占用
来源：http://am.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xw.huixiangedu.cn

[R66] 定时任务
来源：http://xs.haigaiapp.cn

crontab -e;  crontab -l
来源：http://tc.9csxet.cn

[R67] 生成随机十六进制串
来源：http://nt.asd995.cn

openssl rand -hex 16
来源：http://yb.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://my.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zp.szsharing.cn

[R69] 生成随机密码
来源：http://nk.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://mo.asd995.cn

[R70] 时间戳与互转
来源：http://an.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://dv.hahajie.cn

[R71] 日期格式化
来源：http://sv.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wx.asd995.cn

[R72] 等待端口就绪
来源：http://wf.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qd.wgjwhj.cn

[R73] 分割大日志
来源：http://bd.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://nz.jctech888.com.cn

[R74] 批量重命名
来源：http://ax.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gh.szsharing.cn

[R75] 导出环境变量
来源：http://xb.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://hd.9csxet.cn

[R76] 使用临时文件
来源：http://fd.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://og.gzmigu.cn

[R77] 读取用户输入
来源：http://zi.huanxung.cn

read -rp "请输入: " ans
来源：http://va.szxytkj.cn

[R78] 交互式菜单
来源：http://jk.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://os.jctech888.com.cn

[R79] 解析命令行选项
来源：http://oi.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://we.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://sb.521024.cn

time ./run.sh
来源：http://tp.yuntaijiaju.cn

================================================================================
来源：http://cl.colortex.cn

S. C / C++ 专题
来源：http://sw.yuexingan06.cn

================================================================================
来源：http://uv.lnxyls.cn

[S01] C：Hello World
来源：http://on.bookmarksfly.cn

#include <stdio.h>
来源：http://ol.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wq.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://mi.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://mv.yuntaijiaju.cn

[S03] C：读入整数
来源：http://sp.lnxyls.cn

int x; scanf("%d", &x);
来源：http://hh.newstarts.cn

[S04] C：字符串复制
来源：http://eb.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://en.521024.cn

[S05] C：字符串长度
来源：http://qw.szsharing.cn

strlen(s)
来源：http://jf.hnjuh.cn

[S06] C：字符串比较
来源：http://fm.asd995.cn

strcmp(a, b) == 0
来源：http://sz.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://wv.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wi.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://cs.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vd.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://cu.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wc.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://eo.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://ym.hahajie.cn

[S11] C：逐行读文件
来源：http://uv.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://xi.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ra.yuexingan06.cn

fclose(f);
来源：http://ak.shxzukj.cn

[S12] C：写文件
来源：http://tq.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fp.colortex.cn

[S13] C：宏定义
来源：http://zd.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nf.huanxung.cn

[S14] C：枚举
来源：http://tc.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://fa.jianghongdianzi.cn

[S15] C：类型转换
来源：http://yb.9csxet.cn

(double) a / b
来源：http://rf.huanxung.cn

[S16] C：位操作置位
来源：http://qe.nszjky.cn

x |= (1 << 3);
来源：http://lq.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://li.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ef.bjjhwx.cn

[S18] C：命令行参数
来源：http://qi.9csxet.cn

int main(int argc, char **argv)
来源：http://vk.panjiajie.cn

[S19] C：快速排序
来源：http://oj.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kn.chemitech.net.cn

[S20] C：二分查找
来源：http://zb.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zu.szxytkj.cn

[S21] C：字符类别判断
来源：http://ab.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nm.huanxung.cn

[S22] C：字符串转数字
来源：http://dy.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zn.huixiangedu.cn

[S23] C：随机数
来源：http://ja.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qs.bjjhwx.cn

[S24] C：获取本地时间
来源：http://mb.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iz.asd995.cn

[S25] C：内存拷贝
来源：http://jr.yuexingan06.cn

memcpy(dst, src, n);
来源：http://kt.nszjky.cn

[S26] C：内存清零
来源：http://ny.newstarts.cn

memset(a, 0, sizeof a);
来源：http://gw.hnjuh.cn

[S27] C：定义常量
来源：http://sz.shxzskj.cn

const double PI = 3.14159;
来源：http://gr.szsharing.cn

[S28] C：静态变量
来源：http://et.lnxyls.cn

static int counter = 0;
来源：http://zt.haigaiapp.cn

[S29] C：变参函数
来源：http://ea.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lj.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://bt.nicolike.cn

#ifndef X_H
来源：http://hc.muxihuayi.cn

#define X_H
来源：http://wj.hnjuh.cn

#endif
来源：http://pi.bjjhwx.cn

[S31] C++：Hello World
来源：http://cf.shxzukj.cn

#include <iostream>
来源：http://ne.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://gv.jctech888.com.cn

[S32] C++：字符串
来源：http://vg.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://zj.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://yz.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gx.nszjky.cn

[S34] C++：遍历 vector
来源：http://qc.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://dq.panjiajie.cn

[S35] C++：map
来源：http://qp.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ss.yuexingan06.cn

[S36] C++：unordered_map
来源：http://hl.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vu.panjiajie.cn

[S37] C++：set
来源：http://eo.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hh.521024.cn

[S38] C++：排序
来源：http://mf.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://cq.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://zu.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ux.lnxyls.cn

[S40] C++：查找元素
来源：http://xd.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yq.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://pl.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tn.newstarts.cn

[S42] C++：继承与虚函数
来源：http://yh.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://pi.yuexingan06.cn

[S43] C++：智能指针
来源：http://vq.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://py.colortex.cn

[S44] C++：引用传参
来源：http://ji.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://ku.yuntaijiaju.cn

[S45] C++：lambda
来源：http://in.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mk.huixiangedu.cn

[S46] C++：函数模板
来源：http://wr.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ne.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://hs.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wx.asd995.cn

[S48] C++：逐行读文件
来源：http://qc.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sl.huanxung.cn

while (std::getline(in, line)) { }
来源：http://lu.huixinmuqiang.cn

[S49] C++：写文件
来源：http://oo.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qh.wgjwhj.cn

[S50] C++：格式化数字
来源：http://ih.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bd.szxytkj.cn

[S51] C++：显式类型转换
来源：http://ia.wgjwhj.cn

static_cast<double>(a) / b
来源：http://us.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://nj.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://dr.colortex.cn

[S53] C++：移动语义
来源：http://ki.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://os.9csxet.cn

[S54] C++：异常处理
来源：http://id.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ft.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://cl.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ff.colortex.cn

[S56] C++：optional
来源：http://sr.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qs.muxihuayi.cn

[S57] C++：编译期常量
来源：http://ss.nicolike.cn

constexpr int N = 10;
来源：http://cj.bjjhwx.cn

[S58] C++：命名空间
来源：http://qg.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://pc.szsharing.cn

[S59] C++：静态断言
来源：http://bb.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tn.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://tq.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ph.shxzukj.cn

================================================================================
来源：http://mx.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hy.huixinmuqiang.cn

================================================================================
来源：http://gn.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://mh.huixiangedu.cn

println("Hello")
来源：http://yd.szxytkj.cn

[T02] Kotlin：变量
来源：http://vq.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ys.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://cm.huixiangedu.cn

"值: $b"
来源：http://sk.szxytkj.cn

[T04] Kotlin：空安全
来源：http://ws.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://kg.colortex.cn

[T05] Kotlin：when 表达式
来源：http://zd.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qi.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://dp.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zl.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://wt.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tm.panjiajie.cn

[T08] Kotlin：数据类
来源：http://kx.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://mo.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://eb.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://yt.nszjky.cn

[T10] Kotlin：默认参数
来源：http://xe.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fs.gzmigu.cn

[T11] Kotlin：协程
来源：http://pe.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vk.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://uc.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://ru.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://gx.newstarts.cn

val m = mapOf("a" to 1)
来源：http://hj.jctech888.com.cn

[T14] Kotlin：循环
来源：http://ea.521024.cn

for (i in 1..10) println(i)
来源：http://zj.jctech888.com.cn

[T15] Kotlin：接口
来源：http://df.szsharing.cn

interface Shape { fun area(): Double }
来源：http://pw.hahajie.cn

[T16] Swift：Hello World
来源：http://cx.haigaiapp.cn

print("Hello")
来源：http://ip.shxzskj.cn

[T17] Swift：变量与常量
来源：http://aj.shxzskj.cn

var a = 1;  let b = 2
来源：http://cw.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://tq.huanxung.cn

"值: \(b)"
来源：http://in.szxytkj.cn

[T19] Swift：可选绑定
来源：http://fz.nicolike.cn

if let n = opt { print(n) }
来源：http://jr.haigaiapp.cn

[T20] Swift：数组操作
来源：http://kr.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oz.nszjky.cn

[T21] Swift：遍历
来源：http://fp.panjiajie.cn

for x in a { print(x) }
来源：http://lc.huixinmuqiang.cn

[T22] Swift：字典
来源：http://co.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nx.huixiangedu.cn

[T23] Swift：函数
来源：http://tc.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yx.hahajie.cn

[T24] Swift：闭包
来源：http://kb.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qh.huixiangedu.cn

[T25] Swift：结构体
来源：http://zx.huixiangedu.cn

struct P { var x: Int }
来源：http://db.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://co.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://ab.hahajie.cn

[T27] Swift：错误处理
来源：http://ga.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://rw.szxytkj.cn

[T28] Swift：枚举
来源：http://wp.shtwfgs.cn

enum Color { case red, green }
来源：http://po.colortex.cn

[T29] Swift：guard 提前返回
来源：http://wq.9csxet.cn

guard let x = opt else { return }
来源：http://yc.huixinmuqiang.cn

[T30] Swift：协议
来源：http://tl.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://jn.hnjuh.cn

[T31] Lua：Hello World
来源：http://fa.wgjwhj.cn

print("Hello")
来源：http://hp.newstarts.cn

[T32] Lua：局部变量
来源：http://vu.jianghongdianzi.cn

local a = 1
来源：http://lg.hahajie.cn

[T33] Lua：表（数组）
来源：http://lo.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://st.szsharing.cn

[T34] Lua：遍历表
来源：http://xc.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eh.521024.cn


<!-- 参考信息 -->