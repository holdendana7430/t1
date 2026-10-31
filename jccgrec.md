代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yq.panjiajie.cn

[R34] 退出时清理
来源：http://gk.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rv.9csxet.cn

[R35] 后台执行并等待
来源：http://hl.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://af.panjiajie.cn

[R36] 并发执行多个任务
来源：http://ha.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fl.shxzskj.cn

[R37] 把输出赋给变量
来源：http://jk.huixinmuqiang.cn

files=$(ls -1)
来源：http://jh.521024.cn

[R38] 管道串联
来源：http://et.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://cz.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://in.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://xf.chemitech.net.cn

[R40] 追加写日志
来源：http://lu.hnjuh.cn

echo "log" >> out.log
来源：http://wd.panjiajie.cn

[R41] 丢弃输出
来源：http://zi.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://zq.shxzskj.cn

[R42] 输入重定向
来源：http://ae.newstarts.cn

wc -l < a.txt
来源：http://sm.muxihuayi.cn

[R43] 按名字查找文件
来源：http://jn.shxzukj.cn

find . -name "*.log" -type f
来源：http://yu.shtwfgs.cn

[R44] 按修改时间查找
来源：http://mj.hnjuh.cn

find . -mtime -7 -type f
来源：http://tn.bjjhwx.cn

[R45] 批量删除
来源：http://yt.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://vi.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://wr.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dm.9csxet.cn

[R47] sed 单行替换
来源：http://go.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qs.nicolike.cn

[R48] awk 取指定列
来源：http://ed.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://lv.panjiajie.cn

[R49] awk 带条件
来源：http://sk.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ao.szsharing.cn

[R50] awk 求和
来源：http://up.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oe.521024.cn

[R51] 排序去重取前几
来源：http://hl.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ca.muxihuayi.cn

[R52] 统计行数
来源：http://le.haigaiapp.cn

wc -l a.txt
来源：http://ye.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://ki.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pa.bookmarksfly.cn

[R54] 比较两个文件
来源：http://yl.szxytkj.cn

diff a.txt b.txt
来源：http://hf.yuexingan06.cn

[R55] 压缩与解压
来源：http://le.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://me.huixiangedu.cn

[R56] 远程拷贝
来源：http://yy.panjiajie.cn

scp file user@host:/path/
来源：http://ty.jctech888.com.cn

[R57] 远程执行命令
来源：http://fa.lnxyls.cn

ssh user@host 'uptime'
来源：http://dy.bookmarksfly.cn

[R58] 下载文件
来源：http://gh.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fq.nszjky.cn

[R59] 发 POST JSON
来源：http://un.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lm.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://wd.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vq.colortex.cn

[R61] 磁盘占用
来源：http://og.yuntaijiaju.cn

df -h;  du -sh *
来源：http://bi.colortex.cn

[R62] 找最占空间的文件
来源：http://kp.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://ap.szxytkj.cn

[R63] 内存与进程
来源：http://zt.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://bw.chemitech.net.cn

[R64] 结束进程
来源：http://az.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://lj.bjjhwx.cn

[R65] 查看端口占用
来源：http://il.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://in.szsharing.cn

[R66] 定时任务
来源：http://bt.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://rh.hahajie.cn

[R67] 生成随机十六进制串
来源：http://pz.yuexingan06.cn

openssl rand -hex 16
来源：http://iz.nicolike.cn

[R68] 计算文件校验值
来源：http://lr.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ls.yuexingan06.cn

[R69] 生成随机密码
来源：http://jb.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://az.haigaiapp.cn

[R70] 时间戳与互转
来源：http://ag.asd995.cn

date +%s;  date -d @1700000000
来源：http://em.colortex.cn

[R71] 日期格式化
来源：http://pz.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xl.hahajie.cn

[R72] 等待端口就绪
来源：http://ea.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uf.hnjuh.cn

[R73] 分割大日志
来源：http://rj.huixiangedu.cn

split -l 1000 big.log part_
来源：http://mg.hahajie.cn

[R74] 批量重命名
来源：http://lh.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qp.hahajie.cn

[R75] 导出环境变量
来源：http://sa.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://bw.bookmarksfly.cn

[R76] 使用临时文件
来源：http://pp.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kx.jctech888.com.cn

[R77] 读取用户输入
来源：http://ay.newstarts.cn

read -rp "请输入: " ans
来源：http://xa.shxzskj.cn

[R78] 交互式菜单
来源：http://ka.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pl.lnxyls.cn

