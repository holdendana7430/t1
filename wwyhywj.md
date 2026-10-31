代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://rp.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://ge.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://od.panjiajie.cn

[R37] 把输出赋给变量
来源：http://xp.newstarts.cn

files=$(ls -1)
来源：http://qh.jianghongdianzi.cn

[R38] 管道串联
来源：http://gu.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://dz.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://jy.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://hx.asd995.cn

[R40] 追加写日志
来源：http://bp.lnxyls.cn

echo "log" >> out.log
来源：http://sp.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://kb.nicolike.cn

cmd >/dev/null 2>&1
来源：http://ib.colortex.cn

[R42] 输入重定向
来源：http://kv.szsharing.cn

wc -l < a.txt
来源：http://yh.asd995.cn

[R43] 按名字查找文件
来源：http://qo.szsharing.cn

find . -name "*.log" -type f
来源：http://ad.asd995.cn

[R44] 按修改时间查找
来源：http://mn.asd995.cn

find . -mtime -7 -type f
来源：http://mp.panjiajie.cn

[R45] 批量删除
来源：http://mx.szsharing.cn

find . -name "*.tmp" -delete
来源：http://uj.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://ws.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://li.szsharing.cn

[R47] sed 单行替换
来源：http://dg.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jc.lnxyls.cn

[R48] awk 取指定列
来源：http://va.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://kr.muxihuayi.cn

[R49] awk 带条件
来源：http://of.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eh.yuntaijiaju.cn

[R50] awk 求和
来源：http://yn.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://co.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://vn.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ys.huanxung.cn

[R52] 统计行数
来源：http://dm.szxytkj.cn

wc -l a.txt
来源：http://fa.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://an.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ko.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://cz.asd995.cn

diff a.txt b.txt
来源：http://nd.nszjky.cn

[R55] 压缩与解压
来源：http://cx.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://os.jctech888.com.cn

[R56] 远程拷贝
来源：http://tc.jianghongdianzi.cn

scp file user@host:/path/
来源：http://ug.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://sh.muxihuayi.cn

ssh user@host 'uptime'
来源：http://pt.szsharing.cn

[R58] 下载文件
来源：http://yc.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ge.shxzukj.cn

[R59] 发 POST JSON
来源：http://ys.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pk.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://ci.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mo.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://lr.yuntaijiaju.cn

df -h;  du -sh *
来源：http://wj.huanxung.cn

[R62] 找最占空间的文件
来源：http://vj.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://aq.panjiajie.cn

[R63] 内存与进程
来源：http://pc.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://gc.bjjhwx.cn

[R64] 结束进程
来源：http://px.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://ps.9csxet.cn

[R65] 查看端口占用
来源：http://lo.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://on.huanxung.cn

[R66] 定时任务
来源：http://vz.shxzskj.cn

crontab -e;  crontab -l
来源：http://ul.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://lu.lnxyls.cn

openssl rand -hex 16
来源：http://vz.9csxet.cn

[R68] 计算文件校验值
来源：http://ja.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yw.shxzskj.cn

[R69] 生成随机密码
来源：http://re.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://rv.gzmigu.cn

[R70] 时间戳与互转
来源：http://xg.newstarts.cn

date +%s;  date -d @1700000000
来源：http://ze.gzmigu.cn

[R71] 日期格式化
来源：http://xt.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fl.9csxet.cn

[R72] 等待端口就绪
来源：http://vn.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kc.yuexingan06.cn

[R73] 分割大日志
来源：http://ol.muxihuayi.cn

split -l 1000 big.log part_
来源：http://md.jctech888.com.cn

[R74] 批量重命名
来源：http://wx.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://li.wgjwhj.cn

[R75] 导出环境变量
来源：http://pm.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://hg.haigaiapp.cn

[R76] 使用临时文件
来源：http://hl.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aa.panjiajie.cn

[R77] 读取用户输入
来源：http://xb.lnxyls.cn

read -rp "请输入: " ans
来源：http://mr.muxihuayi.cn

[R78] 交互式菜单
来源：http://qv.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iy.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://ij.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vz.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://zn.asd995.cn

time ./run.sh
来源：http://fh.jianghongdianzi.cn

================================================================================
来源：http://bo.521024.cn

S. C / C++ 专题
来源：http://st.shxzukj.cn

