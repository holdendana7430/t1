代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ey.yuntaijiaju.cn

[R34] 退出时清理
来源：http://xq.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://no.huixiangedu.cn

[R35] 后台执行并等待
来源：http://re.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oi.asd995.cn

[R36] 并发执行多个任务
来源：http://lu.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hs.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://vg.yuexingan06.cn

files=$(ls -1)
来源：http://xn.521024.cn

[R38] 管道串联
来源：http://ku.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://bx.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://bo.shxzskj.cn

cmd > out.log 2>&1
来源：http://rs.szxytkj.cn

[R40] 追加写日志
来源：http://rv.jianghongdianzi.cn

echo "log" >> out.log
来源：http://zf.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://lc.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://nj.bookmarksfly.cn

[R42] 输入重定向
来源：http://ny.asd995.cn

wc -l < a.txt
来源：http://uv.shtwfgs.cn

[R43] 按名字查找文件
来源：http://ey.lnxyls.cn

find . -name "*.log" -type f
来源：http://yq.shxzukj.cn

[R44] 按修改时间查找
来源：http://bk.shtwfgs.cn

find . -mtime -7 -type f
来源：http://zz.bjjhwx.cn

[R45] 批量删除
来源：http://yt.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://sy.9csxet.cn

[R46] 递归替换文件内容
来源：http://kt.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bp.hnjuh.cn

[R47] sed 单行替换
来源：http://ue.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zo.hnjuh.cn

[R48] awk 取指定列
来源：http://hl.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://cw.jianghongdianzi.cn

[R49] awk 带条件
来源：http://qu.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uw.huanxung.cn

[R50] awk 求和
来源：http://la.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ok.asd995.cn

[R51] 排序去重取前几
来源：http://ir.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aq.bookmarksfly.cn

[R52] 统计行数
来源：http://kt.wgjwhj.cn

wc -l a.txt
来源：http://kw.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://vt.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jt.jctech888.com.cn

[R54] 比较两个文件
来源：http://ip.colortex.cn

diff a.txt b.txt
来源：http://xd.hahajie.cn

[R55] 压缩与解压
来源：http://kc.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gi.asd995.cn

[R56] 远程拷贝
来源：http://lh.shxzskj.cn

scp file user@host:/path/
来源：http://lq.muxihuayi.cn

[R57] 远程执行命令
来源：http://nk.shxzskj.cn

ssh user@host 'uptime'
来源：http://wj.jctech888.com.cn

[R58] 下载文件
来源：http://no.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wl.haigaiapp.cn

[R59] 发 POST JSON
来源：http://pz.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kq.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://yt.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yn.huanxung.cn

[R61] 磁盘占用
来源：http://od.huixiangedu.cn

df -h;  du -sh *
来源：http://mq.521024.cn

[R62] 找最占空间的文件
来源：http://dp.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://lg.jctech888.com.cn

[R63] 内存与进程
来源：http://zz.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://bx.9csxet.cn

[R64] 结束进程
来源：http://lo.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://ip.nicolike.cn

[R65] 查看端口占用
来源：http://gs.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ky.haigaiapp.cn

[R66] 定时任务
来源：http://qu.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://kd.9csxet.cn

[R67] 生成随机十六进制串
来源：http://um.huanxung.cn

openssl rand -hex 16
来源：http://xe.panjiajie.cn

[R68] 计算文件校验值
来源：http://vc.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qq.haigaiapp.cn

[R69] 生成随机密码
来源：http://zj.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://kj.newstarts.cn

[R70] 时间戳与互转
来源：http://ks.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://fd.gzmigu.cn

[R71] 日期格式化
来源：http://ag.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uj.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://vw.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ac.colortex.cn

[R73] 分割大日志
来源：http://nm.lnxyls.cn

split -l 1000 big.log part_
来源：http://jl.hahajie.cn

[R74] 批量重命名
来源：http://hf.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hx.panjiajie.cn

[R75] 导出环境变量
来源：http://zw.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://xa.9csxet.cn

[R76] 使用临时文件
来源：http://uq.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iz.9csxet.cn

[R77] 读取用户输入
来源：http://dw.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://pp.hahajie.cn

[R78] 交互式菜单
来源：http://st.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mj.szxytkj.cn

[R79] 解析命令行选项
来源：http://pt.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uf.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://zy.muxihuayi.cn

time ./run.sh
来源：http://uo.huanxung.cn

