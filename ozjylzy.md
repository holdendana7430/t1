代发 wailian999

cmd >/dev/null 2>&1
来源：http://di.bjjhwx.cn

[R42] 输入重定向
来源：http://uz.haigaiapp.cn

wc -l < a.txt
来源：http://dd.huanxung.cn

[R43] 按名字查找文件
来源：http://at.huixiangedu.cn

find . -name "*.log" -type f
来源：http://jx.gzmigu.cn

[R44] 按修改时间查找
来源：http://ns.shxzukj.cn

find . -mtime -7 -type f
来源：http://qd.9csxet.cn

[R45] 批量删除
来源：http://mf.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://sy.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://tu.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uv.szsharing.cn

[R47] sed 单行替换
来源：http://br.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oo.wgjwhj.cn

[R48] awk 取指定列
来源：http://el.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://xg.bookmarksfly.cn

[R49] awk 带条件
来源：http://eh.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ha.huixiangedu.cn

[R50] awk 求和
来源：http://xj.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yc.haigaiapp.cn

[R51] 排序去重取前几
来源：http://jw.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ft.jianghongdianzi.cn

[R52] 统计行数
来源：http://tf.szxytkj.cn

wc -l a.txt
来源：http://ek.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://fw.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gi.huixiangedu.cn

[R54] 比较两个文件
来源：http://ed.nicolike.cn

diff a.txt b.txt
来源：http://rc.bookmarksfly.cn

[R55] 压缩与解压
来源：http://kz.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yt.newstarts.cn

[R56] 远程拷贝
来源：http://qf.huixiangedu.cn

scp file user@host:/path/
来源：http://fb.colortex.cn

[R57] 远程执行命令
来源：http://wr.szxytkj.cn

ssh user@host 'uptime'
来源：http://ch.hnjuh.cn

[R58] 下载文件
来源：http://qh.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yp.chemitech.net.cn

[R59] 发 POST JSON
来源：http://uy.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hi.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://lb.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cq.bookmarksfly.cn

[R61] 磁盘占用
来源：http://ny.yuexingan06.cn

df -h;  du -sh *
来源：http://pe.9csxet.cn

[R62] 找最占空间的文件
来源：http://xw.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://vr.yuntaijiaju.cn

[R63] 内存与进程
来源：http://ox.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://vz.shxzskj.cn

[R64] 结束进程
来源：http://zj.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://vk.bookmarksfly.cn

[R65] 查看端口占用
来源：http://vz.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wv.haigaiapp.cn

[R66] 定时任务
来源：http://ki.chemitech.net.cn

crontab -e;  crontab -l
来源：http://hb.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://op.chemitech.net.cn

openssl rand -hex 16
来源：http://yx.chemitech.net.cn

[R68] 计算文件校验值
来源：http://hk.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ck.asd995.cn

[R69] 生成随机密码
来源：http://gh.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://av.wgjwhj.cn

[R70] 时间戳与互转
来源：http://uy.colortex.cn

date +%s;  date -d @1700000000
来源：http://sc.newstarts.cn

[R71] 日期格式化
来源：http://wr.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ze.newstarts.cn

[R72] 等待端口就绪
来源：http://xb.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fe.lnxyls.cn

[R73] 分割大日志
来源：http://ey.hnjuh.cn

split -l 1000 big.log part_
来源：http://tp.huanxung.cn

[R74] 批量重命名
来源：http://vd.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ie.hahajie.cn

[R75] 导出环境变量
来源：http://pr.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://va.szsharing.cn

[R76] 使用临时文件
来源：http://zd.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ij.asd995.cn

[R77] 读取用户输入
来源：http://zr.haigaiapp.cn

read -rp "请输入: " ans
来源：http://ov.huixiangedu.cn

[R78] 交互式菜单
来源：http://kn.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kw.wgjwhj.cn

[R79] 解析命令行选项
来源：http://eb.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dw.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://ug.shxzskj.cn

time ./run.sh
来源：http://ui.asd995.cn

================================================================================
来源：http://xk.hnjuh.cn

S. C / C++ 专题
来源：http://jt.panjiajie.cn

================================================================================
来源：http://ls.wgjwhj.cn

[S01] C：Hello World
来源：http://cf.yuexingan06.cn

#include <stdio.h>
来源：http://wo.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ik.szsharing.cn

[S02] C：变量与格式化输出
来源：http://hb.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://sf.jianghongdianzi.cn

[S03] C：读入整数
来源：http://mo.newstarts.cn

int x; scanf("%d", &x);
来源：http://ov.szxytkj.cn

