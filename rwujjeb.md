代发 wailian999

find . -name "*.log" -type f
来源：http://fc.asd995.cn

[R44] 按修改时间查找
来源：http://ow.chemitech.net.cn

find . -mtime -7 -type f
来源：http://zt.gzmigu.cn

[R45] 批量删除
来源：http://lh.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://cs.panjiajie.cn

[R46] 递归替换文件内容
来源：http://oz.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sm.panjiajie.cn

[R47] sed 单行替换
来源：http://bu.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dg.nicolike.cn

[R48] awk 取指定列
来源：http://ar.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://bf.nszjky.cn

[R49] awk 带条件
来源：http://nt.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pf.huixiangedu.cn

[R50] awk 求和
来源：http://yp.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vc.shxzskj.cn

[R51] 排序去重取前几
来源：http://yh.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://og.521024.cn

[R52] 统计行数
来源：http://zj.shxzskj.cn

wc -l a.txt
来源：http://kj.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://rl.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dj.hahajie.cn

[R54] 比较两个文件
来源：http://uq.hnjuh.cn

diff a.txt b.txt
来源：http://rg.colortex.cn

[R55] 压缩与解压
来源：http://dd.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xd.shtwfgs.cn

[R56] 远程拷贝
来源：http://zo.shtwfgs.cn

scp file user@host:/path/
来源：http://bv.wgjwhj.cn

[R57] 远程执行命令
来源：http://pn.newstarts.cn

ssh user@host 'uptime'
来源：http://or.szxytkj.cn

[R58] 下载文件
来源：http://qn.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gf.newstarts.cn

[R59] 发 POST JSON
来源：http://xp.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ka.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://cz.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mm.asd995.cn

[R61] 磁盘占用
来源：http://ku.jctech888.com.cn

df -h;  du -sh *
来源：http://zq.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://rk.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://sp.szxytkj.cn

[R63] 内存与进程
来源：http://nf.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://dp.hnjuh.cn

[R64] 结束进程
来源：http://xk.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://kt.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://dg.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jh.hahajie.cn

[R66] 定时任务
来源：http://cc.huanxung.cn

crontab -e;  crontab -l
来源：http://fm.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://ay.huixinmuqiang.cn

openssl rand -hex 16
来源：http://oy.szsharing.cn

[R68] 计算文件校验值
来源：http://oh.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pa.shtwfgs.cn

[R69] 生成随机密码
来源：http://kx.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://ut.colortex.cn

[R70] 时间戳与互转
来源：http://xx.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://rf.shxzskj.cn

[R71] 日期格式化
来源：http://ir.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ks.shxzukj.cn

[R72] 等待端口就绪
来源：http://qr.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kz.asd995.cn

[R73] 分割大日志
来源：http://gg.newstarts.cn

split -l 1000 big.log part_
来源：http://mi.nicolike.cn

[R74] 批量重命名
来源：http://gd.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dw.szsharing.cn

[R75] 导出环境变量
来源：http://wh.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://yq.521024.cn

[R76] 使用临时文件
来源：http://xq.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yn.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://uj.hahajie.cn

read -rp "请输入: " ans
来源：http://he.huixiangedu.cn

[R78] 交互式菜单
来源：http://ev.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rq.panjiajie.cn

[R79] 解析命令行选项
来源：http://cl.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://al.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://fd.bookmarksfly.cn

time ./run.sh
来源：http://gt.shtwfgs.cn

================================================================================
来源：http://wy.muxihuayi.cn

S. C / C++ 专题
来源：http://ov.chemitech.net.cn

================================================================================
来源：http://wh.chemitech.net.cn

[S01] C：Hello World
来源：http://jk.521024.cn

#include <stdio.h>
来源：http://nw.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sa.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://ya.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://dw.lnxyls.cn

[S03] C：读入整数
来源：http://zo.colortex.cn

int x; scanf("%d", &x);
来源：http://hw.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://dd.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kl.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ys.bookmarksfly.cn

strlen(s)
来源：http://gm.lnxyls.cn

[S06] C：字符串比较
来源：http://eu.hnjuh.cn

strcmp(a, b) == 0
来源：http://mi.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://ou.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uq.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://wj.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qi.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://cn.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xa.haigaiapp.cn

[S10] C：指针与解引用
来源：http://mm.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://up.shtwfgs.cn

