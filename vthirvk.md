代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://pl.lnxyls.cn

[R32] 参数个数校验
来源：http://ee.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qu.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://li.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mu.hnjuh.cn

[R34] 退出时清理
来源：http://na.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://to.hahajie.cn

[R35] 后台执行并等待
来源：http://fc.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://id.hahajie.cn

[R36] 并发执行多个任务
来源：http://km.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://om.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://hl.szsharing.cn

files=$(ls -1)
来源：http://bn.521024.cn

[R38] 管道串联
来源：http://og.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://nc.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://rb.chemitech.net.cn

cmd > out.log 2>&1
来源：http://cc.asd995.cn

[R40] 追加写日志
来源：http://go.9csxet.cn

echo "log" >> out.log
来源：http://sn.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://ol.newstarts.cn

cmd >/dev/null 2>&1
来源：http://rg.lnxyls.cn

[R42] 输入重定向
来源：http://ho.521024.cn

wc -l < a.txt
来源：http://sg.colortex.cn

[R43] 按名字查找文件
来源：http://bq.huixiangedu.cn

find . -name "*.log" -type f
来源：http://fk.521024.cn

[R44] 按修改时间查找
来源：http://pl.shxzskj.cn

find . -mtime -7 -type f
来源：http://eo.szsharing.cn

[R45] 批量删除
来源：http://iu.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://mc.szxytkj.cn

[R46] 递归替换文件内容
来源：http://xt.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wd.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://qa.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rg.szsharing.cn

[R48] awk 取指定列
来源：http://ct.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://tn.panjiajie.cn

[R49] awk 带条件
来源：http://bu.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fq.huanxung.cn

[R50] awk 求和
来源：http://qu.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ii.bjjhwx.cn

[R51] 排序去重取前几
来源：http://ao.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mv.yuexingan06.cn

[R52] 统计行数
来源：http://aw.hnjuh.cn

wc -l a.txt
来源：http://tm.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://cp.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xn.nicolike.cn

[R54] 比较两个文件
来源：http://xn.szxytkj.cn

diff a.txt b.txt
来源：http://cd.szxytkj.cn

[R55] 压缩与解压
来源：http://ro.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gu.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://vl.bjjhwx.cn

scp file user@host:/path/
来源：http://tc.9csxet.cn

[R57] 远程执行命令
来源：http://oo.newstarts.cn

ssh user@host 'uptime'
来源：http://qj.shtwfgs.cn

[R58] 下载文件
来源：http://po.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jk.shxzskj.cn

[R59] 发 POST JSON
来源：http://md.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oa.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://nu.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ve.chemitech.net.cn

[R61] 磁盘占用
来源：http://bc.lnxyls.cn

df -h;  du -sh *
来源：http://eo.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://tm.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://xp.yuntaijiaju.cn

[R63] 内存与进程
来源：http://he.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://jj.yuntaijiaju.cn

[R64] 结束进程
来源：http://al.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://tx.huanxung.cn

[R65] 查看端口占用
来源：http://kn.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rt.huixiangedu.cn

[R66] 定时任务
来源：http://ie.asd995.cn

crontab -e;  crontab -l
来源：http://lj.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://cn.gzmigu.cn

openssl rand -hex 16
来源：http://ma.nicolike.cn

[R68] 计算文件校验值
来源：http://xh.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gq.nszjky.cn

[R69] 生成随机密码
来源：http://ce.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://pj.wgjwhj.cn

[R70] 时间戳与互转
来源：http://zv.nszjky.cn

date +%s;  date -d @1700000000
来源：http://gh.huanxung.cn

[R71] 日期格式化
来源：http://sr.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lb.huixiangedu.cn

[R72] 等待端口就绪
来源：http://rg.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ya.asd995.cn

[R73] 分割大日志
来源：http://qn.yuexingan06.cn

split -l 1000 big.log part_
来源：http://ar.panjiajie.cn

[R74] 批量重命名
来源：http://id.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wb.nszjky.cn

[R75] 导出环境变量
来源：http://yf.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://po.nicolike.cn

[R76] 使用临时文件
来源：http://fm.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ly.gzmigu.cn

[R77] 读取用户输入
来源：http://rg.521024.cn

read -rp "请输入: " ans
来源：http://be.huanxung.cn

