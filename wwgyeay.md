代发 wailian999

find . -name "*.log" -type f
来源：http://ea.wgjwhj.cn

[R44] 按修改时间查找
来源：http://pl.asd995.cn

find . -mtime -7 -type f
来源：http://ib.jianghongdianzi.cn

[R45] 批量删除
来源：http://hs.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://gt.huanxung.cn

[R46] 递归替换文件内容
来源：http://mu.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rp.shtwfgs.cn

[R47] sed 单行替换
来源：http://gq.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wf.panjiajie.cn

[R48] awk 取指定列
来源：http://bx.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://cl.jianghongdianzi.cn

[R49] awk 带条件
来源：http://ki.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zq.asd995.cn

[R50] awk 求和
来源：http://dh.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hh.huanxung.cn

[R51] 排序去重取前几
来源：http://wn.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cl.szsharing.cn

[R52] 统计行数
来源：http://ie.9csxet.cn

wc -l a.txt
来源：http://dx.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://bw.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vh.yuexingan06.cn

[R54] 比较两个文件
来源：http://rt.521024.cn

diff a.txt b.txt
来源：http://ai.huanxung.cn

[R55] 压缩与解压
来源：http://xb.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ft.wgjwhj.cn

[R56] 远程拷贝
来源：http://mz.wgjwhj.cn

scp file user@host:/path/
来源：http://wn.bookmarksfly.cn

[R57] 远程执行命令
来源：http://ko.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://qq.newstarts.cn

[R58] 下载文件
来源：http://vj.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ua.haigaiapp.cn

[R59] 发 POST JSON
来源：http://la.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gl.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://ux.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nv.yuexingan06.cn

[R61] 磁盘占用
来源：http://oj.szxytkj.cn

df -h;  du -sh *
来源：http://df.colortex.cn

[R62] 找最占空间的文件
来源：http://vd.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://dg.bjjhwx.cn

[R63] 内存与进程
来源：http://jd.asd995.cn

free -h;  ps aux | grep nginx
来源：http://pp.bookmarksfly.cn

[R64] 结束进程
来源：http://lp.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://mu.shxzskj.cn

[R65] 查看端口占用
来源：http://rd.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eb.bookmarksfly.cn

[R66] 定时任务
来源：http://oq.lnxyls.cn

crontab -e;  crontab -l
来源：http://zy.newstarts.cn

[R67] 生成随机十六进制串
来源：http://yf.lnxyls.cn

openssl rand -hex 16
来源：http://de.asd995.cn

[R68] 计算文件校验值
来源：http://ow.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ca.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://eg.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://yj.nicolike.cn

[R70] 时间戳与互转
来源：http://qt.nszjky.cn

date +%s;  date -d @1700000000
来源：http://ru.shxzskj.cn

[R71] 日期格式化
来源：http://vo.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wl.nszjky.cn

[R72] 等待端口就绪
来源：http://at.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rm.lnxyls.cn

[R73] 分割大日志
来源：http://iv.huixiangedu.cn

split -l 1000 big.log part_
来源：http://ej.nicolike.cn

[R74] 批量重命名
来源：http://rx.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xl.newstarts.cn

[R75] 导出环境变量
来源：http://em.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://og.gzmigu.cn

[R76] 使用临时文件
来源：http://tu.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mc.szsharing.cn

[R77] 读取用户输入
来源：http://lh.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://qs.bjjhwx.cn

[R78] 交互式菜单
来源：http://by.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://os.9csxet.cn

[R79] 解析命令行选项
来源：http://wo.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ub.asd995.cn

[R80] 查看脚本执行耗时
来源：http://wb.nicolike.cn

time ./run.sh
来源：http://jq.colortex.cn

================================================================================
来源：http://st.panjiajie.cn

S. C / C++ 专题
来源：http://bk.huanxung.cn

================================================================================
来源：http://af.nicolike.cn

[S01] C：Hello World
来源：http://yc.asd995.cn

#include <stdio.h>
来源：http://nr.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nj.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://zk.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://wx.colortex.cn

[S03] C：读入整数
来源：http://gh.hnjuh.cn

int x; scanf("%d", &x);
来源：http://rb.szsharing.cn

[S04] C：字符串复制
来源：http://je.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ko.hnjuh.cn

[S05] C：字符串长度
来源：http://jy.nszjky.cn

strlen(s)
来源：http://kw.shxzskj.cn

[S06] C：字符串比较
来源：http://pa.newstarts.cn

