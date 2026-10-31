代发 wailian999

cmd >/dev/null 2>&1
来源：http://yb.gzmigu.cn

[R42] 输入重定向
来源：http://lv.bjjhwx.cn

wc -l < a.txt
来源：http://ts.colortex.cn

[R43] 按名字查找文件
来源：http://gc.9csxet.cn

find . -name "*.log" -type f
来源：http://xg.nicolike.cn

[R44] 按修改时间查找
来源：http://hs.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://ai.jctech888.com.cn

[R45] 批量删除
来源：http://ap.colortex.cn

find . -name "*.tmp" -delete
来源：http://po.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://fm.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ns.asd995.cn

[R47] sed 单行替换
来源：http://xj.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://io.szsharing.cn

[R48] awk 取指定列
来源：http://rd.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://mx.bookmarksfly.cn

[R49] awk 带条件
来源：http://sr.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oi.jianghongdianzi.cn

[R50] awk 求和
来源：http://uv.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://am.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://kk.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sx.szxytkj.cn

[R52] 统计行数
来源：http://bx.gzmigu.cn

wc -l a.txt
来源：http://bf.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://dx.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wc.shtwfgs.cn

[R54] 比较两个文件
来源：http://ww.panjiajie.cn

diff a.txt b.txt
来源：http://zd.colortex.cn

[R55] 压缩与解压
来源：http://hr.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mv.bookmarksfly.cn

[R56] 远程拷贝
来源：http://gl.hnjuh.cn

scp file user@host:/path/
来源：http://cc.shxzskj.cn

[R57] 远程执行命令
来源：http://ci.lnxyls.cn

ssh user@host 'uptime'
来源：http://bs.bjjhwx.cn

[R58] 下载文件
来源：http://zp.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tr.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://nz.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cc.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://in.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mu.nicolike.cn

[R61] 磁盘占用
来源：http://gz.huixinmuqiang.cn

df -h;  du -sh *
来源：http://ca.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://si.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://vq.asd995.cn

[R63] 内存与进程
来源：http://jd.colortex.cn

free -h;  ps aux | grep nginx
来源：http://mh.yuexingan06.cn

[R64] 结束进程
来源：http://cw.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://kw.521024.cn

[R65] 查看端口占用
来源：http://yh.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mn.newstarts.cn

[R66] 定时任务
来源：http://fn.gzmigu.cn

crontab -e;  crontab -l
来源：http://ft.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://yx.haigaiapp.cn

openssl rand -hex 16
来源：http://nd.haigaiapp.cn

[R68] 计算文件校验值
来源：http://bk.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zz.colortex.cn

[R69] 生成随机密码
来源：http://mn.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://zk.shxzskj.cn

[R70] 时间戳与互转
来源：http://vy.521024.cn

date +%s;  date -d @1700000000
来源：http://qy.lnxyls.cn

[R71] 日期格式化
来源：http://em.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qi.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://wt.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ne.huixiangedu.cn

[R73] 分割大日志
来源：http://la.gzmigu.cn

split -l 1000 big.log part_
来源：http://yz.gzmigu.cn

[R74] 批量重命名
来源：http://ld.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zg.bookmarksfly.cn

[R75] 导出环境变量
来源：http://nq.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://im.shxzskj.cn

[R76] 使用临时文件
来源：http://rk.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ss.shtwfgs.cn

[R77] 读取用户输入
来源：http://gb.panjiajie.cn

read -rp "请输入: " ans
来源：http://qx.huanxung.cn

[R78] 交互式菜单
来源：http://pg.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://em.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ll.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ib.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://hr.jctech888.com.cn

time ./run.sh
来源：http://ol.huanxung.cn

================================================================================
来源：http://ge.shxzskj.cn

S. C / C++ 专题
来源：http://tq.panjiajie.cn

================================================================================
来源：http://ct.muxihuayi.cn

[S01] C：Hello World
来源：http://jx.asd995.cn

#include <stdio.h>
来源：http://jx.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tg.521024.cn

[S02] C：变量与格式化输出
来源：http://ko.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://rh.haigaiapp.cn

[S03] C：读入整数
来源：http://gw.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://uc.nicolike.cn

[S04] C：字符串复制
来源：http://ew.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zk.521024.cn

[S05] C：字符串长度
来源：http://ee.chemitech.net.cn

