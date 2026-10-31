代发 wailian999

files=$(ls -1)
来源：http://no.szxytkj.cn

[R38] 管道串联
来源：http://sh.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://wj.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://qj.nicolike.cn

cmd > out.log 2>&1
来源：http://gz.chemitech.net.cn

[R40] 追加写日志
来源：http://ws.huixiangedu.cn

echo "log" >> out.log
来源：http://mf.nszjky.cn

[R41] 丢弃输出
来源：http://dm.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://fv.szxytkj.cn

[R42] 输入重定向
来源：http://hi.szsharing.cn

wc -l < a.txt
来源：http://hw.hahajie.cn

[R43] 按名字查找文件
来源：http://at.lnxyls.cn

find . -name "*.log" -type f
来源：http://lq.lnxyls.cn

[R44] 按修改时间查找
来源：http://xn.hnjuh.cn

find . -mtime -7 -type f
来源：http://lc.huixiangedu.cn

[R45] 批量删除
来源：http://zg.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://tn.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://af.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://te.nicolike.cn

[R47] sed 单行替换
来源：http://dt.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cl.chemitech.net.cn

[R48] awk 取指定列
来源：http://he.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://sb.hahajie.cn

[R49] awk 带条件
来源：http://ai.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mu.haigaiapp.cn

[R50] awk 求和
来源：http://tg.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://go.asd995.cn

[R51] 排序去重取前几
来源：http://pw.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xy.gzmigu.cn

[R52] 统计行数
来源：http://ji.panjiajie.cn

wc -l a.txt
来源：http://xe.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://bp.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nv.wgjwhj.cn

[R54] 比较两个文件
来源：http://jp.yuntaijiaju.cn

diff a.txt b.txt
来源：http://ur.chemitech.net.cn

[R55] 压缩与解压
来源：http://eh.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mh.szsharing.cn

[R56] 远程拷贝
来源：http://mc.nicolike.cn

scp file user@host:/path/
来源：http://dt.wgjwhj.cn

[R57] 远程执行命令
来源：http://hp.shxzukj.cn

ssh user@host 'uptime'
来源：http://qm.nszjky.cn

[R58] 下载文件
来源：http://yx.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sl.wgjwhj.cn

[R59] 发 POST JSON
来源：http://ax.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ww.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://pl.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mg.bookmarksfly.cn

[R61] 磁盘占用
来源：http://wm.521024.cn

df -h;  du -sh *
来源：http://pi.shxzskj.cn

[R62] 找最占空间的文件
来源：http://vu.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://xr.9csxet.cn

[R63] 内存与进程
来源：http://vx.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://ec.huixinmuqiang.cn

[R64] 结束进程
来源：http://cj.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://qm.hnjuh.cn

[R65] 查看端口占用
来源：http://ac.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dv.muxihuayi.cn

[R66] 定时任务
来源：http://vi.shxzukj.cn

crontab -e;  crontab -l
来源：http://nk.hahajie.cn

[R67] 生成随机十六进制串
来源：http://cc.asd995.cn

openssl rand -hex 16
来源：http://jy.panjiajie.cn

[R68] 计算文件校验值
来源：http://hy.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://og.szsharing.cn

[R69] 生成随机密码
来源：http://yp.521024.cn

head -c 16 /dev/urandom | base64
来源：http://uj.szxytkj.cn

[R70] 时间戳与互转
来源：http://ig.colortex.cn

date +%s;  date -d @1700000000
来源：http://tt.jianghongdianzi.cn

[R71] 日期格式化
来源：http://og.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zi.9csxet.cn

[R72] 等待端口就绪
来源：http://fv.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ic.shtwfgs.cn

[R73] 分割大日志
来源：http://zf.hahajie.cn

split -l 1000 big.log part_
来源：http://ga.shxzukj.cn

[R74] 批量重命名
来源：http://sa.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zp.9csxet.cn

[R75] 导出环境变量
来源：http://pj.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://qq.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://qi.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dq.hahajie.cn

[R77] 读取用户输入
来源：http://uw.szsharing.cn

read -rp "请输入: " ans
来源：http://jw.huanxung.cn

[R78] 交互式菜单
来源：http://ti.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ll.nszjky.cn

[R79] 解析命令行选项
来源：http://gy.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://el.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://fs.hnjuh.cn

time ./run.sh
来源：http://qt.newstarts.cn

================================================================================
来源：http://pk.shxzskj.cn

S. C / C++ 专题
来源：http://tu.521024.cn