[R78] 交互式菜单
来源：http://az.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ot.newstarts.cn

[R79] 解析命令行选项
来源：http://ke.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ly.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://ig.muxihuayi.cn

time ./run.sh
来源：http://iv.newstarts.cn

================================================================================
来源：http://to.huanxung.cn

S. C / C++ 专题
来源：http://de.huixiangedu.cn

================================================================================
来源：http://qq.lnxyls.cn

[S01] C：Hello World
来源：http://js.jianghongdianzi.cn

#include <stdio.h>
来源：http://ze.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pz.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://ya.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://hk.jianghongdianzi.cn

[S03] C：读入整数
来源：http://zj.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://vh.shxzskj.cn

[S04] C：字符串复制
来源：http://gi.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ol.huanxung.cn

[S05] C：字符串长度
来源：http://hh.gzmigu.cn

strlen(s)
来源：http://hr.yuexingan06.cn

[S06] C：字符串比较
来源：http://yg.hnjuh.cn

strcmp(a, b) == 0
来源：http://yi.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://rq.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nq.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://ys.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ax.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://ja.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bv.asd995.cn

[S10] C：指针与解引用
来源：http://it.szsharing.cn

int *p = &a;  *p = 5;
来源：http://gb.huanxung.cn

[S11] C：逐行读文件
来源：http://sn.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://xx.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mi.muxihuayi.cn

fclose(f);
来源：http://nc.hnjuh.cn

[S12] C：写文件
来源：http://ih.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ub.huanxung.cn

[S13] C：宏定义
来源：http://bf.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://me.szxytkj.cn

[S14] C：枚举
来源：http://ij.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ca.shxzukj.cn

[S15] C：类型转换
来源：http://zz.huixiangedu.cn

(double) a / b
来源：http://kw.huixiangedu.cn

[S16] C：位操作置位
来源：http://zl.hnjuh.cn

x |= (1 << 3);
来源：http://gv.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://xq.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://be.lnxyls.cn

[S18] C：命令行参数
来源：http://dh.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://eo.nszjky.cn

[S19] C：快速排序
来源：http://yo.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qa.shxzskj.cn

[S20] C：二分查找
来源：http://ft.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://va.newstarts.cn

[S21] C：字符类别判断
来源：http://ob.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zc.muxihuayi.cn

[S22] C：字符串转数字
来源：http://nj.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ik.521024.cn

[S23] C：随机数
来源：http://ke.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tk.shxzskj.cn

[S24] C：获取本地时间
来源：http://kz.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uz.panjiajie.cn

[S25] C：内存拷贝
来源：http://np.nicolike.cn

memcpy(dst, src, n);
来源：http://ih.lnxyls.cn

[S26] C：内存清零
来源：http://ee.9csxet.cn

memset(a, 0, sizeof a);
来源：http://vb.nszjky.cn

[S27] C：定义常量
来源：http://md.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://wj.bookmarksfly.cn

[S28] C：静态变量
来源：http://ge.panjiajie.cn

static int counter = 0;
来源：http://ku.hnjuh.cn

[S29] C：变参函数
来源：http://vo.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rg.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://nj.jianghongdianzi.cn

#ifndef X_H
来源：http://kx.shxzskj.cn

#define X_H
来源：http://kd.nszjky.cn

#endif
来源：http://ed.gzmigu.cn

[S31] C++：Hello World
来源：http://yh.nszjky.cn

#include <iostream>
来源：http://nu.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://fj.nicolike.cn

[S32] C++：字符串
来源：http://fr.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://as.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://jw.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://an.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://xz.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://kh.huanxung.cn

[S35] C++：map
来源：http://vt.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dz.nszjky.cn

[S36] C++：unordered_map
来源：http://tc.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bk.bjjhwx.cn

[S37] C++：set
来源：http://if.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lr.szxytkj.cn

[S38] C++：排序
来源：http://et.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://ez.colortex.cn

[S39] C++：自定义比较器排序
来源：http://ua.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wm.jctech888.com.cn

[S40] C++：查找元素
来源：http://gj.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kr.gzmigu.cn

[S41] C++：类与构造函数
来源：http://ld.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://am.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://ia.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://dp.newstarts.cn

[S43] C++：智能指针
来源：http://ph.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://vo.9csxet.cn

