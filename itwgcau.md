代发 wailian999

cmd > out.log 2>&1
来源：http://go.hnjuh.cn

[R40] 追加写日志
来源：http://ac.hahajie.cn

echo "log" >> out.log
来源：http://wv.newstarts.cn

[R41] 丢弃输出
来源：http://kh.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://ag.521024.cn

[R42] 输入重定向
来源：http://hk.yuexingan06.cn

wc -l < a.txt
来源：http://bp.panjiajie.cn

[R43] 按名字查找文件
来源：http://bi.wgjwhj.cn

find . -name "*.log" -type f
来源：http://wg.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://cv.wgjwhj.cn

find . -mtime -7 -type f
来源：http://gx.huanxung.cn

[R45] 批量删除
来源：http://bk.9csxet.cn

find . -name "*.tmp" -delete
来源：http://dl.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://mc.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vz.panjiajie.cn

[R47] sed 单行替换
来源：http://ff.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cq.shtwfgs.cn

[R48] awk 取指定列
来源：http://sh.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://pm.jctech888.com.cn

[R49] awk 带条件
来源：http://fl.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vh.huixiangedu.cn

[R50] awk 求和
来源：http://pu.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rn.gzmigu.cn

[R51] 排序去重取前几
来源：http://dl.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sv.jctech888.com.cn

[R52] 统计行数
来源：http://ou.nicolike.cn

wc -l a.txt
来源：http://hz.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://jp.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://el.asd995.cn

[R54] 比较两个文件
来源：http://am.asd995.cn

diff a.txt b.txt
来源：http://dh.jctech888.com.cn

[R55] 压缩与解压
来源：http://ah.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lc.wgjwhj.cn

[R56] 远程拷贝
来源：http://bt.nicolike.cn

scp file user@host:/path/
来源：http://gy.nicolike.cn

[R57] 远程执行命令
来源：http://iz.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://jr.huixinmuqiang.cn

[R58] 下载文件
来源：http://dj.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ab.yuexingan06.cn

[R59] 发 POST JSON
来源：http://aw.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uv.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://zu.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://df.shxzukj.cn

[R61] 磁盘占用
来源：http://to.haigaiapp.cn

df -h;  du -sh *
来源：http://pi.hahajie.cn

[R62] 找最占空间的文件
来源：http://ci.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://or.gzmigu.cn

[R63] 内存与进程
来源：http://zz.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://uv.newstarts.cn

[R64] 结束进程
来源：http://hb.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://bp.asd995.cn

[R65] 查看端口占用
来源：http://fa.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fw.bjjhwx.cn

[R66] 定时任务
来源：http://ui.haigaiapp.cn

crontab -e;  crontab -l
来源：http://tk.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://tq.hahajie.cn

openssl rand -hex 16
来源：http://uo.9csxet.cn

[R68] 计算文件校验值
来源：http://qm.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ji.yuexingan06.cn

[R69] 生成随机密码
来源：http://ib.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://lv.szsharing.cn

[R70] 时间戳与互转
来源：http://ao.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://zw.huixiangedu.cn

[R71] 日期格式化
来源：http://ay.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ul.521024.cn

[R72] 等待端口就绪
来源：http://kc.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ma.hahajie.cn

[R73] 分割大日志
来源：http://xe.nicolike.cn

split -l 1000 big.log part_
来源：http://qv.hnjuh.cn

[R74] 批量重命名
来源：http://ua.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sh.panjiajie.cn

[R75] 导出环境变量
来源：http://et.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://gf.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://ob.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fp.newstarts.cn

[R77] 读取用户输入
来源：http://fh.muxihuayi.cn

read -rp "请输入: " ans
来源：http://gj.huanxung.cn

[R78] 交互式菜单
来源：http://pc.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kp.hahajie.cn

[R79] 解析命令行选项
来源：http://ww.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fr.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://kn.9csxet.cn

time ./run.sh
来源：http://yu.9csxet.cn

================================================================================
来源：http://ha.huixiangedu.cn

S. C / C++ 专题
来源：http://cw.hnjuh.cn

================================================================================
来源：http://bg.panjiajie.cn

[S01] C：Hello World
来源：http://gg.szxytkj.cn

#include <stdio.h>
来源：http://us.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ru.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://yk.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://wm.nszjky.cn

[S03] C：读入整数
来源：http://at.asd995.cn

int x; scanf("%d", &x);
来源：http://lk.muxihuayi.cn