[S04] C：字符串复制
来源：http://qh.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ex.jctech888.com.cn

[S05] C：字符串长度
来源：http://bp.shxzskj.cn

strlen(s)
来源：http://ru.szsharing.cn

[S06] C：字符串比较
来源：http://uo.yuexingan06.cn

strcmp(a, b) == 0
来源：http://sl.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://if.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wl.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://gn.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nq.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://us.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pv.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://vx.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://lg.bjjhwx.cn

[S11] C：逐行读文件
来源：http://ym.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://vq.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://el.huixiangedu.cn

fclose(f);
来源：http://va.shxzukj.cn

[S12] C：写文件
来源：http://hg.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ya.haigaiapp.cn

[S13] C：宏定义
来源：http://bf.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://in.lnxyls.cn

[S14] C：枚举
来源：http://zu.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://pl.huixinmuqiang.cn

[S15] C：类型转换
来源：http://dt.huixiangedu.cn

(double) a / b
来源：http://zd.asd995.cn

[S16] C：位操作置位
来源：http://ms.szxytkj.cn

x |= (1 << 3);
来源：http://su.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://qp.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oh.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://hc.panjiajie.cn

int main(int argc, char **argv)
来源：http://uo.haigaiapp.cn

[S19] C：快速排序
来源：http://hd.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://om.huixiangedu.cn

[S20] C：二分查找
来源：http://yu.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ir.bjjhwx.cn

[S21] C：字符类别判断
来源：http://fk.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vq.gzmigu.cn

[S22] C：字符串转数字
来源：http://vb.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gk.szxytkj.cn

[S23] C：随机数
来源：http://uy.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://af.haigaiapp.cn

[S24] C：获取本地时间
来源：http://pt.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://st.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://sb.jctech888.com.cn

memcpy(dst, src, n);
来源：http://vl.haigaiapp.cn

[S26] C：内存清零
来源：http://ap.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://wq.huixinmuqiang.cn

[S27] C：定义常量
来源：http://fb.bookmarksfly.cn

const double PI = 3.14159;
来源：http://yz.szxytkj.cn

[S28] C：静态变量
来源：http://jg.hahajie.cn

static int counter = 0;
来源：http://fd.yuexingan06.cn

[S29] C：变参函数
来源：http://gs.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pq.shtwfgs.cn

[S30] C：头文件保护
来源：http://gu.shxzukj.cn

#ifndef X_H
来源：http://sr.colortex.cn

#define X_H
来源：http://ew.9csxet.cn

#endif
来源：http://nq.9csxet.cn

[S31] C++：Hello World
来源：http://bx.gzmigu.cn

#include <iostream>
来源：http://ie.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ep.nicolike.cn

[S32] C++：字符串
来源：http://ol.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://jz.nszjky.cn

[S33] C++：vector 增删
来源：http://by.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://so.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://ij.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://yt.yuntaijiaju.cn

[S35] C++：map
来源：http://bx.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ch.shxzskj.cn

[S36] C++：unordered_map
来源：http://lh.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lg.shxzukj.cn

[S37] C++：set
来源：http://uo.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://na.szxytkj.cn

[S38] C++：排序
来源：http://vc.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://hs.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://ei.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ti.nicolike.cn

[S40] C++：查找元素
来源：http://ow.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mi.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://fp.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://li.huanxung.cn

[S42] C++：继承与虚函数
来源：http://ca.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://au.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://iz.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://so.nicolike.cn

[S44] C++：引用传参
来源：http://yy.hahajie.cn

void inc(int &x) { ++x; }
来源：http://hg.shtwfgs.cn

[S45] C++：lambda
来源：http://uu.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qe.huanxung.cn

[S46] C++：函数模板
来源：http://if.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ok.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://hx.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yl.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://sk.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vt.huanxung.cn

while (std::getline(in, line)) { }
来源：http://be.shxzukj.cn

[S49] C++：写文件
来源：http://zk.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dx.shtwfgs.cn

[S50] C++：格式化数字
来源：http://gv.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yb.huanxung.cn

[S51] C++：显式类型转换
来源：http://dw.chemitech.net.cn

static_cast<double>(a) / b
来源：http://ya.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://ib.huanxung.cn

int size() const noexcept { return n_; }
来源：http://ww.colortex.cn

[S53] C++：移动语义
来源：http://eb.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://sv.521024.cn

[S54] C++：异常处理
来源：http://pc.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gj.nicolike.cn

[S55] C++：结构化绑定
来源：http://zx.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yb.haigaiapp.cn

[S56] C++：optional
来源：http://vl.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ij.newstarts.cn

