代发 wailian999

cmd >/dev/null 2>&1
来源：http://kt.huixinmuqiang.cn

[R42] 输入重定向
来源：http://ap.shxzskj.cn

wc -l < a.txt
来源：http://wc.szsharing.cn

[R43] 按名字查找文件
来源：http://ae.szsharing.cn

find . -name "*.log" -type f
来源：http://ht.colortex.cn

[R44] 按修改时间查找
来源：http://fx.shxzskj.cn

find . -mtime -7 -type f
来源：http://ou.panjiajie.cn

[R45] 批量删除
来源：http://uj.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://ap.lnxyls.cn

[R46] 递归替换文件内容
来源：http://ef.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ma.muxihuayi.cn

[R47] sed 单行替换
来源：http://av.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dm.chemitech.net.cn

[R48] awk 取指定列
来源：http://go.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://zu.gzmigu.cn

[R49] awk 带条件
来源：http://qq.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pa.shtwfgs.cn

[R50] awk 求和
来源：http://ef.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rp.colortex.cn

[R51] 排序去重取前几
来源：http://id.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tb.nicolike.cn

[R52] 统计行数
来源：http://us.521024.cn

wc -l a.txt
来源：http://pa.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://vo.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://so.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://mg.jianghongdianzi.cn

diff a.txt b.txt
来源：http://ck.szsharing.cn

[R55] 压缩与解压
来源：http://oh.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hb.wgjwhj.cn

[R56] 远程拷贝
来源：http://ug.newstarts.cn

scp file user@host:/path/
来源：http://ix.lnxyls.cn

[R57] 远程执行命令
来源：http://jk.jctech888.com.cn

ssh user@host 'uptime'
来源：http://yq.hnjuh.cn

[R58] 下载文件
来源：http://fc.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bg.nszjky.cn

[R59] 发 POST JSON
来源：http://oc.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ub.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://tq.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dj.newstarts.cn

[R61] 磁盘占用
来源：http://yt.shxzukj.cn

df -h;  du -sh *
来源：http://lc.panjiajie.cn

[R62] 找最占空间的文件
来源：http://sn.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://oo.lnxyls.cn

[R63] 内存与进程
来源：http://vl.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://kg.yuexingan06.cn

[R64] 结束进程
来源：http://wf.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://ep.shxzukj.cn

[R65] 查看端口占用
来源：http://xx.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://co.bookmarksfly.cn

[R66] 定时任务
来源：http://jd.newstarts.cn

crontab -e;  crontab -l
来源：http://cx.huanxung.cn

[R67] 生成随机十六进制串
来源：http://ci.huixinmuqiang.cn

openssl rand -hex 16
来源：http://uc.shtwfgs.cn

[R68] 计算文件校验值
来源：http://ft.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kx.bjjhwx.cn

[R69] 生成随机密码
来源：http://ni.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://wl.lnxyls.cn

[R70] 时间戳与互转
来源：http://tv.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://md.yuntaijiaju.cn

[R71] 日期格式化
来源：http://bk.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uq.yuexingan06.cn

[R72] 等待端口就绪
来源：http://dv.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oh.jianghongdianzi.cn

[R73] 分割大日志
来源：http://gc.nicolike.cn

split -l 1000 big.log part_
来源：http://zz.szxytkj.cn

[R74] 批量重命名
来源：http://zu.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pr.asd995.cn

[R75] 导出环境变量
来源：http://mo.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://xv.hnjuh.cn

[R76] 使用临时文件
来源：http://qs.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bi.asd995.cn

[R77] 读取用户输入
来源：http://gx.9csxet.cn

read -rp "请输入: " ans
来源：http://lh.newstarts.cn

[R78] 交互式菜单
来源：http://ff.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lv.nszjky.cn

[R79] 解析命令行选项
来源：http://ph.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dr.colortex.cn

[R80] 查看脚本执行耗时
来源：http://wb.wgjwhj.cn

time ./run.sh
来源：http://cq.haigaiapp.cn

================================================================================
来源：http://pv.huixiangedu.cn

S. C / C++ 专题
来源：http://rl.hahajie.cn

================================================================================
来源：http://wk.nszjky.cn

[S01] C：Hello World
来源：http://fl.shxzukj.cn

#include <stdio.h>
来源：http://vu.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pw.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://ll.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://zs.yuexingan06.cn

[S03] C：读入整数
来源：http://sn.nicolike.cn

int x; scanf("%d", &x);
来源：http://mn.bookmarksfly.cn

[S04] C：字符串复制
来源：http://zi.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fp.wgjwhj.cn