[S04] C：字符串复制
来源：http://ox.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://as.hahajie.cn

[S05] C：字符串长度
来源：http://kr.huixiangedu.cn

strlen(s)
来源：http://zh.colortex.cn

[S06] C：字符串比较
来源：http://mf.jctech888.com.cn

strcmp(a, b) == 0
来源：http://lj.shxzskj.cn

[S07] C：数组遍历求和
来源：http://jj.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://la.521024.cn

[S08] C：动态内存分配与释放
来源：http://rp.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cn.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://yf.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ht.nszjky.cn

[S10] C：指针与解引用
来源：http://bz.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://fg.hahajie.cn

[S11] C：逐行读文件
来源：http://pq.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://cs.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://au.nszjky.cn

fclose(f);
来源：http://xw.haigaiapp.cn

[S12] C：写文件
来源：http://wo.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gq.szxytkj.cn

[S13] C：宏定义
来源：http://zb.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rs.huanxung.cn

[S14] C：枚举
来源：http://ht.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://tb.bookmarksfly.cn

[S15] C：类型转换
来源：http://qb.bjjhwx.cn

(double) a / b
来源：http://dx.wgjwhj.cn

[S16] C：位操作置位
来源：http://fc.jctech888.com.cn

x |= (1 << 3);
来源：http://dn.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://yl.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yt.hahajie.cn

[S18] C：命令行参数
来源：http://ze.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://rm.jianghongdianzi.cn

[S19] C：快速排序
来源：http://zw.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vn.yuntaijiaju.cn

[S20] C：二分查找
来源：http://nx.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xy.nicolike.cn

[S21] C：字符类别判断
来源：http://bc.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vq.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://sc.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cu.muxihuayi.cn

[S23] C：随机数
来源：http://ry.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tj.gzmigu.cn

[S24] C：获取本地时间
来源：http://ir.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ap.shtwfgs.cn

[S25] C：内存拷贝
来源：http://bm.panjiajie.cn

memcpy(dst, src, n);
来源：http://hf.colortex.cn

[S26] C：内存清零
来源：http://mc.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://ln.jianghongdianzi.cn

[S27] C：定义常量
来源：http://yc.521024.cn

const double PI = 3.14159;
来源：http://fx.chemitech.net.cn

[S28] C：静态变量
来源：http://mt.lnxyls.cn

static int counter = 0;
来源：http://sr.szsharing.cn

[S29] C：变参函数
来源：http://kh.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cm.lnxyls.cn

[S30] C：头文件保护
来源：http://ub.haigaiapp.cn

#ifndef X_H
来源：http://lg.gzmigu.cn

#define X_H
来源：http://sc.gzmigu.cn

#endif
来源：http://od.wgjwhj.cn

[S31] C++：Hello World
来源：http://ag.shxzukj.cn

#include <iostream>
来源：http://gh.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ab.bookmarksfly.cn

[S32] C++：字符串
来源：http://xi.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://qh.colortex.cn

[S33] C++：vector 增删
来源：http://sm.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ez.shxzukj.cn

[S34] C++：遍历 vector
来源：http://ju.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://hv.muxihuayi.cn

[S35] C++：map
来源：http://kk.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qo.colortex.cn

[S36] C++：unordered_map
来源：http://jw.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://im.huixinmuqiang.cn

[S37] C++：set
来源：http://qr.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eg.newstarts.cn

[S38] C++：排序
来源：http://lu.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://rt.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://ky.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://is.szxytkj.cn

[S40] C++：查找元素
来源：http://co.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://az.huanxung.cn

[S41] C++：类与构造函数
来源：http://aj.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qc.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://mx.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://sg.shtwfgs.cn

[S43] C++：智能指针
来源：http://zn.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://bm.wgjwhj.cn

[S44] C++：引用传参
来源：http://sp.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://ju.nicolike.cn

[S45] C++：lambda
来源：http://yy.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zo.asd995.cn

[S46] C++：函数模板
来源：http://jn.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cj.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://ql.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mo.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://sd.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iq.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://bp.bjjhwx.cn

[S49] C++：写文件
来源：http://ud.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ow.jctech888.com.cn

[S50] C++：格式化数字
来源：http://lg.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://np.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://qh.haigaiapp.cn

static_cast<double>(a) / b
来源：http://ji.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://wq.asd995.cn

int size() const noexcept { return n_; }
来源：http://sj.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://fu.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://dp.nszjky.cn

[S54] C++：异常处理
来源：http://pz.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dl.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://wy.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wz.chemitech.net.cn