[R79] 解析命令行选项
来源：http://rr.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sr.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://lp.nicolike.cn

time ./run.sh
来源：http://gg.huixiangedu.cn

================================================================================
来源：http://se.huixiangedu.cn

S. C / C++ 专题
来源：http://vo.panjiajie.cn

================================================================================
来源：http://tl.asd995.cn

[S01] C：Hello World
来源：http://cz.chemitech.net.cn

#include <stdio.h>
来源：http://rn.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eb.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://jk.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://ms.panjiajie.cn

[S03] C：读入整数
来源：http://uf.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://no.bjjhwx.cn

[S04] C：字符串复制
来源：http://tt.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wo.hnjuh.cn

[S05] C：字符串长度
来源：http://kd.wgjwhj.cn

strlen(s)
来源：http://fm.gzmigu.cn

[S06] C：字符串比较
来源：http://xw.shxzskj.cn

strcmp(a, b) == 0
来源：http://lg.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://wk.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kn.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://yl.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cx.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://lv.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xb.lnxyls.cn

[S10] C：指针与解引用
来源：http://gq.hahajie.cn

int *p = &a;  *p = 5;
来源：http://kc.shtwfgs.cn

[S11] C：逐行读文件
来源：http://pz.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://cc.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ze.chemitech.net.cn

fclose(f);
来源：http://ra.shxzukj.cn

[S12] C：写文件
来源：http://ye.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://an.shxzukj.cn

[S13] C：宏定义
来源：http://wz.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yr.hahajie.cn

[S14] C：枚举
来源：http://jk.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://eh.szxytkj.cn

[S15] C：类型转换
来源：http://ss.nszjky.cn

(double) a / b
来源：http://bk.muxihuayi.cn

[S16] C：位操作置位
来源：http://ua.bjjhwx.cn

x |= (1 << 3);
来源：http://sm.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://pz.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://km.szxytkj.cn

[S18] C：命令行参数
来源：http://ch.newstarts.cn

int main(int argc, char **argv)
来源：http://jo.huanxung.cn

[S19] C：快速排序
来源：http://uk.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ku.hahajie.cn

[S20] C：二分查找
来源：http://np.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dv.shxzskj.cn

[S21] C：字符类别判断
来源：http://df.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ev.yuexingan06.cn

[S22] C：字符串转数字
来源：http://vd.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hl.gzmigu.cn

[S23] C：随机数
来源：http://qh.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jy.panjiajie.cn

[S24] C：获取本地时间
来源：http://jr.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jg.muxihuayi.cn

[S25] C：内存拷贝
来源：http://yw.hnjuh.cn

memcpy(dst, src, n);
来源：http://hf.yuexingan06.cn

[S26] C：内存清零
来源：http://ri.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://of.bjjhwx.cn

[S27] C：定义常量
来源：http://ls.wgjwhj.cn

const double PI = 3.14159;
来源：http://yg.yuntaijiaju.cn

[S28] C：静态变量
来源：http://ek.bjjhwx.cn

static int counter = 0;
来源：http://ph.huanxung.cn

[S29] C：变参函数
来源：http://ax.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://an.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://em.hnjuh.cn

#ifndef X_H
来源：http://ro.521024.cn

#define X_H
来源：http://kl.yuexingan06.cn

#endif
来源：http://pt.panjiajie.cn

[S31] C++：Hello World
来源：http://hd.huanxung.cn

#include <iostream>
来源：http://lx.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://ia.shtwfgs.cn

[S32] C++：字符串
来源：http://md.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://fi.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://bv.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fp.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://sb.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://je.huixiangedu.cn

[S35] C++：map
来源：http://zt.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mq.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://mc.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://va.9csxet.cn

[S37] C++：set
来源：http://fg.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pm.bjjhwx.cn

[S38] C++：排序
来源：http://ba.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://io.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://bk.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gc.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://if.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ys.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://nd.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qj.hahajie.cn

[S42] C++：继承与虚函数
来源：http://xw.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://lt.muxihuayi.cn

[S43] C++：智能指针
来源：http://yt.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://eo.521024.cn

[S44] C++：引用传参
来源：http://kd.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://bj.huixinmuqiang.cn

[S45] C++：lambda
来源：http://nr.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dv.bjjhwx.cn

[S46] C++：函数模板
来源：http://er.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ub.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://tb.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aj.nicolike.cn

[S48] C++：逐行读文件
来源：http://ed.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yl.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://sc.9csxet.cn

