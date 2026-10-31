代发 wailian999

cmd > out.log 2>&1
来源：http://mj.chemitech.net.cn

[R40] 追加写日志
来源：http://gv.nszjky.cn

echo "log" >> out.log
来源：http://vb.asd995.cn

[R41] 丢弃输出
来源：http://lz.szsharing.cn

cmd >/dev/null 2>&1
来源：http://dv.9csxet.cn

[R42] 输入重定向
来源：http://kb.shtwfgs.cn

wc -l < a.txt
来源：http://bt.9csxet.cn

[R43] 按名字查找文件
来源：http://cq.szsharing.cn

find . -name "*.log" -type f
来源：http://bv.shtwfgs.cn

[R44] 按修改时间查找
来源：http://wl.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://zo.nicolike.cn

[R45] 批量删除
来源：http://bg.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://jp.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://fw.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gy.szsharing.cn

[R47] sed 单行替换
来源：http://vi.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sn.nszjky.cn

[R48] awk 取指定列
来源：http://wh.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://da.shxzukj.cn

[R49] awk 带条件
来源：http://sa.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rx.jianghongdianzi.cn

[R50] awk 求和
来源：http://ly.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mx.asd995.cn

[R51] 排序去重取前几
来源：http://ud.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ng.bjjhwx.cn

[R52] 统计行数
来源：http://bg.panjiajie.cn

wc -l a.txt
来源：http://yb.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://mg.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yb.hnjuh.cn

[R54] 比较两个文件
来源：http://gt.521024.cn

diff a.txt b.txt
来源：http://sj.huanxung.cn

[R55] 压缩与解压
来源：http://tj.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mi.jctech888.com.cn

[R56] 远程拷贝
来源：http://hs.chemitech.net.cn

scp file user@host:/path/
来源：http://sg.panjiajie.cn

[R57] 远程执行命令
来源：http://jp.newstarts.cn

ssh user@host 'uptime'
来源：http://pi.szxytkj.cn

[R58] 下载文件
来源：http://be.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ce.szxytkj.cn

[R59] 发 POST JSON
来源：http://od.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xq.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://ch.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://id.szsharing.cn

[R61] 磁盘占用
来源：http://ji.panjiajie.cn

df -h;  du -sh *
来源：http://sn.huanxung.cn

[R62] 找最占空间的文件
来源：http://up.asd995.cn

du -ah . | sort -rh | head -10
来源：http://ut.lnxyls.cn

[R63] 内存与进程
来源：http://wg.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://nx.panjiajie.cn

[R64] 结束进程
来源：http://ap.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://bg.wgjwhj.cn

[R65] 查看端口占用
来源：http://fn.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://js.chemitech.net.cn

[R66] 定时任务
来源：http://mv.wgjwhj.cn

crontab -e;  crontab -l
来源：http://op.szsharing.cn

[R67] 生成随机十六进制串
来源：http://pb.shxzukj.cn

openssl rand -hex 16
来源：http://oa.bjjhwx.cn

[R68] 计算文件校验值
来源：http://gd.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dj.panjiajie.cn

[R69] 生成随机密码
来源：http://ud.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://jp.nszjky.cn

[R70] 时间戳与互转
来源：http://zy.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://ov.521024.cn

[R71] 日期格式化
来源：http://rk.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ps.muxihuayi.cn

[R72] 等待端口就绪
来源：http://af.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qb.bookmarksfly.cn

[R73] 分割大日志
来源：http://da.asd995.cn

split -l 1000 big.log part_
来源：http://px.huixinmuqiang.cn

[R74] 批量重命名
来源：http://cy.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vs.chemitech.net.cn

[R75] 导出环境变量
来源：http://go.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://eq.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://vr.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tz.haigaiapp.cn

[R77] 读取用户输入
来源：http://fy.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://af.shxzskj.cn

[R78] 交互式菜单
来源：http://ps.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qs.huixiangedu.cn

[R79] 解析命令行选项
来源：http://va.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nf.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://wi.huixinmuqiang.cn

time ./run.sh
来源：http://dx.szsharing.cn

================================================================================
来源：http://oo.nicolike.cn

S. C / C++ 专题
来源：http://ca.huixiangedu.cn

================================================================================
来源：http://ub.yuexingan06.cn

[S01] C：Hello World
来源：http://kw.bookmarksfly.cn

#include <stdio.h>
来源：http://in.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ts.nicolike.cn

[S02] C：变量与格式化输出
来源：http://hh.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://qs.shxzskj.cn

[S03] C：读入整数
来源：http://xv.huanxung.cn

