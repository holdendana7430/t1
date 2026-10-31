代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tq.asd995.cn

[R34] 退出时清理
来源：http://jo.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ch.shtwfgs.cn

[R35] 后台执行并等待
来源：http://un.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zz.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://yy.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pc.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://xn.asd995.cn

files=$(ls -1)
来源：http://dm.muxihuayi.cn

[R38] 管道串联
来源：http://kf.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://hi.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://oc.newstarts.cn

cmd > out.log 2>&1
来源：http://da.huixiangedu.cn

[R40] 追加写日志
来源：http://ct.huanxung.cn

echo "log" >> out.log
来源：http://nb.huanxung.cn

[R41] 丢弃输出
来源：http://ah.huanxung.cn

cmd >/dev/null 2>&1
来源：http://co.shxzukj.cn

[R42] 输入重定向
来源：http://zh.bookmarksfly.cn

wc -l < a.txt
来源：http://xe.shxzskj.cn

[R43] 按名字查找文件
来源：http://jv.nicolike.cn

find . -name "*.log" -type f
来源：http://gw.szsharing.cn

[R44] 按修改时间查找
来源：http://kl.nszjky.cn

find . -mtime -7 -type f
来源：http://kw.haigaiapp.cn

[R45] 批量删除
来源：http://qs.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://ez.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://ob.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jj.huixiangedu.cn

[R47] sed 单行替换
来源：http://fv.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wy.nicolike.cn

[R48] awk 取指定列
来源：http://lw.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://hy.colortex.cn

[R49] awk 带条件
来源：http://nu.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wg.chemitech.net.cn

[R50] awk 求和
来源：http://su.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vw.nicolike.cn

[R51] 排序去重取前几
来源：http://gt.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hy.huixinmuqiang.cn

[R52] 统计行数
来源：http://ie.shtwfgs.cn

wc -l a.txt
来源：http://qp.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://kq.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dj.shtwfgs.cn

[R54] 比较两个文件
来源：http://nx.wgjwhj.cn

diff a.txt b.txt
来源：http://bw.nicolike.cn

[R55] 压缩与解压
来源：http://so.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kn.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ie.hahajie.cn

scp file user@host:/path/
来源：http://hc.shxzskj.cn

[R57] 远程执行命令
来源：http://zn.muxihuayi.cn

ssh user@host 'uptime'
来源：http://tg.bjjhwx.cn

[R58] 下载文件
来源：http://eg.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qa.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://ep.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://td.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://yu.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wc.shtwfgs.cn

[R61] 磁盘占用
来源：http://yb.nicolike.cn

df -h;  du -sh *
来源：http://xv.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://if.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://dd.9csxet.cn

[R63] 内存与进程
来源：http://sp.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://ma.bjjhwx.cn

[R64] 结束进程
来源：http://dk.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://ag.jctech888.com.cn

[R65] 查看端口占用
来源：http://gf.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ro.hnjuh.cn

[R66] 定时任务
来源：http://ec.panjiajie.cn

crontab -e;  crontab -l
来源：http://wl.521024.cn

[R67] 生成随机十六进制串
来源：http://ed.hahajie.cn

openssl rand -hex 16
来源：http://jt.yuexingan06.cn

[R68] 计算文件校验值
来源：http://nd.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://to.shxzskj.cn

[R69] 生成随机密码
来源：http://ek.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://na.huanxung.cn

[R70] 时间戳与互转
来源：http://nl.szsharing.cn

date +%s;  date -d @1700000000
来源：http://iu.huixinmuqiang.cn

[R71] 日期格式化
来源：http://ks.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fs.szxytkj.cn

[R72] 等待端口就绪
来源：http://by.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rv.gzmigu.cn

[R73] 分割大日志
来源：http://ls.asd995.cn

split -l 1000 big.log part_
来源：http://eg.szsharing.cn

[R74] 批量重命名
来源：http://ce.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gx.muxihuayi.cn

[R75] 导出环境变量
来源：http://po.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://fj.9csxet.cn

[R76] 使用临时文件
来源：http://rx.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ij.yuexingan06.cn

[R77] 读取用户输入
来源：http://kb.521024.cn

read -rp "请输入: " ans
来源：http://ny.yuexingan06.cn

[R78] 交互式菜单
来源：http://md.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ji.521024.cn