================================================================================
来源：http://bf.panjiajie.cn

[S01] C：Hello World
来源：http://km.chemitech.net.cn

#include <stdio.h>
来源：http://ym.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bd.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://jf.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://kr.nszjky.cn

[S03] C：读入整数
来源：http://bc.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://ao.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://mw.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ae.9csxet.cn

[S05] C：字符串长度
来源：http://wa.shxzukj.cn

strlen(s)
来源：http://rr.panjiajie.cn

[S06] C：字符串比较
来源：http://at.hahajie.cn

strcmp(a, b) == 0
来源：http://jf.szsharing.cn

[S07] C：数组遍历求和
来源：http://nf.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tf.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://on.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hc.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://un.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ol.jctech888.com.cn

[S10] C：指针与解引用
来源：http://no.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://mc.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://eu.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://xj.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zs.huanxung.cn

fclose(f);
来源：http://ws.lnxyls.cn

[S12] C：写文件
来源：http://nw.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wj.shxzukj.cn

[S13] C：宏定义
来源：http://nj.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://so.szxytkj.cn

[S14] C：枚举
来源：http://cv.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://cw.huixinmuqiang.cn

[S15] C：类型转换
来源：http://cc.yuntaijiaju.cn

(double) a / b
来源：http://jj.bookmarksfly.cn

[S16] C：位操作置位
来源：http://ni.haigaiapp.cn

x |= (1 << 3);
来源：http://qr.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://vj.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xy.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://wq.huanxung.cn

int main(int argc, char **argv)
来源：http://ol.jianghongdianzi.cn

[S19] C：快速排序
来源：http://dh.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ve.hahajie.cn

[S20] C：二分查找
来源：http://dr.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vq.nicolike.cn

[S21] C：字符类别判断
来源：http://vo.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ma.muxihuayi.cn

[S22] C：字符串转数字
来源：http://qt.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bb.newstarts.cn

[S23] C：随机数
来源：http://su.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://in.gzmigu.cn

[S24] C：获取本地时间
来源：http://zm.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oq.colortex.cn

[S25] C：内存拷贝
来源：http://ft.bjjhwx.cn

memcpy(dst, src, n);
来源：http://et.yuntaijiaju.cn

[S26] C：内存清零
来源：http://ei.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://pi.muxihuayi.cn

[S27] C：定义常量
来源：http://lt.chemitech.net.cn

const double PI = 3.14159;
来源：http://nz.nicolike.cn

[S28] C：静态变量
来源：http://ef.szsharing.cn

static int counter = 0;
来源：http://ue.gzmigu.cn

[S29] C：变参函数
来源：http://mi.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ef.nszjky.cn

[S30] C：头文件保护
来源：http://ik.huanxung.cn

#ifndef X_H
来源：http://xq.bookmarksfly.cn

#define X_H
来源：http://ei.huanxung.cn

#endif
来源：http://vo.hahajie.cn

[S31] C++：Hello World
来源：http://jt.jctech888.com.cn

#include <iostream>
来源：http://ha.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://cj.521024.cn

[S32] C++：字符串
来源：http://vu.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://dl.yuexingan06.cn

[S33] C++：vector 增删
来源：http://dv.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zd.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://ax.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://lp.nicolike.cn

[S35] C++：map
来源：http://sv.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nf.521024.cn

[S36] C++：unordered_map
来源：http://jc.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://da.haigaiapp.cn

[S37] C++：set
来源：http://hm.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hh.huanxung.cn

[S38] C++：排序
来源：http://nb.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://yo.asd995.cn

[S39] C++：自定义比较器排序
来源：http://kg.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zn.bjjhwx.cn

[S40] C++：查找元素
来源：http://hh.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ru.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://hm.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fg.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://ee.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://bp.521024.cn

[S43] C++：智能指针
来源：http://em.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://re.szxytkj.cn

[S44] C++：引用传参
来源：http://pw.521024.cn

void inc(int &x) { ++x; }
来源：http://ox.newstarts.cn

[S45] C++：lambda
来源：http://uw.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qt.huanxung.cn

[S46] C++：函数模板
来源：http://mq.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kp.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://vz.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pd.gzmigu.cn

[S48] C++：逐行读文件
来源：http://nn.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sf.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://lk.jctech888.com.cn

[S49] C++：写文件
来源：http://kn.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mb.shtwfgs.cn

[S50] C++：格式化数字
来源：http://hb.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bk.newstarts.cn

[S51] C++：显式类型转换
来源：http://tp.szsharing.cn