int x; scanf("%d", &x);
来源：http://hz.szsharing.cn

[S04] C：字符串复制
来源：http://ng.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zp.shtwfgs.cn

[S05] C：字符串长度
来源：http://gs.huanxung.cn

strlen(s)
来源：http://jy.chemitech.net.cn

[S06] C：字符串比较
来源：http://sr.521024.cn

strcmp(a, b) == 0
来源：http://vm.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://ip.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kr.asd995.cn

[S08] C：动态内存分配与释放
来源：http://gm.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mw.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://my.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vh.asd995.cn

[S10] C：指针与解引用
来源：http://oz.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ku.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://or.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://jn.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zv.gzmigu.cn

fclose(f);
来源：http://vp.bjjhwx.cn

[S12] C：写文件
来源：http://pr.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rh.shxzskj.cn

[S13] C：宏定义
来源：http://ut.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://us.521024.cn

[S14] C：枚举
来源：http://jw.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ja.huanxung.cn

[S15] C：类型转换
来源：http://yr.lnxyls.cn

(double) a / b
来源：http://wu.lnxyls.cn

[S16] C：位操作置位
来源：http://sn.asd995.cn

x |= (1 << 3);
来源：http://es.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://er.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hy.nicolike.cn

[S18] C：命令行参数
来源：http://lp.panjiajie.cn

int main(int argc, char **argv)
来源：http://uf.9csxet.cn

[S19] C：快速排序
来源：http://ur.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yd.shtwfgs.cn

[S20] C：二分查找
来源：http://gp.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qq.huixiangedu.cn

[S21] C：字符类别判断
来源：http://ji.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mp.jctech888.com.cn

[S22] C：字符串转数字
来源：http://dk.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kq.haigaiapp.cn

[S23] C：随机数
来源：http://gc.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sk.szxytkj.cn

[S24] C：获取本地时间
来源：http://wg.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ay.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://ay.jctech888.com.cn

memcpy(dst, src, n);
来源：http://az.nicolike.cn

[S26] C：内存清零
来源：http://hr.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://rs.huixiangedu.cn

[S27] C：定义常量
来源：http://hy.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://wo.yuntaijiaju.cn

[S28] C：静态变量
来源：http://uf.shtwfgs.cn

static int counter = 0;
来源：http://rh.asd995.cn

[S29] C：变参函数
来源：http://ex.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tu.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://cn.521024.cn

#ifndef X_H
来源：http://ft.gzmigu.cn

#define X_H
来源：http://ua.colortex.cn

#endif
来源：http://li.bjjhwx.cn

[S31] C++：Hello World
来源：http://ir.yuntaijiaju.cn

#include <iostream>
来源：http://xe.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://nc.yuntaijiaju.cn

[S32] C++：字符串
来源：http://qs.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://lj.haigaiapp.cn

[S33] C++：vector 增删
来源：http://os.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kd.szxytkj.cn

[S34] C++：遍历 vector
来源：http://oe.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://iv.jctech888.com.cn

[S35] C++：map
来源：http://sv.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ld.colortex.cn

[S36] C++：unordered_map
来源：http://sv.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qs.nszjky.cn

[S37] C++：set
来源：http://de.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lt.9csxet.cn

[S38] C++：排序
来源：http://dw.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://cs.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://sx.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zx.521024.cn

[S40] C++：查找元素
来源：http://sc.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xv.nicolike.cn

[S41] C++：类与构造函数
来源：http://sh.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://um.newstarts.cn

[S42] C++：继承与虚函数
来源：http://nm.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://zu.lnxyls.cn

[S43] C++：智能指针
来源：http://gg.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://mm.521024.cn

[S44] C++：引用传参
来源：http://lg.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://hq.shtwfgs.cn

[S45] C++：lambda
来源：http://te.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://li.521024.cn

[S46] C++：函数模板
来源：http://nh.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vb.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://qe.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://br.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://ca.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pq.521024.cn

while (std::getline(in, line)) { }
来源：http://ys.huixinmuqiang.cn

[S49] C++：写文件
来源：http://do.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vy.yuexingan06.cn

[S50] C++：格式化数字
来源：http://zh.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wu.gzmigu.cn

[S51] C++：显式类型转换
来源：http://pg.nicolike.cn

static_cast<double>(a) / b
来源：http://jx.521024.cn

[S52] C++：const 与 noexcept
来源：http://mb.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://rz.szxytkj.cn

[S53] C++：移动语义
来源：http://dm.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://tq.wgjwhj.cn

[S54] C++：异常处理
来源：http://id.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bp.shxzskj.cn