[S44] C++：引用传参
来源：http://bs.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://et.asd995.cn

[S45] C++：lambda
来源：http://pv.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wl.asd995.cn

[S46] C++：函数模板
来源：http://fj.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qv.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://zg.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ky.panjiajie.cn

[S48] C++：逐行读文件
来源：http://dr.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jv.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://pk.newstarts.cn

[S49] C++：写文件
来源：http://yj.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wq.huixiangedu.cn

[S50] C++：格式化数字
来源：http://un.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://di.nszjky.cn

[S51] C++：显式类型转换
来源：http://qd.asd995.cn

static_cast<double>(a) / b
来源：http://uy.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://im.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://ar.shxzskj.cn

[S53] C++：移动语义
来源：http://vb.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://wf.nicolike.cn

[S54] C++：异常处理
来源：http://sm.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sz.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://zb.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tz.panjiajie.cn

[S56] C++：optional
来源：http://vr.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yy.huanxung.cn

[S57] C++：编译期常量
来源：http://pn.jianghongdianzi.cn

constexpr int N = 10;
来源：http://up.wgjwhj.cn

[S58] C++：命名空间
来源：http://zi.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://vw.shtwfgs.cn

[S59] C++：静态断言
来源：http://qd.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ce.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://wo.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zp.huanxung.cn

================================================================================
来源：http://wx.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vk.muxihuayi.cn

================================================================================
来源：http://wt.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://mj.lnxyls.cn

println("Hello")
来源：http://qb.9csxet.cn

[T02] Kotlin：变量
来源：http://pm.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fl.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://op.hahajie.cn

"值: $b"
来源：http://ly.szxytkj.cn

[T04] Kotlin：空安全
来源：http://ld.lnxyls.cn

val n: String? = null;  n?.length
来源：http://lc.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://ru.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hy.521024.cn

[T06] Kotlin：集合映射
来源：http://jq.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cl.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://aw.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yr.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://pc.asd995.cn

data class User(val name: String, val age: Int)
来源：http://fx.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://dg.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://wj.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://qr.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wu.chemitech.net.cn

[T11] Kotlin：协程
来源：http://dy.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xb.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://lj.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://ek.asd995.cn

[T13] Kotlin：只读 Map
来源：http://lr.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://wq.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://bd.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://zg.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://we.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://vi.chemitech.net.cn

[T16] Swift：Hello World
来源：http://kk.hnjuh.cn

print("Hello")
来源：http://nu.nicolike.cn

[T17] Swift：变量与常量
来源：http://ti.hahajie.cn

var a = 1;  let b = 2
来源：http://qr.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://nx.haigaiapp.cn

"值: \(b)"
来源：http://ou.newstarts.cn

[T19] Swift：可选绑定
来源：http://iz.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://ct.huixiangedu.cn

[T20] Swift：数组操作
来源：http://lg.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ug.shxzukj.cn

[T21] Swift：遍历
来源：http://vu.nicolike.cn

for x in a { print(x) }
来源：http://fq.nicolike.cn

[T22] Swift：字典
来源：http://dd.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zl.hnjuh.cn

[T23] Swift：函数
来源：http://vp.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://st.bjjhwx.cn

[T24] Swift：闭包
来源：http://am.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vh.9csxet.cn

[T25] Swift：结构体
来源：http://ia.huixiangedu.cn

struct P { var x: Int }
来源：http://zg.newstarts.cn

[T26] Swift：类与重写
来源：http://ea.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://dz.newstarts.cn

[T27] Swift：错误处理
来源：http://ve.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://ik.nicolike.cn

[T28] Swift：枚举
来源：http://bk.hnjuh.cn

enum Color { case red, green }
来源：http://sr.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://pj.gzmigu.cn

guard let x = opt else { return }
来源：http://tb.szsharing.cn

[T30] Swift：协议
来源：http://uw.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://xt.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://ho.jctech888.com.cn

print("Hello")
来源：http://ga.huanxung.cn

[T32] Lua：局部变量
来源：http://zc.yuntaijiaju.cn

local a = 1
来源：http://jq.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://ea.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zo.asd995.cn

[T34] Lua：遍历表
来源：http://tj.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ef.bjjhwx.cn


<!-- 参考信息 -->