[S57] C++：编译期常量
来源：http://kv.lnxyls.cn

constexpr int N = 10;
来源：http://ma.bjjhwx.cn

[S58] C++：命名空间
来源：http://il.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://tj.bookmarksfly.cn

[S59] C++：静态断言
来源：http://la.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://de.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ab.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ur.hahajie.cn

================================================================================
来源：http://pm.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jc.9csxet.cn

================================================================================
来源：http://pa.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://bu.szsharing.cn

println("Hello")
来源：http://hd.newstarts.cn

[T02] Kotlin：变量
来源：http://vq.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://as.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://ao.nicolike.cn

"值: $b"
来源：http://ug.lnxyls.cn

[T04] Kotlin：空安全
来源：http://so.hahajie.cn

val n: String? = null;  n?.length
来源：http://tu.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://nc.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xy.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://mx.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jn.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://ls.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aw.hahajie.cn

[T08] Kotlin：数据类
来源：http://xa.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://yl.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://ec.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://qj.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://vf.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gv.newstarts.cn

[T11] Kotlin：协程
来源：http://ac.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rj.9csxet.cn

[T12] Kotlin：解构声明
来源：http://vx.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://ao.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://pf.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://pt.muxihuayi.cn

[T14] Kotlin：循环
来源：http://rn.nszjky.cn

for (i in 1..10) println(i)
来源：http://wz.hnjuh.cn

[T15] Kotlin：接口
来源：http://yo.szsharing.cn

interface Shape { fun area(): Double }
来源：http://ln.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://iv.shxzukj.cn

print("Hello")
来源：http://dy.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://wg.bjjhwx.cn

var a = 1;  let b = 2
来源：http://xt.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://db.shxzskj.cn

"值: \(b)"
来源：http://et.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://ig.colortex.cn

if let n = opt { print(n) }
来源：http://oy.newstarts.cn

[T20] Swift：数组操作
来源：http://gw.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jn.jctech888.com.cn

[T21] Swift：遍历
来源：http://au.panjiajie.cn

for x in a { print(x) }
来源：http://iv.szxytkj.cn

[T22] Swift：字典
来源：http://il.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://du.jctech888.com.cn

[T23] Swift：函数
来源：http://iq.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qo.panjiajie.cn

[T24] Swift：闭包
来源：http://lv.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://su.bookmarksfly.cn

[T25] Swift：结构体
来源：http://wv.newstarts.cn

struct P { var x: Int }
来源：http://cb.szsharing.cn

[T26] Swift：类与重写
来源：http://ah.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://xl.hahajie.cn

[T27] Swift：错误处理
来源：http://pi.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://yc.jctech888.com.cn

[T28] Swift：枚举
来源：http://yv.jctech888.com.cn

enum Color { case red, green }
来源：http://jc.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://fk.hahajie.cn

guard let x = opt else { return }
来源：http://zz.shxzukj.cn

[T30] Swift：协议
来源：http://jy.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://br.szxytkj.cn

[T31] Lua：Hello World
来源：http://ik.muxihuayi.cn

print("Hello")
来源：http://pt.haigaiapp.cn

[T32] Lua：局部变量
来源：http://fn.wgjwhj.cn

local a = 1
来源：http://yk.shxzskj.cn

[T33] Lua：表（数组）
来源：http://ti.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://be.asd995.cn

[T34] Lua：遍历表
来源：http://my.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://in.wgjwhj.cn

[T35] Lua：字典表
来源：http://eq.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://nw.gzmigu.cn

[T36] Lua：函数
来源：http://ey.yuexingan06.cn

function add(a, b) return a + b end
来源：http://pu.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://mo.chemitech.net.cn

"a" .. "b"
来源：http://xp.yuexingan06.cn

[T38] Lua：条件
来源：http://tx.shxzukj.cn

if x > 0 then print("正") end
来源：http://gy.panjiajie.cn

[T39] Lua：模式匹配
来源：http://fj.chemitech.net.cn

string.find(s, "%d+")
来源：http://yj.yuntaijiaju.cn

[T40] Lua：元表
来源：http://br.9csxet.cn

setmetatable({}, { __index = base })
来源：http://ka.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://iz.chemitech.net.cn

print "Hello\n";
来源：http://yr.szsharing.cn

[T42] Perl：变量类型
来源：http://iv.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://na.colortex.cn

[T43] Perl：字符串插值
来源：http://re.chemitech.net.cn

"值: $a"
来源：http://sv.szxytkj.cn

[T44] Perl：条件
来源：http://bl.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://km.lnxyls.cn


<!-- 参考信息 -->