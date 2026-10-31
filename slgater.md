代发 wailian999

find . -name "*.tmp" -delete
来源：http://eh.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://bh.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ve.huanxung.cn

[R47] sed 单行替换
来源：http://ey.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hi.yuexingan06.cn

[R48] awk 取指定列
来源：http://fg.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://rr.szxytkj.cn

[R49] awk 带条件
来源：http://zo.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aw.asd995.cn

[R50] awk 求和
来源：http://nz.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cg.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://zo.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oz.shxzskj.cn

[R52] 统计行数
来源：http://tq.521024.cn

wc -l a.txt
来源：http://et.521024.cn

[R53] 查看文件头与实时尾
来源：http://lw.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wz.lnxyls.cn

[R54] 比较两个文件
来源：http://nb.nszjky.cn

diff a.txt b.txt
来源：http://kb.bjjhwx.cn

[R55] 压缩与解压
来源：http://kn.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://by.muxihuayi.cn

[R56] 远程拷贝
来源：http://ka.huixinmuqiang.cn

scp file user@host:/path/
来源：http://jz.shxzskj.cn

[R57] 远程执行命令
来源：http://me.shxzukj.cn

ssh user@host 'uptime'
来源：http://nk.yuntaijiaju.cn

[R58] 下载文件
来源：http://rz.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ym.hnjuh.cn

[R59] 发 POST JSON
来源：http://hv.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hy.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://zi.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rk.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://ct.jctech888.com.cn

df -h;  du -sh *
来源：http://uk.shxzukj.cn

[R62] 找最占空间的文件
来源：http://zo.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://bq.9csxet.cn

[R63] 内存与进程
来源：http://uk.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://wz.bjjhwx.cn

[R64] 结束进程
来源：http://pi.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://ac.haigaiapp.cn

[R65] 查看端口占用
来源：http://xk.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cj.colortex.cn

[R66] 定时任务
来源：http://mr.jctech888.com.cn

crontab -e;  crontab -l
来源：http://as.nszjky.cn

[R67] 生成随机十六进制串
来源：http://ui.521024.cn

openssl rand -hex 16
来源：http://qc.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://wn.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wj.colortex.cn

[R69] 生成随机密码
来源：http://xc.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://ce.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://ge.huanxung.cn

date +%s;  date -d @1700000000
来源：http://pm.nszjky.cn

[R71] 日期格式化
来源：http://xf.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bo.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://pu.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kv.bjjhwx.cn

[R73] 分割大日志
来源：http://vm.nicolike.cn

split -l 1000 big.log part_
来源：http://hb.muxihuayi.cn

[R74] 批量重命名
来源：http://ue.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xa.bjjhwx.cn

[R75] 导出环境变量
来源：http://fs.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://cl.huanxung.cn

[R76] 使用临时文件
来源：http://xo.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://si.haigaiapp.cn

[R77] 读取用户输入
来源：http://sm.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://rb.huixiangedu.cn

[R78] 交互式菜单
来源：http://tr.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://im.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://ko.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lb.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://yu.gzmigu.cn

time ./run.sh
来源：http://er.haigaiapp.cn

================================================================================
来源：http://ue.shtwfgs.cn

S. C / C++ 专题
来源：http://di.huixinmuqiang.cn

================================================================================
来源：http://lh.wgjwhj.cn

[S01] C：Hello World
来源：http://px.huixinmuqiang.cn

#include <stdio.h>
来源：http://wg.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dp.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://vw.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://st.521024.cn

[S03] C：读入整数
来源：http://bb.gzmigu.cn

int x; scanf("%d", &x);
来源：http://vc.wgjwhj.cn

[S04] C：字符串复制
来源：http://sj.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cu.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://jk.haigaiapp.cn

strlen(s)
来源：http://eg.haigaiapp.cn

[S06] C：字符串比较
来源：http://cz.shxzskj.cn

strcmp(a, b) == 0
来源：http://ia.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://wu.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rg.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://nj.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dv.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://lv.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://db.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://zg.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://sz.asd995.cn

[S11] C：逐行读文件
来源：http://ka.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://zz.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dk.szxytkj.cn

fclose(f);
来源：http://st.shxzskj.cn

[S12] C：写文件
来源：http://iz.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zp.szsharing.cn

[S13] C：宏定义
来源：http://sc.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sy.huixinmuqiang.cn

[S14] C：枚举
来源：http://za.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://im.hahajie.cn