[S11] C：逐行读文件
来源：http://km.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://tw.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zb.yuntaijiaju.cn

fclose(f);
来源：http://to.huixinmuqiang.cn

[S12] C：写文件
来源：http://lf.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oz.szsharing.cn

[S13] C：宏定义
来源：http://rx.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xn.chemitech.net.cn

[S14] C：枚举
来源：http://gl.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://cc.panjiajie.cn

[S15] C：类型转换
来源：http://bu.chemitech.net.cn

(double) a / b
来源：http://xx.haigaiapp.cn

[S16] C：位操作置位
来源：http://si.szsharing.cn

x |= (1 << 3);
来源：http://ar.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://yg.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ud.huixiangedu.cn

[S18] C：命令行参数
来源：http://zd.newstarts.cn

int main(int argc, char **argv)
来源：http://mt.jianghongdianzi.cn

[S19] C：快速排序
来源：http://wu.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xp.shtwfgs.cn

[S20] C：二分查找
来源：http://bl.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ue.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://gk.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ro.nszjky.cn

[S22] C：字符串转数字
来源：http://fm.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ma.huixinmuqiang.cn

[S23] C：随机数
来源：http://ja.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gp.muxihuayi.cn

[S24] C：获取本地时间
来源：http://jl.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qf.nszjky.cn

[S25] C：内存拷贝
来源：http://ip.wgjwhj.cn

memcpy(dst, src, n);
来源：http://sy.lnxyls.cn

[S26] C：内存清零
来源：http://ht.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://fd.bjjhwx.cn

[S27] C：定义常量
来源：http://hr.bookmarksfly.cn

const double PI = 3.14159;
来源：http://eo.shxzskj.cn

[S28] C：静态变量
来源：http://qq.huixinmuqiang.cn

static int counter = 0;
来源：http://ck.hnjuh.cn

[S29] C：变参函数
来源：http://gz.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ry.huixiangedu.cn

[S30] C：头文件保护
来源：http://mu.yuntaijiaju.cn

#ifndef X_H
来源：http://gs.newstarts.cn

#define X_H
来源：http://qz.muxihuayi.cn

#endif
来源：http://ac.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://yn.bjjhwx.cn

#include <iostream>
来源：http://wh.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://cu.yuntaijiaju.cn

[S32] C++：字符串
来源：http://zk.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://zs.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ch.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ru.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://zf.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://oi.9csxet.cn

[S35] C++：map
来源：http://jd.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://up.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://ez.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pc.bookmarksfly.cn

[S37] C++：set
来源：http://ne.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bv.huixiangedu.cn

[S38] C++：排序
来源：http://lf.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://se.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://ah.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xc.panjiajie.cn

[S40] C++：查找元素
来源：http://pk.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sa.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://ts.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rh.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://im.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://dp.gzmigu.cn

[S43] C++：智能指针
来源：http://wy.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://yj.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://al.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://hg.hahajie.cn

[S45] C++：lambda
来源：http://co.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://up.9csxet.cn

[S46] C++：函数模板
来源：http://fo.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ud.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://av.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bu.521024.cn

[S48] C++：逐行读文件
来源：http://nz.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ud.newstarts.cn

while (std::getline(in, line)) { }
来源：http://qs.nicolike.cn

[S49] C++：写文件
来源：http://yc.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://et.shtwfgs.cn

[S50] C++：格式化数字
来源：http://il.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cw.szsharing.cn

[S51] C++：显式类型转换
来源：http://ds.hahajie.cn

static_cast<double>(a) / b
来源：http://ig.asd995.cn

[S52] C++：const 与 noexcept
来源：http://gc.asd995.cn

int size() const noexcept { return n_; }
来源：http://wh.bjjhwx.cn

[S53] C++：移动语义
来源：http://fw.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://om.shtwfgs.cn

[S54] C++：异常处理
来源：http://px.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jl.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://yo.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qo.hahajie.cn

[S56] C++：optional
来源：http://gg.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ri.gzmigu.cn

[S57] C++：编译期常量
来源：http://ag.newstarts.cn

constexpr int N = 10;
来源：http://qd.huixiangedu.cn

[S58] C++：命名空间
来源：http://bk.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://ti.wgjwhj.cn

[S59] C++：静态断言
来源：http://uv.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ja.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://ok.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wd.asd995.cn