[R79] 解析命令行选项
来源：http://cm.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vd.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://ku.asd995.cn

time ./run.sh
来源：http://tw.hahajie.cn

================================================================================
来源：http://zb.hahajie.cn

S. C / C++ 专题
来源：http://xc.yuntaijiaju.cn

================================================================================
来源：http://yf.szxytkj.cn

[S01] C：Hello World
来源：http://ix.asd995.cn

#include <stdio.h>
来源：http://ty.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ok.521024.cn

[S02] C：变量与格式化输出
来源：http://kb.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://si.shtwfgs.cn

[S03] C：读入整数
来源：http://vp.asd995.cn

int x; scanf("%d", &x);
来源：http://vo.colortex.cn

[S04] C：字符串复制
来源：http://mm.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dy.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://ve.asd995.cn

strlen(s)
来源：http://nr.szxytkj.cn

[S06] C：字符串比较
来源：http://ly.hahajie.cn

strcmp(a, b) == 0
来源：http://qv.nicolike.cn

[S07] C：数组遍历求和
来源：http://qq.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tc.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://tt.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mf.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://im.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sw.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://sk.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://zk.huixiangedu.cn

[S11] C：逐行读文件
来源：http://ip.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://dr.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zu.lnxyls.cn

fclose(f);
来源：http://bd.shtwfgs.cn

[S12] C：写文件
来源：http://nr.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xz.lnxyls.cn

[S13] C：宏定义
来源：http://cx.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rr.bookmarksfly.cn

[S14] C：枚举
来源：http://oh.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://pg.bookmarksfly.cn

[S15] C：类型转换
来源：http://hq.muxihuayi.cn

(double) a / b
来源：http://oj.nicolike.cn

[S16] C：位操作置位
来源：http://pm.shxzukj.cn

x |= (1 << 3);
来源：http://fp.huanxung.cn

[S17] C：安全拼接字符串
来源：http://th.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ke.gzmigu.cn

[S18] C：命令行参数
来源：http://gw.nszjky.cn

int main(int argc, char **argv)
来源：http://xx.nicolike.cn

[S19] C：快速排序
来源：http://iw.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tr.shxzskj.cn

[S20] C：二分查找
来源：http://cd.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hn.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://jc.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kh.hahajie.cn

[S22] C：字符串转数字
来源：http://bo.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sj.521024.cn

[S23] C：随机数
来源：http://aq.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pa.huixiangedu.cn

[S24] C：获取本地时间
来源：http://cn.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gd.haigaiapp.cn

[S25] C：内存拷贝
来源：http://nu.hahajie.cn

memcpy(dst, src, n);
来源：http://ec.colortex.cn

[S26] C：内存清零
来源：http://tu.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://yj.haigaiapp.cn

[S27] C：定义常量
来源：http://dd.nszjky.cn

const double PI = 3.14159;
来源：http://av.gzmigu.cn

[S28] C：静态变量
来源：http://my.gzmigu.cn

static int counter = 0;
来源：http://rc.huixiangedu.cn

[S29] C：变参函数
来源：http://ps.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sm.nicolike.cn

[S30] C：头文件保护
来源：http://xa.bookmarksfly.cn

#ifndef X_H
来源：http://ze.lnxyls.cn

#define X_H
来源：http://rx.szxytkj.cn

#endif
来源：http://cs.jctech888.com.cn

[S31] C++：Hello World
来源：http://gn.szsharing.cn

#include <iostream>
来源：http://rg.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://nf.huanxung.cn

[S32] C++：字符串
来源：http://xt.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://vy.521024.cn

[S33] C++：vector 增删
来源：http://mg.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xs.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://hz.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://fr.hnjuh.cn

[S35] C++：map
来源：http://cf.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bv.wgjwhj.cn

[S36] C++：unordered_map
来源：http://wd.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cu.szsharing.cn

[S37] C++：set
来源：http://nv.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dj.wgjwhj.cn

[S38] C++：排序
来源：http://hm.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://fw.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://xx.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cn.asd995.cn

[S40] C++：查找元素
来源：http://tu.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yo.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://as.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mj.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://mw.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://de.wgjwhj.cn

[S43] C++：智能指针
来源：http://pw.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://kn.wgjwhj.cn