strcmp(a, b) == 0
来源：http://lj.asd995.cn

[S07] C：数组遍历求和
来源：http://vm.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ar.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ef.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wg.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://ma.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jm.jctech888.com.cn

[S10] C：指针与解引用
来源：http://wu.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://gw.bjjhwx.cn

[S11] C：逐行读文件
来源：http://dg.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://jo.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vl.nszjky.cn

fclose(f);
来源：http://km.muxihuayi.cn

[S12] C：写文件
来源：http://jp.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bo.huixinmuqiang.cn

[S13] C：宏定义
来源：http://is.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nz.shxzukj.cn

[S14] C：枚举
来源：http://ys.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://qo.bookmarksfly.cn

[S15] C：类型转换
来源：http://ii.shtwfgs.cn

(double) a / b
来源：http://pa.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://hq.panjiajie.cn

x |= (1 << 3);
来源：http://px.newstarts.cn

[S17] C：安全拼接字符串
来源：http://up.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ez.colortex.cn

[S18] C：命令行参数
来源：http://ep.haigaiapp.cn

int main(int argc, char **argv)
来源：http://bb.shxzukj.cn

[S19] C：快速排序
来源：http://pu.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pq.asd995.cn

[S20] C：二分查找
来源：http://gs.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://an.521024.cn

[S21] C：字符类别判断
来源：http://ns.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://th.newstarts.cn

[S22] C：字符串转数字
来源：http://aq.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://me.huixinmuqiang.cn

[S23] C：随机数
来源：http://xz.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zg.jctech888.com.cn

[S24] C：获取本地时间
来源：http://vl.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lt.szxytkj.cn

[S25] C：内存拷贝
来源：http://cj.gzmigu.cn

memcpy(dst, src, n);
来源：http://tr.lnxyls.cn

[S26] C：内存清零
来源：http://ze.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://rr.gzmigu.cn

[S27] C：定义常量
来源：http://za.lnxyls.cn

const double PI = 3.14159;
来源：http://ag.chemitech.net.cn

[S28] C：静态变量
来源：http://mc.asd995.cn

static int counter = 0;
来源：http://de.wgjwhj.cn

[S29] C：变参函数
来源：http://yk.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ad.shxzukj.cn

[S30] C：头文件保护
来源：http://jb.huixinmuqiang.cn

#ifndef X_H
来源：http://lf.521024.cn

#define X_H
来源：http://pm.panjiajie.cn

#endif
来源：http://zx.wgjwhj.cn

[S31] C++：Hello World
来源：http://ip.gzmigu.cn

#include <iostream>
来源：http://za.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://hw.chemitech.net.cn

[S32] C++：字符串
来源：http://nm.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://qj.panjiajie.cn

[S33] C++：vector 增删
来源：http://ax.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://na.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://oa.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://eb.nszjky.cn

[S35] C++：map
来源：http://da.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bm.9csxet.cn

[S36] C++：unordered_map
来源：http://pw.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://as.yuntaijiaju.cn

[S37] C++：set
来源：http://yo.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bc.huixiangedu.cn

[S38] C++：排序
来源：http://ys.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://aa.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://kh.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://os.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://pz.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ex.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://rl.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lx.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://sb.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://pf.hnjuh.cn

[S43] C++：智能指针
来源：http://kj.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://xx.huixiangedu.cn

[S44] C++：引用传参
来源：http://pv.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://uj.colortex.cn

[S45] C++：lambda
来源：http://gq.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dt.szxytkj.cn

[S46] C++：函数模板
来源：http://fu.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jl.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://uk.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xu.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://mc.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rb.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://ll.szsharing.cn

[S49] C++：写文件
来源：http://gx.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://in.muxihuayi.cn

[S50] C++：格式化数字
来源：http://rw.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://is.panjiajie.cn

[S51] C++：显式类型转换
来源：http://qy.hnjuh.cn

static_cast<double>(a) / b
来源：http://me.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://az.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://zf.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://pk.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://ik.jctech888.com.cn

[S54] C++：异常处理
来源：http://on.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ni.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://iu.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sn.haigaiapp.cn

[S56] C++：optional
来源：http://pk.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rs.wgjwhj.cn

[S57] C++：编译期常量
来源：http://vr.jctech888.com.cn

constexpr int N = 10;
来源：http://sq.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://hg.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://qx.jctech888.com.cn

[S59] C++：静态断言
来源：http://yc.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qq.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://qm.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ap.huixinmuqiang.cn