================================================================================
来源：http://op.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ce.9csxet.cn

================================================================================
来源：http://yu.9csxet.cn

[T01] Kotlin：Hello World
来源：http://za.newstarts.cn

println("Hello")
来源：http://uh.asd995.cn

[T02] Kotlin：变量
来源：http://fn.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ld.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://yd.newstarts.cn

"值: $b"
来源：http://bc.nszjky.cn

[T04] Kotlin：空安全
来源：http://sd.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://kj.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://xi.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dc.9csxet.cn

[T06] Kotlin：集合映射
来源：http://lj.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lm.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://wn.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yy.9csxet.cn

[T08] Kotlin：数据类
来源：http://xz.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://zv.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://np.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://ty.asd995.cn

[T10] Kotlin：默认参数
来源：http://xv.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lq.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://yo.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cd.nicolike.cn

[T12] Kotlin：解构声明
来源：http://sg.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://fm.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://aa.asd995.cn

val m = mapOf("a" to 1)
来源：http://yp.chemitech.net.cn

[T14] Kotlin：循环
来源：http://xa.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://tj.huanxung.cn

[T15] Kotlin：接口
来源：http://kl.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://ry.huanxung.cn

[T16] Swift：Hello World
来源：http://wo.521024.cn

print("Hello")
来源：http://ed.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://fr.haigaiapp.cn

var a = 1;  let b = 2
来源：http://bn.hnjuh.cn

[T18] Swift：字符串插值
来源：http://uh.newstarts.cn

"值: \(b)"
来源：http://wt.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://yq.chemitech.net.cn

if let n = opt { print(n) }
来源：http://ev.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://bc.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ug.nicolike.cn

[T21] Swift：遍历
来源：http://un.yuexingan06.cn

for x in a { print(x) }
来源：http://ix.bjjhwx.cn

[T22] Swift：字典
来源：http://be.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vx.jctech888.com.cn

[T23] Swift：函数
来源：http://iy.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ir.9csxet.cn

[T24] Swift：闭包
来源：http://oy.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sp.bjjhwx.cn

[T25] Swift：结构体
来源：http://sp.9csxet.cn

struct P { var x: Int }
来源：http://ad.asd995.cn

[T26] Swift：类与重写
来源：http://kr.nszjky.cn

class A: Base { override func f() {} }
来源：http://ho.asd995.cn

[T27] Swift：错误处理
来源：http://cb.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://dr.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://gt.9csxet.cn

enum Color { case red, green }
来源：http://qm.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://gi.yuexingan06.cn

guard let x = opt else { return }
来源：http://ur.bjjhwx.cn

[T30] Swift：协议
来源：http://xq.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://jx.newstarts.cn

[T31] Lua：Hello World
来源：http://zi.jctech888.com.cn

print("Hello")
来源：http://tt.colortex.cn

[T32] Lua：局部变量
来源：http://pf.nicolike.cn

local a = 1
来源：http://fg.huanxung.cn

[T33] Lua：表（数组）
来源：http://pq.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zj.wgjwhj.cn

[T34] Lua：遍历表
来源：http://ql.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pq.nicolike.cn

[T35] Lua：字典表
来源：http://vb.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://bc.chemitech.net.cn

[T36] Lua：函数
来源：http://lk.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://ik.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://jz.colortex.cn

"a" .. "b"
来源：http://ni.jctech888.com.cn

[T38] Lua：条件
来源：http://ei.muxihuayi.cn

if x > 0 then print("正") end
来源：http://kb.shxzskj.cn

[T39] Lua：模式匹配
来源：http://kn.newstarts.cn

string.find(s, "%d+")
来源：http://xe.wgjwhj.cn

[T40] Lua：元表
来源：http://ri.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://dt.nszjky.cn

[T41] Perl：Hello World
来源：http://bf.nszjky.cn

print "Hello\n";
来源：http://ls.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://uu.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ll.panjiajie.cn

[T43] Perl：字符串插值
来源：http://mv.muxihuayi.cn

"值: $a"
来源：http://hf.wgjwhj.cn

[T44] Perl：条件
来源：http://uj.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://mc.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://pc.asd995.cn

for my $x (@arr) { print $x; }
来源：http://bv.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://dc.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://db.colortex.cn


<!-- 参考信息 -->