================================================================================
来源：http://zy.yuntaijiaju.cn

[S01] C：Hello World
来源：http://bq.huanxung.cn

#include <stdio.h>
来源：http://yf.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tl.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://yi.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://ur.521024.cn

[S03] C：读入整数
来源：http://ao.nszjky.cn

int x; scanf("%d", &x);
来源：http://up.huanxung.cn

[S04] C：字符串复制
来源：http://gs.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iy.hnjuh.cn

[S05] C：字符串长度
来源：http://gx.jctech888.com.cn

strlen(s)
来源：http://lz.shxzskj.cn

[S06] C：字符串比较
来源：http://cq.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://ou.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://tn.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nu.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://an.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://us.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://uf.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://en.lnxyls.cn

[S10] C：指针与解引用
来源：http://er.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://rd.521024.cn

[S11] C：逐行读文件
来源：http://gc.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://ds.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lb.hahajie.cn

fclose(f);
来源：http://jt.nszjky.cn

[S12] C：写文件
来源：http://mp.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mp.panjiajie.cn

[S13] C：宏定义
来源：http://ym.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rp.shxzskj.cn

[S14] C：枚举
来源：http://qy.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://pi.szsharing.cn

[S15] C：类型转换
来源：http://ie.haigaiapp.cn

(double) a / b
来源：http://rn.chemitech.net.cn

[S16] C：位操作置位
来源：http://cd.shxzukj.cn

x |= (1 << 3);
来源：http://lf.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://yt.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tc.muxihuayi.cn

[S18] C：命令行参数
来源：http://wm.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://sm.panjiajie.cn

[S19] C：快速排序
来源：http://db.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wr.chemitech.net.cn

[S20] C：二分查找
来源：http://qf.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rm.521024.cn

[S21] C：字符类别判断
来源：http://mn.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vt.muxihuayi.cn

[S22] C：字符串转数字
来源：http://su.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nq.huixinmuqiang.cn

[S23] C：随机数
来源：http://eq.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vi.huanxung.cn

[S24] C：获取本地时间
来源：http://ci.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://so.521024.cn

[S25] C：内存拷贝
来源：http://hu.huanxung.cn

memcpy(dst, src, n);
来源：http://ui.newstarts.cn

[S26] C：内存清零
来源：http://bb.huanxung.cn

memset(a, 0, sizeof a);
来源：http://bu.huixinmuqiang.cn

[S27] C：定义常量
来源：http://gb.szxytkj.cn

const double PI = 3.14159;
来源：http://iy.nicolike.cn

[S28] C：静态变量
来源：http://tf.haigaiapp.cn

static int counter = 0;
来源：http://nt.bjjhwx.cn

[S29] C：变参函数
来源：http://mw.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ru.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://dd.chemitech.net.cn

#ifndef X_H
来源：http://vo.asd995.cn

#define X_H
来源：http://tt.521024.cn

#endif
来源：http://sb.hnjuh.cn

[S31] C++：Hello World
来源：http://ys.yuexingan06.cn

#include <iostream>
来源：http://hw.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://ry.shxzukj.cn

[S32] C++：字符串
来源：http://kq.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://qx.hahajie.cn

[S33] C++：vector 增删
来源：http://gn.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sz.nicolike.cn

[S34] C++：遍历 vector
来源：http://zp.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://bz.hnjuh.cn

[S35] C++：map
来源：http://pj.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ar.bjjhwx.cn

[S36] C++：unordered_map
来源：http://wk.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lz.hnjuh.cn

[S37] C++：set
来源：http://ut.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jk.huanxung.cn

[S38] C++：排序
来源：http://pt.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://ps.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://qf.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kf.hnjuh.cn

[S40] C++：查找元素
来源：http://ye.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bk.hnjuh.cn

[S41] C++：类与构造函数
来源：http://zg.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ie.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://xp.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://gh.yuexingan06.cn

[S43] C++：智能指针
来源：http://ar.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://qy.jctech888.com.cn

[S44] C++：引用传参
来源：http://rj.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://ud.shxzskj.cn

[S45] C++：lambda
来源：http://lt.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://on.muxihuayi.cn

[S46] C++：函数模板
来源：http://ev.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wi.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://lj.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xx.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://cz.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yo.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://ne.asd995.cn