[S15] C：类型转换
来源：http://dt.bookmarksfly.cn

(double) a / b
来源：http://bs.szsharing.cn

[S16] C：位操作置位
来源：http://tt.hahajie.cn

x |= (1 << 3);
来源：http://wr.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://co.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ou.nszjky.cn

[S18] C：命令行参数
来源：http://kk.szsharing.cn

int main(int argc, char **argv)
来源：http://qi.szxytkj.cn

[S19] C：快速排序
来源：http://lg.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vk.nicolike.cn

[S20] C：二分查找
来源：http://qy.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hx.yuexingan06.cn

[S21] C：字符类别判断
来源：http://ve.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mq.shxzukj.cn

[S22] C：字符串转数字
来源：http://xk.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xu.shtwfgs.cn

[S23] C：随机数
来源：http://cf.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fc.shtwfgs.cn

[S24] C：获取本地时间
来源：http://by.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ed.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://hf.szxytkj.cn

memcpy(dst, src, n);
来源：http://uv.asd995.cn

[S26] C：内存清零
来源：http://rt.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://gz.huanxung.cn

[S27] C：定义常量
来源：http://ne.shtwfgs.cn

const double PI = 3.14159;
来源：http://bb.colortex.cn

[S28] C：静态变量
来源：http://gb.shxzskj.cn

static int counter = 0;
来源：http://kg.chemitech.net.cn

[S29] C：变参函数
来源：http://ht.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gj.shxzukj.cn

[S30] C：头文件保护
来源：http://uv.chemitech.net.cn

#ifndef X_H
来源：http://kb.muxihuayi.cn

#define X_H
来源：http://qq.9csxet.cn

#endif
来源：http://hj.jctech888.com.cn

[S31] C++：Hello World
来源：http://dk.lnxyls.cn

#include <iostream>
来源：http://qs.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://fb.hnjuh.cn

[S32] C++：字符串
来源：http://xr.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://qi.shxzukj.cn

[S33] C++：vector 增删
来源：http://dm.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zq.lnxyls.cn

[S34] C++：遍历 vector
来源：http://vm.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://qq.521024.cn

[S35] C++：map
来源：http://be.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gs.wgjwhj.cn

[S36] C++：unordered_map
来源：http://eu.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ql.haigaiapp.cn

[S37] C++：set
来源：http://wb.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://et.nszjky.cn

[S38] C++：排序
来源：http://so.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://vg.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://cy.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bg.szsharing.cn

[S40] C++：查找元素
来源：http://zs.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hq.szsharing.cn

[S41] C++：类与构造函数
来源：http://wv.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ao.9csxet.cn

[S42] C++：继承与虚函数
来源：http://cz.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://sg.colortex.cn

[S43] C++：智能指针
来源：http://bf.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://sw.bookmarksfly.cn

[S44] C++：引用传参
来源：http://pn.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://bi.colortex.cn

[S45] C++：lambda
来源：http://fq.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cq.panjiajie.cn

[S46] C++：函数模板
来源：http://xi.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ca.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://ny.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qq.asd995.cn

[S48] C++：逐行读文件
来源：http://vv.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rj.colortex.cn

while (std::getline(in, line)) { }
来源：http://es.wgjwhj.cn

[S49] C++：写文件
来源：http://bd.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://my.wgjwhj.cn

[S50] C++：格式化数字
来源：http://jt.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vb.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://tl.szxytkj.cn

static_cast<double>(a) / b
来源：http://jf.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://hc.nicolike.cn

int size() const noexcept { return n_; }
来源：http://ux.9csxet.cn

[S53] C++：移动语义
来源：http://qv.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://uz.gzmigu.cn

[S54] C++：异常处理
来源：http://xv.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bg.9csxet.cn

[S55] C++：结构化绑定
来源：http://xy.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qk.shxzukj.cn

[S56] C++：optional
来源：http://jm.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zw.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://gt.huixiangedu.cn

constexpr int N = 10;
来源：http://tw.bjjhwx.cn

[S58] C++：命名空间
来源：http://rl.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://iq.asd995.cn

[S59] C++：静态断言
来源：http://ik.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uu.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://qp.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mq.huixiangedu.cn

================================================================================
来源：http://ww.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hm.gzmigu.cn

================================================================================
来源：http://bz.newstarts.cn

[T01] Kotlin：Hello World
来源：http://gw.wgjwhj.cn