================================================================================
来源：http://oq.yuntaijiaju.cn

S. C / C++ 专题
来源：http://fs.nszjky.cn

================================================================================
来源：http://bx.hnjuh.cn

[S01] C：Hello World
来源：http://wd.shtwfgs.cn

#include <stdio.h>
来源：http://ug.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jt.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://gq.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://gw.szxytkj.cn

[S03] C：读入整数
来源：http://wx.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://gd.9csxet.cn

[S04] C：字符串复制
来源：http://qk.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ke.huanxung.cn

[S05] C：字符串长度
来源：http://lh.yuntaijiaju.cn

strlen(s)
来源：http://qa.haigaiapp.cn

[S06] C：字符串比较
来源：http://db.jctech888.com.cn

strcmp(a, b) == 0
来源：http://qf.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://ev.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vj.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://tj.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cy.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://fj.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gl.jctech888.com.cn

[S10] C：指针与解引用
来源：http://it.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://tf.shxzukj.cn

[S11] C：逐行读文件
来源：http://kp.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://dt.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qh.huanxung.cn

fclose(f);
来源：http://mi.9csxet.cn

[S12] C：写文件
来源：http://jo.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gl.szxytkj.cn

[S13] C：宏定义
来源：http://rl.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cp.muxihuayi.cn

[S14] C：枚举
来源：http://tf.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://lp.asd995.cn

[S15] C：类型转换
来源：http://li.huixiangedu.cn

(double) a / b
来源：http://eq.gzmigu.cn

[S16] C：位操作置位
来源：http://ui.bjjhwx.cn

x |= (1 << 3);
来源：http://fx.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://kz.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xd.huanxung.cn

[S18] C：命令行参数
来源：http://ke.shtwfgs.cn

int main(int argc, char **argv)
来源：http://kn.shtwfgs.cn

[S19] C：快速排序
来源：http://rl.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dr.lnxyls.cn

[S20] C：二分查找
来源：http://mo.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dx.jctech888.com.cn

[S21] C：字符类别判断
来源：http://op.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fb.lnxyls.cn

[S22] C：字符串转数字
来源：http://eh.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ae.lnxyls.cn

[S23] C：随机数
来源：http://uu.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vf.wgjwhj.cn

[S24] C：获取本地时间
来源：http://rh.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tr.nszjky.cn

[S25] C：内存拷贝
来源：http://yw.shxzukj.cn

memcpy(dst, src, n);
来源：http://gs.huixinmuqiang.cn

[S26] C：内存清零
来源：http://nn.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://kj.yuexingan06.cn

[S27] C：定义常量
来源：http://kp.521024.cn

const double PI = 3.14159;
来源：http://jz.nszjky.cn

[S28] C：静态变量
来源：http://uz.muxihuayi.cn

static int counter = 0;
来源：http://hg.bjjhwx.cn

[S29] C：变参函数
来源：http://ec.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lz.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://vd.szsharing.cn

#ifndef X_H
来源：http://of.shtwfgs.cn

#define X_H
来源：http://yb.521024.cn

#endif
来源：http://al.lnxyls.cn

[S31] C++：Hello World
来源：http://md.huixinmuqiang.cn

#include <iostream>
来源：http://wg.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://gk.huixiangedu.cn

[S32] C++：字符串
来源：http://ca.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://zd.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://bw.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://np.hnjuh.cn

[S34] C++：遍历 vector
来源：http://ru.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://lk.huixinmuqiang.cn

[S35] C++：map
来源：http://tl.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://al.hnjuh.cn

[S36] C++：unordered_map
来源：http://vk.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://db.shtwfgs.cn

[S37] C++：set
来源：http://px.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yb.hnjuh.cn

[S38] C++：排序
来源：http://fw.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://vw.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://ny.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jz.nicolike.cn

[S40] C++：查找元素
来源：http://em.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qf.nicolike.cn

[S41] C++：类与构造函数
来源：http://fd.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sy.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://os.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://az.bookmarksfly.cn

[S43] C++：智能指针
来源：http://iv.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://go.chemitech.net.cn

[S44] C++：引用传参
来源：http://ps.9csxet.cn

void inc(int &x) { ++x; }
来源：http://no.huixinmuqiang.cn

[S45] C++：lambda
来源：http://xp.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ii.hahajie.cn

[S46] C++：函数模板
来源：http://ub.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ri.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://cw.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pe.gzmigu.cn

[S48] C++：逐行读文件
来源：http://uw.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://am.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://pd.hahajie.cn