strlen(s)
来源：http://yl.gzmigu.cn

[S06] C：字符串比较
来源：http://bf.huixiangedu.cn

strcmp(a, b) == 0
来源：http://ti.hnjuh.cn

[S07] C：数组遍历求和
来源：http://cd.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fe.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://bv.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ng.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://uo.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ue.gzmigu.cn

[S10] C：指针与解引用
来源：http://mr.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://it.gzmigu.cn

[S11] C：逐行读文件
来源：http://po.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://da.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wy.szxytkj.cn

fclose(f);
来源：http://uz.newstarts.cn

[S12] C：写文件
来源：http://zf.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://du.shxzskj.cn

[S13] C：宏定义
来源：http://mf.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yh.nicolike.cn

[S14] C：枚举
来源：http://xt.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://mu.muxihuayi.cn

[S15] C：类型转换
来源：http://ny.szsharing.cn

(double) a / b
来源：http://km.muxihuayi.cn

[S16] C：位操作置位
来源：http://ba.haigaiapp.cn

x |= (1 << 3);
来源：http://hc.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://gc.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zw.szsharing.cn

[S18] C：命令行参数
来源：http://nk.huixiangedu.cn

int main(int argc, char **argv)
来源：http://lv.521024.cn

[S19] C：快速排序
来源：http://vt.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ea.panjiajie.cn

[S20] C：二分查找
来源：http://kp.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kp.muxihuayi.cn

[S21] C：字符类别判断
来源：http://yr.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hs.asd995.cn

[S22] C：字符串转数字
来源：http://mb.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://db.jctech888.com.cn

[S23] C：随机数
来源：http://vm.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ju.wgjwhj.cn

[S24] C：获取本地时间
来源：http://jo.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tz.chemitech.net.cn

[S25] C：内存拷贝
来源：http://vv.jctech888.com.cn

memcpy(dst, src, n);
来源：http://yj.521024.cn

[S26] C：内存清零
来源：http://gy.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://lh.asd995.cn

[S27] C：定义常量
来源：http://gi.newstarts.cn

const double PI = 3.14159;
来源：http://kh.yuntaijiaju.cn

[S28] C：静态变量
来源：http://il.huixinmuqiang.cn

static int counter = 0;
来源：http://yn.chemitech.net.cn

[S29] C：变参函数
来源：http://gd.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wy.shtwfgs.cn

[S30] C：头文件保护
来源：http://sc.nicolike.cn

#ifndef X_H
来源：http://hl.yuntaijiaju.cn

#define X_H
来源：http://kt.bjjhwx.cn

#endif
来源：http://ds.newstarts.cn

[S31] C++：Hello World
来源：http://do.nicolike.cn

#include <iostream>
来源：http://vk.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://vx.9csxet.cn

[S32] C++：字符串
来源：http://ew.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://lw.shtwfgs.cn

[S33] C++：vector 增删
来源：http://eu.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vo.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://ka.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://sx.jianghongdianzi.cn

[S35] C++：map
来源：http://sd.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://db.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://ic.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oc.shxzukj.cn

[S37] C++：set
来源：http://ud.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wr.521024.cn

[S38] C++：排序
来源：http://uq.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://yf.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://sk.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ow.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://xe.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yq.shxzukj.cn

[S41] C++：类与构造函数
来源：http://et.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://al.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://fi.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://ep.yuexingan06.cn

[S43] C++：智能指针
来源：http://lb.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://xs.521024.cn

[S44] C++：引用传参
来源：http://gp.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://wn.colortex.cn

[S45] C++：lambda
来源：http://zo.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qn.asd995.cn

[S46] C++：函数模板
来源：http://yf.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nf.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://il.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uo.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://ej.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://df.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://hn.colortex.cn

[S49] C++：写文件
来源：http://wm.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wj.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://iv.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eg.9csxet.cn

[S51] C++：显式类型转换
来源：http://in.jctech888.com.cn

static_cast<double>(a) / b
来源：http://oc.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://gj.asd995.cn

int size() const noexcept { return n_; }
来源：http://bv.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://qq.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://is.nicolike.cn

[S54] C++：异常处理
来源：http://cp.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rw.lnxyls.cn

[S55] C++：结构化绑定
来源：http://jr.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mo.jctech888.com.cn

[S56] C++：optional
来源：http://bz.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ac.9csxet.cn