[S05] C：字符串长度
来源：http://kl.shxzskj.cn

strlen(s)
来源：http://dk.asd995.cn

[S06] C：字符串比较
来源：http://hf.muxihuayi.cn

strcmp(a, b) == 0
来源：http://ym.szxytkj.cn

[S07] C：数组遍历求和
来源：http://yk.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bd.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://gq.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xf.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://hd.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lo.lnxyls.cn

[S10] C：指针与解引用
来源：http://nl.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://rh.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://ov.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://dl.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lt.huixinmuqiang.cn

fclose(f);
来源：http://lk.huanxung.cn

[S12] C：写文件
来源：http://xl.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zq.newstarts.cn

[S13] C：宏定义
来源：http://rp.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kj.nicolike.cn

[S14] C：枚举
来源：http://ub.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://qz.shxzukj.cn

[S15] C：类型转换
来源：http://uc.shxzskj.cn

(double) a / b
来源：http://ep.bookmarksfly.cn

[S16] C：位操作置位
来源：http://zq.yuexingan06.cn

x |= (1 << 3);
来源：http://yf.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://qu.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ed.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://gz.yuexingan06.cn

int main(int argc, char **argv)
来源：http://ti.colortex.cn

[S19] C：快速排序
来源：http://us.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sv.bookmarksfly.cn

[S20] C：二分查找
来源：http://kf.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vw.huanxung.cn

[S21] C：字符类别判断
来源：http://vk.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nz.nicolike.cn

[S22] C：字符串转数字
来源：http://uk.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ae.colortex.cn

[S23] C：随机数
来源：http://ec.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vr.shxzukj.cn

[S24] C：获取本地时间
来源：http://sz.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ye.wgjwhj.cn

[S25] C：内存拷贝
来源：http://ex.szxytkj.cn

memcpy(dst, src, n);
来源：http://bf.shtwfgs.cn

[S26] C：内存清零
来源：http://px.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://ve.asd995.cn

[S27] C：定义常量
来源：http://oi.hnjuh.cn

const double PI = 3.14159;
来源：http://vg.wgjwhj.cn

[S28] C：静态变量
来源：http://gj.shtwfgs.cn

static int counter = 0;
来源：http://qs.haigaiapp.cn

[S29] C：变参函数
来源：http://it.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uk.wgjwhj.cn

[S30] C：头文件保护
来源：http://cv.newstarts.cn

#ifndef X_H
来源：http://mu.chemitech.net.cn

#define X_H
来源：http://ms.jctech888.com.cn

#endif
来源：http://yv.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://ae.hahajie.cn

#include <iostream>
来源：http://ch.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://xu.huixinmuqiang.cn

[S32] C++：字符串
来源：http://ux.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://kk.yuexingan06.cn

[S33] C++：vector 增删
来源：http://xk.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hq.9csxet.cn

[S34] C++：遍历 vector
来源：http://sp.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://jh.szxytkj.cn

[S35] C++：map
来源：http://fj.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vc.wgjwhj.cn

[S36] C++：unordered_map
来源：http://pj.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nl.lnxyls.cn

[S37] C++：set
来源：http://pw.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vi.lnxyls.cn

[S38] C++：排序
来源：http://cl.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://my.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://gv.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tf.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://nk.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://di.panjiajie.cn

[S41] C++：类与构造函数
来源：http://to.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ig.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://fp.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://ot.szsharing.cn

[S43] C++：智能指针
来源：http://wo.521024.cn

auto p = std::make_unique<int>(5);
来源：http://dj.szsharing.cn

[S44] C++：引用传参
来源：http://bi.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://re.bookmarksfly.cn

[S45] C++：lambda
来源：http://wp.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dn.hahajie.cn

[S46] C++：函数模板
来源：http://si.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fo.521024.cn

[S47] C++：结构化绑定遍历
来源：http://vb.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yq.hahajie.cn

[S48] C++：逐行读文件
来源：http://ek.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fb.hahajie.cn

while (std::getline(in, line)) { }
来源：http://av.wgjwhj.cn

[S49] C++：写文件
来源：http://wk.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dk.huixiangedu.cn

[S50] C++：格式化数字
来源：http://xn.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qe.hnjuh.cn

[S51] C++：显式类型转换
来源：http://uu.shxzukj.cn

static_cast<double>(a) / b
来源：http://rm.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://fb.huanxung.cn

int size() const noexcept { return n_; }
来源：http://gp.521024.cn

[S53] C++：移动语义
来源：http://jh.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://bo.yuexingan06.cn

[S54] C++：异常处理
来源：http://bf.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lx.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://kl.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yt.colortex.cn