[S49] C++：写文件
来源：http://bv.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pq.nszjky.cn

[S50] C++：格式化数字
来源：http://kd.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mb.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://nq.chemitech.net.cn

static_cast<double>(a) / b
来源：http://ar.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://yh.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://ua.asd995.cn

[S53] C++：移动语义
来源：http://uh.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://nd.shxzskj.cn

[S54] C++：异常处理
来源：http://ta.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vu.lnxyls.cn

[S55] C++：结构化绑定
来源：http://cb.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://th.bookmarksfly.cn

[S56] C++：optional
来源：http://ax.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jh.hahajie.cn

[S57] C++：编译期常量
来源：http://kb.huixinmuqiang.cn

constexpr int N = 10;
来源：http://wy.asd995.cn

[S58] C++：命名空间
来源：http://ca.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://un.nicolike.cn

[S59] C++：静态断言
来源：http://ze.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://im.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://ru.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bc.9csxet.cn

================================================================================
来源：http://dr.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://no.521024.cn

================================================================================
来源：http://uu.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://dd.newstarts.cn

println("Hello")
来源：http://tw.newstarts.cn

[T02] Kotlin：变量
来源：http://iq.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ho.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://wl.chemitech.net.cn

"值: $b"
来源：http://ao.newstarts.cn

[T04] Kotlin：空安全
来源：http://ha.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://pi.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://og.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vz.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://se.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gf.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://vk.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ht.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://ra.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://bk.521024.cn

[T09] Kotlin：扩展函数
来源：http://zw.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://yr.hahajie.cn

[T10] Kotlin：默认参数
来源：http://ao.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tg.lnxyls.cn

[T11] Kotlin：协程
来源：http://ne.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://md.nicolike.cn

[T12] Kotlin：解构声明
来源：http://gw.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://li.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://hf.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://gj.shxzskj.cn

[T14] Kotlin：循环
来源：http://yi.szsharing.cn

for (i in 1..10) println(i)
来源：http://co.lnxyls.cn

[T15] Kotlin：接口
来源：http://ia.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://iw.521024.cn

[T16] Swift：Hello World
来源：http://ha.jctech888.com.cn

print("Hello")
来源：http://ik.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://rq.wgjwhj.cn

var a = 1;  let b = 2
来源：http://qt.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://ei.jianghongdianzi.cn

"值: \(b)"
来源：http://cr.hnjuh.cn

[T19] Swift：可选绑定
来源：http://yf.asd995.cn

if let n = opt { print(n) }
来源：http://oy.nicolike.cn

[T20] Swift：数组操作
来源：http://nv.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bs.lnxyls.cn

[T21] Swift：遍历
来源：http://xx.521024.cn

for x in a { print(x) }
来源：http://wp.shtwfgs.cn

[T22] Swift：字典
来源：http://bt.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fq.shtwfgs.cn

[T23] Swift：函数
来源：http://xy.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hs.haigaiapp.cn

[T24] Swift：闭包
来源：http://ks.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sc.huixiangedu.cn

[T25] Swift：结构体
来源：http://lz.bookmarksfly.cn

struct P { var x: Int }
来源：http://vi.shxzskj.cn

[T26] Swift：类与重写
来源：http://kv.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://lr.521024.cn

[T27] Swift：错误处理
来源：http://xt.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://sn.asd995.cn

[T28] Swift：枚举
来源：http://ue.521024.cn

enum Color { case red, green }
来源：http://fu.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://hk.bookmarksfly.cn

guard let x = opt else { return }
来源：http://so.bjjhwx.cn

[T30] Swift：协议
来源：http://hb.521024.cn

protocol Shape { func area() -> Double }
来源：http://yb.9csxet.cn

[T31] Lua：Hello World
来源：http://yp.colortex.cn

print("Hello")
来源：http://ml.hahajie.cn

[T32] Lua：局部变量
来源：http://rm.huixinmuqiang.cn

local a = 1
来源：http://hx.521024.cn

[T33] Lua：表（数组）
来源：http://it.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tx.shxzskj.cn

[T34] Lua：遍历表
来源：http://gu.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kl.szxytkj.cn

[T35] Lua：字典表
来源：http://xo.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://pa.panjiajie.cn

[T36] Lua：函数
来源：http://gj.newstarts.cn

function add(a, b) return a + b end
来源：http://fn.nicolike.cn


<!-- 参考信息 -->