================================================================================
来源：http://qa.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nm.bookmarksfly.cn

================================================================================
来源：http://mx.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://mw.panjiajie.cn

println("Hello")
来源：http://qy.gzmigu.cn

[T02] Kotlin：变量
来源：http://nd.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dr.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://bm.nszjky.cn

"值: $b"
来源：http://po.newstarts.cn

[T04] Kotlin：空安全
来源：http://mk.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://xq.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://qp.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jc.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://wf.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xt.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://ud.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pj.shxzukj.cn

[T08] Kotlin：数据类
来源：http://kp.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://pk.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://jo.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://co.newstarts.cn

[T10] Kotlin：默认参数
来源：http://ft.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bn.9csxet.cn

[T11] Kotlin：协程
来源：http://bc.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sc.9csxet.cn

[T12] Kotlin：解构声明
来源：http://xj.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://pc.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://rn.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://ig.shtwfgs.cn

[T14] Kotlin：循环
来源：http://kt.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://dm.521024.cn

[T15] Kotlin：接口
来源：http://le.nszjky.cn

interface Shape { fun area(): Double }
来源：http://ms.shxzskj.cn

[T16] Swift：Hello World
来源：http://kx.bjjhwx.cn

print("Hello")
来源：http://yx.shxzskj.cn

[T17] Swift：变量与常量
来源：http://na.colortex.cn

var a = 1;  let b = 2
来源：http://vc.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://xf.szxytkj.cn

"值: \(b)"
来源：http://jm.panjiajie.cn

[T19] Swift：可选绑定
来源：http://qx.9csxet.cn

if let n = opt { print(n) }
来源：http://iu.lnxyls.cn

[T20] Swift：数组操作
来源：http://tz.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ny.chemitech.net.cn

[T21] Swift：遍历
来源：http://li.asd995.cn

for x in a { print(x) }
来源：http://xt.szxytkj.cn

[T22] Swift：字典
来源：http://eu.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sp.wgjwhj.cn

[T23] Swift：函数
来源：http://tq.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://es.nszjky.cn

[T24] Swift：闭包
来源：http://li.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ga.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://zx.bookmarksfly.cn

struct P { var x: Int }
来源：http://by.lnxyls.cn

[T26] Swift：类与重写
来源：http://wf.huanxung.cn

class A: Base { override func f() {} }
来源：http://ny.wgjwhj.cn

[T27] Swift：错误处理
来源：http://lb.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://vq.asd995.cn

[T28] Swift：枚举
来源：http://vi.szxytkj.cn

enum Color { case red, green }
来源：http://hb.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://gv.shxzskj.cn

guard let x = opt else { return }
来源：http://vb.nszjky.cn

[T30] Swift：协议
来源：http://mh.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://lu.gzmigu.cn

[T31] Lua：Hello World
来源：http://vd.chemitech.net.cn

print("Hello")
来源：http://or.nicolike.cn

[T32] Lua：局部变量
来源：http://by.521024.cn

local a = 1
来源：http://bv.shxzskj.cn

[T33] Lua：表（数组）
来源：http://bk.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vk.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://rs.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pi.hnjuh.cn

[T35] Lua：字典表
来源：http://he.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://ro.bookmarksfly.cn

[T36] Lua：函数
来源：http://cn.shxzskj.cn

function add(a, b) return a + b end
来源：http://hn.nicolike.cn

[T37] Lua：字符串拼接
来源：http://wn.521024.cn

"a" .. "b"
来源：http://ki.9csxet.cn

[T38] Lua：条件
来源：http://wj.nicolike.cn

if x > 0 then print("正") end
来源：http://nk.hahajie.cn

[T39] Lua：模式匹配
来源：http://nb.521024.cn

string.find(s, "%d+")
来源：http://ma.nszjky.cn

[T40] Lua：元表
来源：http://ec.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://tp.chemitech.net.cn

[T41] Perl：Hello World
来源：http://ag.shtwfgs.cn

print "Hello\n";
来源：http://jf.gzmigu.cn

[T42] Perl：变量类型
来源：http://qj.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fi.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://ht.hnjuh.cn

"值: $a"
来源：http://cx.muxihuayi.cn

[T44] Perl：条件
来源：http://gy.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://ad.lnxyls.cn

[T45] Perl：数组遍历
来源：http://cg.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://ex.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://he.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ok.shxzskj.cn


<!-- 参考信息 -->