[S55] C++：结构化绑定
来源：http://rs.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lh.jctech888.com.cn

[S56] C++：optional
来源：http://vx.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ul.huixiangedu.cn

[S57] C++：编译期常量
来源：http://wf.panjiajie.cn

constexpr int N = 10;
来源：http://yu.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://sx.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://dd.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://na.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kr.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://rr.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yo.newstarts.cn

================================================================================
来源：http://et.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pq.jianghongdianzi.cn

================================================================================
来源：http://tr.colortex.cn

[T01] Kotlin：Hello World
来源：http://lf.chemitech.net.cn

println("Hello")
来源：http://yp.szxytkj.cn

[T02] Kotlin：变量
来源：http://wk.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://on.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://us.colortex.cn

"值: $b"
来源：http://ym.panjiajie.cn

[T04] Kotlin：空安全
来源：http://ni.nszjky.cn

val n: String? = null;  n?.length
来源：http://kq.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://mc.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bt.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://oc.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://su.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://vu.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qm.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://ig.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://uo.colortex.cn

[T09] Kotlin：扩展函数
来源：http://pz.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://ht.szsharing.cn

[T10] Kotlin：默认参数
来源：http://rn.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pj.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://ii.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tf.521024.cn

[T12] Kotlin：解构声明
来源：http://ri.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://gr.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://nh.asd995.cn

val m = mapOf("a" to 1)
来源：http://tv.shxzskj.cn

[T14] Kotlin：循环
来源：http://mg.nszjky.cn

for (i in 1..10) println(i)
来源：http://bh.nszjky.cn

[T15] Kotlin：接口
来源：http://hu.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://dt.nicolike.cn

[T16] Swift：Hello World
来源：http://it.huanxung.cn

print("Hello")
来源：http://vc.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://pb.szxytkj.cn

var a = 1;  let b = 2
来源：http://aj.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://gv.bjjhwx.cn

"值: \(b)"
来源：http://cb.newstarts.cn

[T19] Swift：可选绑定
来源：http://hs.yuexingan06.cn

if let n = opt { print(n) }
来源：http://nm.haigaiapp.cn

[T20] Swift：数组操作
来源：http://ov.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ao.bookmarksfly.cn

[T21] Swift：遍历
来源：http://ge.muxihuayi.cn

for x in a { print(x) }
来源：http://fh.hnjuh.cn

[T22] Swift：字典
来源：http://ml.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cv.jctech888.com.cn

[T23] Swift：函数
来源：http://nu.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lo.hahajie.cn

[T24] Swift：闭包
来源：http://ht.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zw.jctech888.com.cn

[T25] Swift：结构体
来源：http://gm.shxzukj.cn

struct P { var x: Int }
来源：http://xp.jctech888.com.cn

[T26] Swift：类与重写
来源：http://nu.nszjky.cn

class A: Base { override func f() {} }
来源：http://yk.huanxung.cn

[T27] Swift：错误处理
来源：http://by.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://ah.nszjky.cn

[T28] Swift：枚举
来源：http://oy.huanxung.cn

enum Color { case red, green }
来源：http://xa.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://zl.asd995.cn

guard let x = opt else { return }
来源：http://pz.lnxyls.cn

[T30] Swift：协议
来源：http://hd.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://ed.nszjky.cn

[T31] Lua：Hello World
来源：http://ii.hnjuh.cn

print("Hello")
来源：http://lm.bjjhwx.cn

[T32] Lua：局部变量
来源：http://wu.muxihuayi.cn

local a = 1
来源：http://vi.shxzskj.cn

[T33] Lua：表（数组）
来源：http://sp.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ik.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://tj.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wh.panjiajie.cn

[T35] Lua：字典表
来源：http://ta.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://uy.newstarts.cn

[T36] Lua：函数
来源：http://hh.shxzskj.cn

function add(a, b) return a + b end
来源：http://jr.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://jd.yuntaijiaju.cn

"a" .. "b"
来源：http://pe.jctech888.com.cn

[T38] Lua：条件
来源：http://bn.shxzukj.cn

if x > 0 then print("正") end
来源：http://fi.asd995.cn

[T39] Lua：模式匹配
来源：http://tx.asd995.cn

string.find(s, "%d+")
来源：http://bb.nszjky.cn

[T40] Lua：元表
来源：http://cg.colortex.cn

setmetatable({}, { __index = base })
来源：http://np.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://iw.huixiangedu.cn

print "Hello\n";
来源：http://gh.yuexingan06.cn

[T42] Perl：变量类型
来源：http://gf.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vn.muxihuayi.cn


<!-- 参考信息 -->