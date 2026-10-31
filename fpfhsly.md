代发 wailian999

cmd > out.log 2>&1
来源：http://vq.nszjky.cn

[R40] 追加写日志
来源：http://fy.shxzskj.cn

echo "log" >> out.log
来源：http://fg.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://bu.nicolike.cn

cmd >/dev/null 2>&1
来源：http://qo.newstarts.cn

[R42] 输入重定向
来源：http://lf.colortex.cn

wc -l < a.txt
来源：http://rh.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://jp.wgjwhj.cn

find . -name "*.log" -type f
来源：http://bd.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://rs.shxzskj.cn

find . -mtime -7 -type f
来源：http://lp.lnxyls.cn

[R45] 批量删除
来源：http://zr.szsharing.cn

find . -name "*.tmp" -delete
来源：http://mp.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://nn.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ty.shtwfgs.cn

[R47] sed 单行替换
来源：http://az.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dy.521024.cn

[R48] awk 取指定列
来源：http://tp.521024.cn

awk '{print $1, $3}' a.txt
来源：http://hu.haigaiapp.cn

[R49] awk 带条件
来源：http://fg.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ap.jctech888.com.cn

[R50] awk 求和
来源：http://el.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vg.szxytkj.cn

[R51] 排序去重取前几
来源：http://iu.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ly.9csxet.cn

[R52] 统计行数
来源：http://li.shxzskj.cn

wc -l a.txt
来源：http://te.asd995.cn

[R53] 查看文件头与实时尾
来源：http://si.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sy.nicolike.cn

[R54] 比较两个文件
来源：http://rd.szxytkj.cn

diff a.txt b.txt
来源：http://rw.nicolike.cn

[R55] 压缩与解压
来源：http://fk.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zl.huanxung.cn

[R56] 远程拷贝
来源：http://qt.jianghongdianzi.cn

scp file user@host:/path/
来源：http://sk.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://yj.bjjhwx.cn

ssh user@host 'uptime'
来源：http://ua.shxzukj.cn

[R58] 下载文件
来源：http://na.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ln.asd995.cn

[R59] 发 POST JSON
来源：http://nl.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rg.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://wt.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xs.wgjwhj.cn

[R61] 磁盘占用
来源：http://gg.newstarts.cn

df -h;  du -sh *
来源：http://ov.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://id.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://ef.huixiangedu.cn

[R63] 内存与进程
来源：http://gn.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://rp.shxzskj.cn

[R64] 结束进程
来源：http://fn.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://mv.shtwfgs.cn

[R65] 查看端口占用
来源：http://wp.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gj.shxzukj.cn

[R66] 定时任务
来源：http://kf.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://qm.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://cn.panjiajie.cn

openssl rand -hex 16
来源：http://xt.huixiangedu.cn

[R68] 计算文件校验值
来源：http://al.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xv.bookmarksfly.cn

[R69] 生成随机密码
来源：http://jy.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://uc.shxzukj.cn

[R70] 时间戳与互转
来源：http://af.nicolike.cn

date +%s;  date -d @1700000000
来源：http://bf.9csxet.cn

[R71] 日期格式化
来源：http://hx.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nq.bjjhwx.cn

[R72] 等待端口就绪
来源：http://es.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ho.hnjuh.cn

[R73] 分割大日志
来源：http://eg.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://rh.hnjuh.cn

[R74] 批量重命名
来源：http://am.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tf.bookmarksfly.cn

[R75] 导出环境变量
来源：http://fq.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://cm.colortex.cn

[R76] 使用临时文件
来源：http://km.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rg.yuexingan06.cn

[R77] 读取用户输入
来源：http://wu.szsharing.cn

read -rp "请输入: " ans
来源：http://ut.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://ds.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ew.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://pt.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ge.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://ln.huanxung.cn

time ./run.sh
来源：http://bb.hahajie.cn

================================================================================
来源：http://ba.chemitech.net.cn

S. C / C++ 专题
来源：http://mp.nicolike.cn

================================================================================
来源：http://ia.jctech888.com.cn

[S01] C：Hello World
来源：http://dm.wgjwhj.cn

#include <stdio.h>
来源：http://qn.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ut.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://tk.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://vp.hahajie.cn

[S03] C：读入整数
来源：http://vy.panjiajie.cn

int x; scanf("%d", &x);
来源：http://jg.9csxet.cn

[S04] C：字符串复制
来源：http://kq.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ek.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ug.jianghongdianzi.cn