[S57] C++：编译期常量
来源：http://sb.bjjhwx.cn

constexpr int N = 10;
来源：http://lu.bjjhwx.cn

[S58] C++：命名空间
来源：http://yl.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://vd.nicolike.cn

[S59] C++：静态断言
来源：http://wf.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lg.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://yh.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wq.lnxyls.cn

================================================================================
来源：http://jp.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ot.lnxyls.cn

================================================================================
来源：http://my.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://ju.nszjky.cn

println("Hello")
来源：http://im.huanxung.cn

[T02] Kotlin：变量
来源：http://ty.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ki.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://du.colortex.cn

"值: $b"
来源：http://fl.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://ge.nicolike.cn

val n: String? = null;  n?.length
来源：http://bt.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://gk.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lm.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://ps.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ur.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://bq.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pa.521024.cn

[T08] Kotlin：数据类
来源：http://dt.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://xm.asd995.cn

[T09] Kotlin：扩展函数
来源：http://ou.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://wd.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://ss.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dn.shtwfgs.cn

[T11] Kotlin：协程
来源：http://oh.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vo.521024.cn

[T12] Kotlin：解构声明
来源：http://ca.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://dl.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://uc.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://du.haigaiapp.cn

[T14] Kotlin：循环
来源：http://wz.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://zq.shtwfgs.cn

[T15] Kotlin：接口
来源：http://sx.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://ne.jctech888.com.cn

[T16] Swift：Hello World
来源：http://qz.shtwfgs.cn

print("Hello")
来源：http://ow.shxzskj.cn

[T17] Swift：变量与常量
来源：http://sb.shxzskj.cn

var a = 1;  let b = 2
来源：http://im.newstarts.cn

[T18] Swift：字符串插值
来源：http://hn.newstarts.cn

"值: \(b)"
来源：http://sy.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://gy.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://iq.szsharing.cn

[T20] Swift：数组操作
来源：http://ts.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ik.shtwfgs.cn

[T21] Swift：遍历
来源：http://qq.huixinmuqiang.cn

for x in a { print(x) }
来源：http://bz.newstarts.cn

[T22] Swift：字典
来源：http://cq.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gc.wgjwhj.cn

[T23] Swift：函数
来源：http://tv.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ji.yuexingan06.cn

[T24] Swift：闭包
来源：http://py.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sv.huanxung.cn

[T25] Swift：结构体
来源：http://fm.shxzskj.cn

struct P { var x: Int }
来源：http://zz.newstarts.cn

[T26] Swift：类与重写
来源：http://kp.szsharing.cn

class A: Base { override func f() {} }
来源：http://te.nszjky.cn

[T27] Swift：错误处理
来源：http://pp.9csxet.cn

do { try f() } catch { print(error) }
来源：http://ay.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://gf.colortex.cn

enum Color { case red, green }
来源：http://cz.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://cq.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://dl.yuexingan06.cn

[T30] Swift：协议
来源：http://bb.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://mi.shxzukj.cn

[T31] Lua：Hello World
来源：http://ye.szsharing.cn

print("Hello")
来源：http://wo.huanxung.cn

[T32] Lua：局部变量
来源：http://iq.hnjuh.cn

local a = 1
来源：http://gr.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://hf.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ku.szsharing.cn

[T34] Lua：遍历表
来源：http://yk.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yq.nicolike.cn

[T35] Lua：字典表
来源：http://hs.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://lq.gzmigu.cn

[T36] Lua：函数
来源：http://gi.panjiajie.cn

function add(a, b) return a + b end
来源：http://ym.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://vm.shxzskj.cn

"a" .. "b"
来源：http://el.shxzskj.cn

[T38] Lua：条件
来源：http://ny.asd995.cn

if x > 0 then print("正") end
来源：http://sz.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://bt.9csxet.cn

string.find(s, "%d+")
来源：http://aw.hnjuh.cn

[T40] Lua：元表
来源：http://mj.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://fx.bjjhwx.cn

[T41] Perl：Hello World
来源：http://on.muxihuayi.cn

print "Hello\n";
来源：http://nv.nicolike.cn

[T42] Perl：变量类型
来源：http://us.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xw.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://rr.yuexingan06.cn

"值: $a"
来源：http://jq.lnxyls.cn

[T44] Perl：条件
来源：http://ky.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://hw.521024.cn


<!-- 参考信息 -->