[S56] C++：optional
来源：http://ki.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iz.521024.cn

[S57] C++：编译期常量
来源：http://ki.newstarts.cn

constexpr int N = 10;
来源：http://li.nszjky.cn

[S58] C++：命名空间
来源：http://mr.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://rg.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://cc.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yl.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://wl.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://so.huanxung.cn

================================================================================
来源：http://ue.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ql.wgjwhj.cn

================================================================================
来源：http://qr.nicolike.cn

[T01] Kotlin：Hello World
来源：http://da.szxytkj.cn

println("Hello")
来源：http://yr.hahajie.cn

[T02] Kotlin：变量
来源：http://pk.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lc.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://vw.521024.cn

"值: $b"
来源：http://hu.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://ti.hnjuh.cn

val n: String? = null;  n?.length
来源：http://zi.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://fe.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cq.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://hv.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://on.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://vd.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://re.shxzskj.cn

[T08] Kotlin：数据类
来源：http://po.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://is.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://pa.521024.cn

fun String.exclaim() = this + "!"
来源：http://zv.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://ie.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fh.gzmigu.cn

[T11] Kotlin：协程
来源：http://tn.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gx.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://xo.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://da.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://ln.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://rz.jctech888.com.cn

[T14] Kotlin：循环
来源：http://wm.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://to.jctech888.com.cn

[T15] Kotlin：接口
来源：http://zf.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://ud.wgjwhj.cn

[T16] Swift：Hello World
来源：http://ea.newstarts.cn

print("Hello")
来源：http://gr.shxzukj.cn

[T17] Swift：变量与常量
来源：http://ey.hnjuh.cn

var a = 1;  let b = 2
来源：http://gu.shxzukj.cn

[T18] Swift：字符串插值
来源：http://rk.haigaiapp.cn

"值: \(b)"
来源：http://fv.hnjuh.cn

[T19] Swift：可选绑定
来源：http://iq.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://ih.bjjhwx.cn

[T20] Swift：数组操作
来源：http://pb.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xe.haigaiapp.cn

[T21] Swift：遍历
来源：http://rp.yuexingan06.cn

for x in a { print(x) }
来源：http://cw.colortex.cn

[T22] Swift：字典
来源：http://if.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ji.shxzukj.cn

[T23] Swift：函数
来源：http://co.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kl.bookmarksfly.cn

[T24] Swift：闭包
来源：http://zl.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wf.lnxyls.cn

[T25] Swift：结构体
来源：http://qq.hnjuh.cn

struct P { var x: Int }
来源：http://gh.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://yn.colortex.cn

class A: Base { override func f() {} }
来源：http://ly.521024.cn

[T27] Swift：错误处理
来源：http://ug.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://xq.bjjhwx.cn

[T28] Swift：枚举
来源：http://ua.shxzskj.cn

enum Color { case red, green }
来源：http://ya.colortex.cn

[T29] Swift：guard 提前返回
来源：http://pk.shtwfgs.cn

guard let x = opt else { return }
来源：http://qm.shxzskj.cn

[T30] Swift：协议
来源：http://iu.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://mf.nicolike.cn

[T31] Lua：Hello World
来源：http://dl.colortex.cn

print("Hello")
来源：http://id.wgjwhj.cn

[T32] Lua：局部变量
来源：http://fk.gzmigu.cn

local a = 1
来源：http://dt.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://mv.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sg.hnjuh.cn

[T34] Lua：遍历表
来源：http://sp.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qa.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://cu.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://cm.bjjhwx.cn

[T36] Lua：函数
来源：http://hl.newstarts.cn

function add(a, b) return a + b end
来源：http://wn.szsharing.cn

[T37] Lua：字符串拼接
来源：http://of.lnxyls.cn

"a" .. "b"
来源：http://yz.szxytkj.cn

[T38] Lua：条件
来源：http://kh.nszjky.cn

if x > 0 then print("正") end
来源：http://lg.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://dh.gzmigu.cn

string.find(s, "%d+")
来源：http://dw.hnjuh.cn

[T40] Lua：元表
来源：http://dm.huanxung.cn

setmetatable({}, { __index = base })
来源：http://tr.chemitech.net.cn

[T41] Perl：Hello World
来源：http://va.shxzskj.cn

print "Hello\n";
来源：http://zj.newstarts.cn

[T42] Perl：变量类型
来源：http://jr.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zc.huixinmuqiang.cn


<!-- 参考信息 -->