strlen(s)
来源：http://ev.panjiajie.cn

[S06] C：字符串比较
来源：http://yn.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://kk.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://vy.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yz.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://yx.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jn.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://zb.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tu.asd995.cn

[S10] C：指针与解引用
来源：http://ss.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://dg.jctech888.com.cn

[S11] C：逐行读文件
来源：http://jj.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://gx.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mz.nicolike.cn

fclose(f);
来源：http://io.gzmigu.cn

[S12] C：写文件
来源：http://jh.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ox.muxihuayi.cn

[S13] C：宏定义
来源：http://pa.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cb.jctech888.com.cn

[S14] C：枚举
来源：http://vi.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ro.szsharing.cn

[S15] C：类型转换
来源：http://iw.lnxyls.cn

(double) a / b
来源：http://qz.shxzskj.cn

[S16] C：位操作置位
来源：http://xu.hnjuh.cn

x |= (1 << 3);
来源：http://hz.nicolike.cn

[S17] C：安全拼接字符串
来源：http://en.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nj.521024.cn

[S18] C：命令行参数
来源：http://kt.szxytkj.cn

int main(int argc, char **argv)
来源：http://ah.newstarts.cn

[S19] C：快速排序
来源：http://gj.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zk.wgjwhj.cn

[S20] C：二分查找
来源：http://df.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wk.lnxyls.cn

[S21] C：字符类别判断
来源：http://az.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jv.nicolike.cn

[S22] C：字符串转数字
来源：http://ly.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://af.9csxet.cn

[S23] C：随机数
来源：http://vv.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bm.jctech888.com.cn

[S24] C：获取本地时间
来源：http://os.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://na.colortex.cn

[S25] C：内存拷贝
来源：http://qh.yuexingan06.cn

memcpy(dst, src, n);
来源：http://ke.lnxyls.cn

[S26] C：内存清零
来源：http://ib.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://ll.hahajie.cn

[S27] C：定义常量
来源：http://rv.shtwfgs.cn

const double PI = 3.14159;
来源：http://cm.szxytkj.cn

[S28] C：静态变量
来源：http://ay.shxzukj.cn

static int counter = 0;
来源：http://oo.muxihuayi.cn

[S29] C：变参函数
来源：http://xn.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dw.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://se.huixinmuqiang.cn

#ifndef X_H
来源：http://wy.nicolike.cn

#define X_H
来源：http://ph.bjjhwx.cn

#endif
来源：http://xd.asd995.cn

[S31] C++：Hello World
来源：http://ii.bjjhwx.cn

#include <iostream>
来源：http://ns.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://bm.bjjhwx.cn

[S32] C++：字符串
来源：http://sm.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://zg.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://js.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rb.nicolike.cn

[S34] C++：遍历 vector
来源：http://gs.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://nv.jianghongdianzi.cn

[S35] C++：map
来源：http://do.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pt.jctech888.com.cn

[S36] C++：unordered_map
来源：http://ln.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cc.muxihuayi.cn

[S37] C++：set
来源：http://bv.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://su.newstarts.cn

[S38] C++：排序
来源：http://rx.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://er.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://uf.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xn.hnjuh.cn

[S40] C++：查找元素
来源：http://ye.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lo.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://mw.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pn.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://dr.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://vz.shxzukj.cn

[S43] C++：智能指针
来源：http://ct.521024.cn

auto p = std::make_unique<int>(5);
来源：http://oe.huixiangedu.cn

[S44] C++：引用传参
来源：http://yo.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://ri.szsharing.cn

[S45] C++：lambda
来源：http://fq.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ox.haigaiapp.cn

[S46] C++：函数模板
来源：http://sx.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xx.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://ft.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wn.nicolike.cn

[S48] C++：逐行读文件
来源：http://br.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pv.9csxet.cn

while (std::getline(in, line)) { }
来源：http://nh.huanxung.cn

[S49] C++：写文件
来源：http://eb.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pl.shxzskj.cn

[S50] C++：格式化数字
来源：http://jh.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oh.huanxung.cn

[S51] C++：显式类型转换
来源：http://oy.9csxet.cn

static_cast<double>(a) / b
来源：http://jh.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://qg.nszjky.cn

int size() const noexcept { return n_; }
来源：http://jw.hnjuh.cn

[S53] C++：移动语义
来源：http://jo.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://ed.nszjky.cn

[S54] C++：异常处理
来源：http://fy.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://om.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://ft.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rm.colortex.cn