[S44] C++：引用传参
来源：http://zk.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://uf.9csxet.cn

[S45] C++：lambda
来源：http://hi.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://td.gzmigu.cn

[S46] C++：函数模板
来源：http://sx.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://su.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://st.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://at.huanxung.cn

[S48] C++：逐行读文件
来源：http://pc.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pp.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://va.bookmarksfly.cn

[S49] C++：写文件
来源：http://wj.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uo.chemitech.net.cn

[S50] C++：格式化数字
来源：http://eh.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vu.nszjky.cn

[S51] C++：显式类型转换
来源：http://qf.asd995.cn

static_cast<double>(a) / b
来源：http://sa.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://ba.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://rr.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://ro.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://kl.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://ev.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gb.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://yj.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://su.haigaiapp.cn

[S56] C++：optional
来源：http://qy.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ru.shxzukj.cn

[S57] C++：编译期常量
来源：http://ps.szxytkj.cn

constexpr int N = 10;
来源：http://ov.huanxung.cn

[S58] C++：命名空间
来源：http://zj.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://cl.gzmigu.cn

[S59] C++：静态断言
来源：http://sl.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zf.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://ie.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gw.hahajie.cn

================================================================================
来源：http://ji.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://od.shxzukj.cn

================================================================================
来源：http://kb.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://vv.szsharing.cn

println("Hello")
来源：http://ml.jctech888.com.cn

[T02] Kotlin：变量
来源：http://ln.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://il.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://ut.yuntaijiaju.cn

"值: $b"
来源：http://qv.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://tw.hahajie.cn

val n: String? = null;  n?.length
来源：http://na.521024.cn

[T05] Kotlin：when 表达式
来源：http://fm.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gv.521024.cn

[T06] Kotlin：集合映射
来源：http://uq.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uu.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://hh.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ka.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://qr.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://lc.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://ye.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://uo.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://lt.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vf.haigaiapp.cn

[T11] Kotlin：协程
来源：http://za.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://as.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://vr.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://hn.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://qb.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://sp.521024.cn

[T14] Kotlin：循环
来源：http://hv.shxzskj.cn

for (i in 1..10) println(i)
来源：http://la.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://zy.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://ec.colortex.cn

[T16] Swift：Hello World
来源：http://bh.jctech888.com.cn

print("Hello")
来源：http://fk.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://em.huixiangedu.cn

var a = 1;  let b = 2
来源：http://ms.szsharing.cn

[T18] Swift：字符串插值
来源：http://bt.521024.cn

"值: \(b)"
来源：http://zr.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://oi.huixiangedu.cn

if let n = opt { print(n) }
来源：http://sn.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://jx.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yq.521024.cn

[T21] Swift：遍历
来源：http://mp.yuexingan06.cn

for x in a { print(x) }
来源：http://mv.szsharing.cn

[T22] Swift：字典
来源：http://nv.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fe.nszjky.cn

[T23] Swift：函数
来源：http://vm.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vo.newstarts.cn

[T24] Swift：闭包
来源：http://zr.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kz.muxihuayi.cn

[T25] Swift：结构体
来源：http://un.asd995.cn

struct P { var x: Int }
来源：http://mq.521024.cn

[T26] Swift：类与重写
来源：http://iu.szsharing.cn

class A: Base { override func f() {} }
来源：http://rg.hahajie.cn

[T27] Swift：错误处理
来源：http://ca.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://yi.lnxyls.cn

[T28] Swift：枚举
来源：http://zu.szsharing.cn

enum Color { case red, green }
来源：http://bv.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://xq.asd995.cn

guard let x = opt else { return }
来源：http://wj.nszjky.cn

[T30] Swift：协议
来源：http://al.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://ui.nicolike.cn

[T31] Lua：Hello World
来源：http://zd.huanxung.cn

print("Hello")
来源：http://cq.colortex.cn

[T32] Lua：局部变量
来源：http://lg.szxytkj.cn

local a = 1
来源：http://bl.szsharing.cn

[T33] Lua：表（数组）
来源：http://ku.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pq.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://an.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://je.asd995.cn

[T35] Lua：字典表
来源：http://we.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://zy.bjjhwx.cn

[T36] Lua：函数
来源：http://bx.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://zo.szsharing.cn


<!-- 参考信息 -->