[S56] C++：optional
来源：http://ni.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rq.huixiangedu.cn

[S57] C++：编译期常量
来源：http://nm.jctech888.com.cn

constexpr int N = 10;
来源：http://zc.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://ps.521024.cn

namespace ns { int f() { return 1; } }
来源：http://km.szxytkj.cn

[S59] C++：静态断言
来源：http://zg.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lu.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://eq.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ca.huixiangedu.cn

================================================================================
来源：http://az.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bn.chemitech.net.cn

================================================================================
来源：http://pa.asd995.cn

[T01] Kotlin：Hello World
来源：http://qu.huixinmuqiang.cn

println("Hello")
来源：http://fm.gzmigu.cn

[T02] Kotlin：变量
来源：http://ri.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://un.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://hq.colortex.cn

"值: $b"
来源：http://pj.panjiajie.cn

[T04] Kotlin：空安全
来源：http://wc.9csxet.cn

val n: String? = null;  n?.length
来源：http://ka.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://up.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fg.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://zk.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ug.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://nn.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qe.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://qe.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://fp.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://jf.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://ss.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://am.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dp.muxihuayi.cn

[T11] Kotlin：协程
来源：http://wa.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kz.521024.cn

[T12] Kotlin：解构声明
来源：http://zy.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://wd.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://ze.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://ku.nicolike.cn

[T14] Kotlin：循环
来源：http://ab.lnxyls.cn

for (i in 1..10) println(i)
来源：http://yr.huixiangedu.cn

[T15] Kotlin：接口
来源：http://cb.521024.cn

interface Shape { fun area(): Double }
来源：http://be.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://kk.szxytkj.cn

print("Hello")
来源：http://sa.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://kp.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://ow.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://qh.nicolike.cn

"值: \(b)"
来源：http://mt.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://im.9csxet.cn

if let n = opt { print(n) }
来源：http://il.gzmigu.cn

[T20] Swift：数组操作
来源：http://bk.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nb.chemitech.net.cn

[T21] Swift：遍历
来源：http://fj.gzmigu.cn

for x in a { print(x) }
来源：http://zh.wgjwhj.cn

[T22] Swift：字典
来源：http://vu.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wz.chemitech.net.cn

[T23] Swift：函数
来源：http://kq.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jz.huixiangedu.cn

[T24] Swift：闭包
来源：http://za.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hm.szsharing.cn

[T25] Swift：结构体
来源：http://sc.nicolike.cn

struct P { var x: Int }
来源：http://ln.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://ku.huanxung.cn

class A: Base { override func f() {} }
来源：http://ey.haigaiapp.cn

[T27] Swift：错误处理
来源：http://eg.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://ru.huixiangedu.cn

[T28] Swift：枚举
来源：http://fc.jianghongdianzi.cn

enum Color { case red, green }
来源：http://mh.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://rb.bookmarksfly.cn

guard let x = opt else { return }
来源：http://kv.huixinmuqiang.cn

[T30] Swift：协议
来源：http://vw.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://uj.lnxyls.cn

[T31] Lua：Hello World
来源：http://fa.szsharing.cn

print("Hello")
来源：http://cn.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://az.hahajie.cn

local a = 1
来源：http://qr.lnxyls.cn

[T33] Lua：表（数组）
来源：http://am.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://av.nicolike.cn

[T34] Lua：遍历表
来源：http://ks.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mj.gzmigu.cn

[T35] Lua：字典表
来源：http://dn.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://bq.panjiajie.cn

[T36] Lua：函数
来源：http://rm.yuexingan06.cn

function add(a, b) return a + b end
来源：http://sa.newstarts.cn

[T37] Lua：字符串拼接
来源：http://ot.szsharing.cn

"a" .. "b"
来源：http://vm.shtwfgs.cn

[T38] Lua：条件
来源：http://mz.gzmigu.cn

if x > 0 then print("正") end
来源：http://fe.shxzukj.cn

[T39] Lua：模式匹配
来源：http://rt.shxzskj.cn

string.find(s, "%d+")
来源：http://np.521024.cn

[T40] Lua：元表
来源：http://uu.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://rn.gzmigu.cn

[T41] Perl：Hello World
来源：http://jx.nicolike.cn

print "Hello\n";
来源：http://mb.shtwfgs.cn

[T42] Perl：变量类型
来源：http://uq.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gu.hahajie.cn

[T43] Perl：字符串插值
来源：http://ry.colortex.cn

"值: $a"
来源：http://ni.muxihuayi.cn

[T44] Perl：条件
来源：http://qn.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://zz.panjiajie.cn


<!-- 参考信息 -->