[S56] C++：optional
来源：http://eb.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pb.hahajie.cn

[S57] C++：编译期常量
来源：http://oi.shxzskj.cn

constexpr int N = 10;
来源：http://zr.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://nt.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://xw.haigaiapp.cn

[S59] C++：静态断言
来源：http://pk.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lc.521024.cn

[S60] C++：遍历并删除元素
来源：http://jq.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kr.szxytkj.cn

================================================================================
来源：http://wu.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ub.wgjwhj.cn

================================================================================
来源：http://hr.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://bk.huanxung.cn

println("Hello")
来源：http://fs.hnjuh.cn

[T02] Kotlin：变量
来源：http://ki.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mb.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://uo.huixinmuqiang.cn

"值: $b"
来源：http://tc.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://pz.panjiajie.cn

val n: String? = null;  n?.length
来源：http://xf.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://dc.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rr.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://dc.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yx.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://jf.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qz.panjiajie.cn

[T08] Kotlin：数据类
来源：http://iz.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://sx.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://lg.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://mf.521024.cn

[T10] Kotlin：默认参数
来源：http://ud.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wz.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://eq.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://et.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://il.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://hf.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://bz.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ga.bjjhwx.cn

[T14] Kotlin：循环
来源：http://rw.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://pf.bjjhwx.cn

[T15] Kotlin：接口
来源：http://ng.newstarts.cn

interface Shape { fun area(): Double }
来源：http://tj.panjiajie.cn

[T16] Swift：Hello World
来源：http://yv.bookmarksfly.cn

print("Hello")
来源：http://dz.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://sb.9csxet.cn

var a = 1;  let b = 2
来源：http://xz.shxzukj.cn

[T18] Swift：字符串插值
来源：http://ua.bookmarksfly.cn

"值: \(b)"
来源：http://li.lnxyls.cn

[T19] Swift：可选绑定
来源：http://ww.haigaiapp.cn

if let n = opt { print(n) }
来源：http://gh.521024.cn

[T20] Swift：数组操作
来源：http://ua.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ah.shtwfgs.cn

[T21] Swift：遍历
来源：http://xj.9csxet.cn

for x in a { print(x) }
来源：http://hk.jctech888.com.cn

[T22] Swift：字典
来源：http://ht.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qx.jctech888.com.cn

[T23] Swift：函数
来源：http://zo.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://va.panjiajie.cn

[T24] Swift：闭包
来源：http://ae.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pn.shxzukj.cn

[T25] Swift：结构体
来源：http://ov.yuntaijiaju.cn

struct P { var x: Int }
来源：http://sb.nicolike.cn

[T26] Swift：类与重写
来源：http://pi.nszjky.cn

class A: Base { override func f() {} }
来源：http://vc.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://ma.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://hh.huixiangedu.cn

[T28] Swift：枚举
来源：http://em.panjiajie.cn

enum Color { case red, green }
来源：http://pq.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://is.newstarts.cn

guard let x = opt else { return }
来源：http://sv.lnxyls.cn

[T30] Swift：协议
来源：http://dm.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://vb.shtwfgs.cn

[T31] Lua：Hello World
来源：http://rr.bjjhwx.cn

print("Hello")
来源：http://kh.colortex.cn

[T32] Lua：局部变量
来源：http://xh.yuexingan06.cn

local a = 1
来源：http://sb.panjiajie.cn

[T33] Lua：表（数组）
来源：http://wa.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jl.muxihuayi.cn

[T34] Lua：遍历表
来源：http://mn.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ro.yuexingan06.cn

[T35] Lua：字典表
来源：http://tv.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://je.chemitech.net.cn

[T36] Lua：函数
来源：http://eo.huanxung.cn

function add(a, b) return a + b end
来源：http://iy.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://zp.wgjwhj.cn

"a" .. "b"
来源：http://mt.haigaiapp.cn

[T38] Lua：条件
来源：http://lz.nszjky.cn

if x > 0 then print("正") end
来源：http://rz.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://ff.asd995.cn

string.find(s, "%d+")
来源：http://zg.yuntaijiaju.cn

[T40] Lua：元表
来源：http://se.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://fu.nszjky.cn

[T41] Perl：Hello World
来源：http://gk.szsharing.cn

print "Hello\n";
来源：http://fl.shxzukj.cn

[T42] Perl：变量类型
来源：http://zx.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://im.9csxet.cn


<!-- 参考信息 -->