println("Hello")
来源：http://jb.shtwfgs.cn

[T02] Kotlin：变量
来源：http://bn.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ui.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://fg.shxzukj.cn

"值: $b"
来源：http://bn.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://fy.hnjuh.cn

val n: String? = null;  n?.length
来源：http://cj.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://is.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zj.newstarts.cn

[T06] Kotlin：集合映射
来源：http://wz.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yr.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://sr.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hv.szsharing.cn

[T08] Kotlin：数据类
来源：http://ao.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://na.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://zq.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://uc.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://wz.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xp.colortex.cn

[T11] Kotlin：协程
来源：http://bf.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tk.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://wk.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://az.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://hc.szsharing.cn

val m = mapOf("a" to 1)
来源：http://sk.521024.cn

[T14] Kotlin：循环
来源：http://qp.lnxyls.cn

for (i in 1..10) println(i)
来源：http://qo.haigaiapp.cn

[T15] Kotlin：接口
来源：http://yk.colortex.cn

interface Shape { fun area(): Double }
来源：http://ea.huixiangedu.cn

[T16] Swift：Hello World
来源：http://ip.nicolike.cn

print("Hello")
来源：http://nd.shxzskj.cn

[T17] Swift：变量与常量
来源：http://wf.asd995.cn

var a = 1;  let b = 2
来源：http://ic.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://ez.shxzukj.cn

"值: \(b)"
来源：http://cd.9csxet.cn

[T19] Swift：可选绑定
来源：http://la.muxihuayi.cn

if let n = opt { print(n) }
来源：http://yh.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://wp.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://go.huixiangedu.cn

[T21] Swift：遍历
来源：http://xa.asd995.cn

for x in a { print(x) }
来源：http://yl.nicolike.cn

[T22] Swift：字典
来源：http://tb.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iy.szsharing.cn

[T23] Swift：函数
来源：http://pb.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ph.asd995.cn

[T24] Swift：闭包
来源：http://tx.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yv.chemitech.net.cn

[T25] Swift：结构体
来源：http://xs.colortex.cn

struct P { var x: Int }
来源：http://re.yuexingan06.cn

[T26] Swift：类与重写
来源：http://iu.huanxung.cn

class A: Base { override func f() {} }
来源：http://pd.huixiangedu.cn

[T27] Swift：错误处理
来源：http://cp.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://fg.huanxung.cn

[T28] Swift：枚举
来源：http://nx.huanxung.cn

enum Color { case red, green }
来源：http://pt.521024.cn

[T29] Swift：guard 提前返回
来源：http://yg.szsharing.cn

guard let x = opt else { return }
来源：http://om.bookmarksfly.cn

[T30] Swift：协议
来源：http://jm.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://ib.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://ea.jctech888.com.cn

print("Hello")
来源：http://yx.9csxet.cn

[T32] Lua：局部变量
来源：http://om.hnjuh.cn

local a = 1
来源：http://ni.panjiajie.cn

[T33] Lua：表（数组）
来源：http://pp.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pu.newstarts.cn

[T34] Lua：遍历表
来源：http://xn.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gx.shxzskj.cn

[T35] Lua：字典表
来源：http://oy.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://do.yuexingan06.cn

[T36] Lua：函数
来源：http://dk.jctech888.com.cn

function add(a, b) return a + b end
来源：http://ka.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://pv.huixinmuqiang.cn

"a" .. "b"
来源：http://gx.shxzukj.cn

[T38] Lua：条件
来源：http://vy.colortex.cn

if x > 0 then print("正") end
来源：http://ak.newstarts.cn

[T39] Lua：模式匹配
来源：http://mr.nszjky.cn

string.find(s, "%d+")
来源：http://en.yuntaijiaju.cn

[T40] Lua：元表
来源：http://wx.hahajie.cn

setmetatable({}, { __index = base })
来源：http://sz.9csxet.cn

[T41] Perl：Hello World
来源：http://eb.huanxung.cn

print "Hello\n";
来源：http://sj.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://cr.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://so.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://wh.bookmarksfly.cn

"值: $a"
来源：http://zv.yuexingan06.cn

[T44] Perl：条件
来源：http://qc.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://il.shxzskj.cn

[T45] Perl：数组遍历
来源：http://rb.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://we.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://na.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nu.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://mi.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xb.hahajie.cn

[T48] Perl：正则替换
来源：http://gw.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://jt.bookmarksfly.cn


<!-- 参考信息 -->