[S49] C++：写文件
来源：http://yq.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kw.hnjuh.cn

[S50] C++：格式化数字
来源：http://en.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tl.colortex.cn

[S51] C++：显式类型转换
来源：http://ry.muxihuayi.cn

static_cast<double>(a) / b
来源：http://tw.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://we.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://hf.muxihuayi.cn

[S53] C++：移动语义
来源：http://zr.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://gu.muxihuayi.cn

[S54] C++：异常处理
来源：http://vn.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oh.521024.cn

[S55] C++：结构化绑定
来源：http://ki.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ad.shxzskj.cn

[S56] C++：optional
来源：http://we.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pz.521024.cn

[S57] C++：编译期常量
来源：http://ky.gzmigu.cn

constexpr int N = 10;
来源：http://zg.newstarts.cn

[S58] C++：命名空间
来源：http://ss.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://zf.huanxung.cn

[S59] C++：静态断言
来源：http://wu.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sv.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://cq.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ws.szsharing.cn

================================================================================
来源：http://iz.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pt.chemitech.net.cn

================================================================================
来源：http://uy.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://sd.shxzukj.cn

println("Hello")
来源：http://dn.chemitech.net.cn

[T02] Kotlin：变量
来源：http://md.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jd.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://lk.gzmigu.cn

"值: $b"
来源：http://sk.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://gv.shxzskj.cn

val n: String? = null;  n?.length
来源：http://sk.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://iq.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ak.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://sv.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pp.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://wo.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qv.hnjuh.cn

[T08] Kotlin：数据类
来源：http://ws.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://uc.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://lu.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://mt.szsharing.cn

[T10] Kotlin：默认参数
来源：http://tt.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hf.nicolike.cn

[T11] Kotlin：协程
来源：http://mb.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mf.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://ta.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://sa.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://tg.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://wa.chemitech.net.cn

[T14] Kotlin：循环
来源：http://pj.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://iz.lnxyls.cn

[T15] Kotlin：接口
来源：http://yp.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://lr.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://ax.gzmigu.cn

print("Hello")
来源：http://ez.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://em.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://bd.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://dg.nicolike.cn

"值: \(b)"
来源：http://sa.gzmigu.cn

[T19] Swift：可选绑定
来源：http://li.lnxyls.cn

if let n = opt { print(n) }
来源：http://mx.shtwfgs.cn

[T20] Swift：数组操作
来源：http://wy.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://or.nicolike.cn

[T21] Swift：遍历
来源：http://bm.muxihuayi.cn

for x in a { print(x) }
来源：http://fb.chemitech.net.cn

[T22] Swift：字典
来源：http://rt.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://en.9csxet.cn

[T23] Swift：函数
来源：http://cb.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hg.haigaiapp.cn

[T24] Swift：闭包
来源：http://sk.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ug.huixiangedu.cn

[T25] Swift：结构体
来源：http://qq.shxzskj.cn

struct P { var x: Int }
来源：http://oc.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://to.shxzukj.cn

class A: Base { override func f() {} }
来源：http://zs.hahajie.cn

[T27] Swift：错误处理
来源：http://hs.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://xu.nicolike.cn

[T28] Swift：枚举
来源：http://zr.yuntaijiaju.cn

enum Color { case red, green }
来源：http://gu.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://we.yuexingan06.cn

guard let x = opt else { return }
来源：http://cr.lnxyls.cn

[T30] Swift：协议
来源：http://jy.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://kb.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://qh.huixinmuqiang.cn

print("Hello")
来源：http://ul.521024.cn

[T32] Lua：局部变量
来源：http://kb.colortex.cn

local a = 1
来源：http://ay.shxzskj.cn

[T33] Lua：表（数组）
来源：http://of.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://do.huixiangedu.cn

[T34] Lua：遍历表
来源：http://kq.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gk.nszjky.cn

[T35] Lua：字典表
来源：http://pb.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://ea.szxytkj.cn

[T36] Lua：函数
来源：http://zm.nicolike.cn

function add(a, b) return a + b end
来源：http://ro.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://rr.panjiajie.cn

"a" .. "b"
来源：http://sx.shtwfgs.cn

[T38] Lua：条件
来源：http://dj.hahajie.cn

if x > 0 then print("正") end
来源：http://xd.nszjky.cn


<!-- 参考信息 -->