static_cast<double>(a) / b
来源：http://fe.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://ex.colortex.cn

int size() const noexcept { return n_; }
来源：http://is.hnjuh.cn

[S53] C++：移动语义
来源：http://fm.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://eo.521024.cn

[S54] C++：异常处理
来源：http://oc.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ul.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://lv.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zj.hahajie.cn

[S56] C++：optional
来源：http://af.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uv.haigaiapp.cn

[S57] C++：编译期常量
来源：http://or.9csxet.cn

constexpr int N = 10;
来源：http://yr.yuexingan06.cn

[S58] C++：命名空间
来源：http://ve.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://kr.newstarts.cn

[S59] C++：静态断言
来源：http://ld.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://af.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://fv.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://se.huixinmuqiang.cn

================================================================================
来源：http://hk.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://us.gzmigu.cn

================================================================================
来源：http://zh.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://wv.huixinmuqiang.cn

println("Hello")
来源：http://jq.jctech888.com.cn

[T02] Kotlin：变量
来源：http://gp.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cq.colortex.cn

[T03] Kotlin：字符串模板
来源：http://jc.muxihuayi.cn

"值: $b"
来源：http://oo.hnjuh.cn

[T04] Kotlin：空安全
来源：http://ma.shxzskj.cn

val n: String? = null;  n?.length
来源：http://vb.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://va.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bl.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://nn.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fy.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://ia.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jn.shxzukj.cn

[T08] Kotlin：数据类
来源：http://wu.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://pp.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://zt.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://co.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://ks.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xx.haigaiapp.cn

[T11] Kotlin：协程
来源：http://ps.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lc.521024.cn

[T12] Kotlin：解构声明
来源：http://ja.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://kn.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://zx.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://wv.szxytkj.cn

[T14] Kotlin：循环
来源：http://hr.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://aj.haigaiapp.cn

[T15] Kotlin：接口
来源：http://kb.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://it.9csxet.cn

[T16] Swift：Hello World
来源：http://vq.9csxet.cn

print("Hello")
来源：http://yr.newstarts.cn

[T17] Swift：变量与常量
来源：http://tn.shxzukj.cn

var a = 1;  let b = 2
来源：http://as.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://qh.bookmarksfly.cn

"值: \(b)"
来源：http://aq.gzmigu.cn

[T19] Swift：可选绑定
来源：http://sp.szsharing.cn

if let n = opt { print(n) }
来源：http://ho.newstarts.cn

[T20] Swift：数组操作
来源：http://cv.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mr.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://og.panjiajie.cn

for x in a { print(x) }
来源：http://yk.jctech888.com.cn

[T22] Swift：字典
来源：http://rb.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sk.nicolike.cn

[T23] Swift：函数
来源：http://ec.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lh.panjiajie.cn

[T24] Swift：闭包
来源：http://hh.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kb.nicolike.cn

[T25] Swift：结构体
来源：http://mn.szxytkj.cn

struct P { var x: Int }
来源：http://pz.shxzskj.cn

[T26] Swift：类与重写
来源：http://da.nicolike.cn

class A: Base { override func f() {} }
来源：http://zg.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://uz.colortex.cn

do { try f() } catch { print(error) }
来源：http://rp.gzmigu.cn

[T28] Swift：枚举
来源：http://ct.shtwfgs.cn

enum Color { case red, green }
来源：http://oq.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ro.panjiajie.cn

guard let x = opt else { return }
来源：http://wz.lnxyls.cn

[T30] Swift：协议
来源：http://en.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://ig.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://od.521024.cn

print("Hello")
来源：http://jk.muxihuayi.cn

[T32] Lua：局部变量
来源：http://os.jianghongdianzi.cn

local a = 1
来源：http://uv.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://sy.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kk.nszjky.cn

[T34] Lua：遍历表
来源：http://uy.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bj.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://yy.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://bp.nicolike.cn

[T36] Lua：函数
来源：http://nu.nszjky.cn

function add(a, b) return a + b end
来源：http://ue.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://tr.huanxung.cn

"a" .. "b"
来源：http://ac.colortex.cn

[T38] Lua：条件
来源：http://is.asd995.cn

if x > 0 then print("正") end
来源：http://pn.szsharing.cn

[T39] Lua：模式匹配
来源：http://oq.shxzukj.cn

string.find(s, "%d+")
来源：http://qa.huanxung.cn

[T40] Lua：元表
来源：http://xx.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://kv.colortex.cn


<!-- 参考信息 -->