[S49] C++：写文件
来源：http://jr.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rm.hnjuh.cn

[S50] C++：格式化数字
来源：http://vy.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://em.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://bk.gzmigu.cn

static_cast<double>(a) / b
来源：http://zq.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://lx.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://ac.shxzskj.cn

[S53] C++：移动语义
来源：http://jd.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://xp.yuexingan06.cn

[S54] C++：异常处理
来源：http://qb.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lp.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://xu.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://na.haigaiapp.cn

[S56] C++：optional
来源：http://td.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tu.gzmigu.cn

[S57] C++：编译期常量
来源：http://ib.szxytkj.cn

constexpr int N = 10;
来源：http://pd.muxihuayi.cn

[S58] C++：命名空间
来源：http://ck.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://co.bookmarksfly.cn

[S59] C++：静态断言
来源：http://jm.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xe.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://da.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bo.asd995.cn

================================================================================
来源：http://fl.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://df.shtwfgs.cn

================================================================================
来源：http://se.newstarts.cn

[T01] Kotlin：Hello World
来源：http://sp.hahajie.cn

println("Hello")
来源：http://gf.asd995.cn

[T02] Kotlin：变量
来源：http://mj.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vw.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://am.nszjky.cn

"值: $b"
来源：http://xx.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://xz.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://nt.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://aq.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jm.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://ag.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://js.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://vz.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zs.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://vl.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://gz.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://mt.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://ir.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://qs.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vi.szsharing.cn

[T11] Kotlin：协程
来源：http://ec.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bz.asd995.cn

[T12] Kotlin：解构声明
来源：http://ys.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://eo.colortex.cn

[T13] Kotlin：只读 Map
来源：http://xm.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://rg.jctech888.com.cn

[T14] Kotlin：循环
来源：http://kv.szxytkj.cn

for (i in 1..10) println(i)
来源：http://tq.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://un.asd995.cn

interface Shape { fun area(): Double }
来源：http://mv.huanxung.cn

[T16] Swift：Hello World
来源：http://pj.huixiangedu.cn

print("Hello")
来源：http://hr.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ei.521024.cn

var a = 1;  let b = 2
来源：http://tc.nszjky.cn

[T18] Swift：字符串插值
来源：http://hn.jctech888.com.cn

"值: \(b)"
来源：http://fv.nicolike.cn

[T19] Swift：可选绑定
来源：http://ry.colortex.cn

if let n = opt { print(n) }
来源：http://bp.asd995.cn

[T20] Swift：数组操作
来源：http://lb.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ee.szsharing.cn

[T21] Swift：遍历
来源：http://nj.wgjwhj.cn

for x in a { print(x) }
来源：http://zr.nszjky.cn

[T22] Swift：字典
来源：http://nc.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://na.9csxet.cn

[T23] Swift：函数
来源：http://ga.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://em.newstarts.cn

[T24] Swift：闭包
来源：http://rs.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sd.bjjhwx.cn

[T25] Swift：结构体
来源：http://rp.bjjhwx.cn

struct P { var x: Int }
来源：http://nv.huixiangedu.cn

[T26] Swift：类与重写
来源：http://zr.shxzskj.cn

class A: Base { override func f() {} }
来源：http://ux.yuexingan06.cn

[T27] Swift：错误处理
来源：http://ku.colortex.cn

do { try f() } catch { print(error) }
来源：http://ss.gzmigu.cn

[T28] Swift：枚举
来源：http://pq.wgjwhj.cn

enum Color { case red, green }
来源：http://pi.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://ue.gzmigu.cn

guard let x = opt else { return }
来源：http://nn.chemitech.net.cn

[T30] Swift：协议
来源：http://ou.colortex.cn

protocol Shape { func area() -> Double }
来源：http://yz.bjjhwx.cn

[T31] Lua：Hello World
来源：http://of.newstarts.cn

print("Hello")
来源：http://ut.gzmigu.cn

[T32] Lua：局部变量
来源：http://if.colortex.cn

local a = 1
来源：http://ja.hahajie.cn

[T33] Lua：表（数组）
来源：http://ik.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ro.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://vm.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://be.asd995.cn

[T35] Lua：字典表
来源：http://bn.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://um.nicolike.cn

[T36] Lua：函数
来源：http://nc.muxihuayi.cn

function add(a, b) return a + b end
来源：http://dj.wgjwhj.cn


<!-- 参考信息 -->