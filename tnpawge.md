代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://ae.newstarts.cn

[R52] 统计行数
来源：http://gs.panjiajie.cn

wc -l a.txt
来源：http://nc.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://hf.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gr.szsharing.cn

[R54] 比较两个文件
来源：http://jy.yuntaijiaju.cn

diff a.txt b.txt
来源：http://dr.shtwfgs.cn

[R55] 压缩与解压
来源：http://qk.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ms.bjjhwx.cn

[R56] 远程拷贝
来源：http://ye.9csxet.cn

scp file user@host:/path/
来源：http://am.shtwfgs.cn

[R57] 远程执行命令
来源：http://gm.szsharing.cn

ssh user@host 'uptime'
来源：http://ls.shxzskj.cn

[R58] 下载文件
来源：http://um.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ku.chemitech.net.cn

[R59] 发 POST JSON
来源：http://bv.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mh.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://ld.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ie.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://cp.huanxung.cn

df -h;  du -sh *
来源：http://km.huanxung.cn

[R62] 找最占空间的文件
来源：http://vw.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://qe.asd995.cn

[R63] 内存与进程
来源：http://fy.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://qh.panjiajie.cn

[R64] 结束进程
来源：http://lu.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://oa.szsharing.cn

[R65] 查看端口占用
来源：http://zl.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://si.yuntaijiaju.cn

[R66] 定时任务
来源：http://eo.shtwfgs.cn

crontab -e;  crontab -l
来源：http://ek.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://ei.hnjuh.cn

openssl rand -hex 16
来源：http://bt.shxzskj.cn

[R68] 计算文件校验值
来源：http://fq.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hd.colortex.cn

[R69] 生成随机密码
来源：http://xb.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://pt.yuexingan06.cn

[R70] 时间戳与互转
来源：http://th.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://ko.gzmigu.cn

[R71] 日期格式化
来源：http://fo.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://du.huixiangedu.cn

[R72] 等待端口就绪
来源：http://bd.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xu.jianghongdianzi.cn

[R73] 分割大日志
来源：http://pe.nicolike.cn

split -l 1000 big.log part_
来源：http://bn.hahajie.cn

[R74] 批量重命名
来源：http://wo.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kb.huixiangedu.cn

[R75] 导出环境变量
来源：http://sh.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://zq.chemitech.net.cn

[R76] 使用临时文件
来源：http://ci.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://or.hnjuh.cn

[R77] 读取用户输入
来源：http://be.gzmigu.cn

read -rp "请输入: " ans
来源：http://pu.shxzskj.cn

[R78] 交互式菜单
来源：http://kb.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gm.shtwfgs.cn

[R79] 解析命令行选项
来源：http://fp.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wp.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://ed.huanxung.cn

time ./run.sh
来源：http://nt.shtwfgs.cn

================================================================================
来源：http://vo.chemitech.net.cn

S. C / C++ 专题
来源：http://pc.huixinmuqiang.cn

================================================================================
来源：http://dh.wgjwhj.cn

[S01] C：Hello World
来源：http://aq.huixiangedu.cn

#include <stdio.h>
来源：http://sq.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dn.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://al.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://ki.muxihuayi.cn

[S03] C：读入整数
来源：http://ve.shxzskj.cn

int x; scanf("%d", &x);
来源：http://un.yuexingan06.cn

[S04] C：字符串复制
来源：http://fr.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vc.panjiajie.cn

[S05] C：字符串长度
来源：http://fr.asd995.cn

strlen(s)
来源：http://cl.9csxet.cn

[S06] C：字符串比较
来源：http://ss.szxytkj.cn

strcmp(a, b) == 0
来源：http://cm.hahajie.cn

[S07] C：数组遍历求和
来源：http://dx.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vp.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://sn.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xx.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://cq.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tz.hnjuh.cn

[S10] C：指针与解引用
来源：http://rf.521024.cn

int *p = &a;  *p = 5;
来源：http://wt.shxzukj.cn

[S11] C：逐行读文件
来源：http://eq.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://fu.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://on.hahajie.cn

fclose(f);
来源：http://vy.huanxung.cn

[S12] C：写文件
来源：http://jm.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gp.hnjuh.cn

[S13] C：宏定义
来源：http://zn.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sx.colortex.cn

[S14] C：枚举
来源：http://up.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://kf.9csxet.cn

[S15] C：类型转换
来源：http://nv.muxihuayi.cn

(double) a / b
来源：http://ya.shtwfgs.cn

[S16] C：位操作置位
来源：http://mq.gzmigu.cn

x |= (1 << 3);
来源：http://ly.asd995.cn

[S17] C：安全拼接字符串
来源：http://bc.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bm.szsharing.cn

[S18] C：命令行参数
来源：http://gu.jctech888.com.cn

int main(int argc, char **argv)
来源：http://jq.panjiajie.cn

[S19] C：快速排序
来源：http://tn.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ia.yuexingan06.cn

[S20] C：二分查找
来源：http://ui.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qz.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://ry.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yu.newstarts.cn

[S22] C：字符串转数字
来源：http://tg.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gs.hnjuh.cn

[S23] C：随机数
来源：http://re.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fd.chemitech.net.cn

[S24] C：获取本地时间
来源：http://ea.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pu.haigaiapp.cn

[S25] C：内存拷贝
来源：http://tu.lnxyls.cn

memcpy(dst, src, n);
来源：http://kn.haigaiapp.cn

[S26] C：内存清零
来源：http://dl.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://ap.521024.cn

[S27] C：定义常量
来源：http://ux.colortex.cn

const double PI = 3.14159;
来源：http://kb.shxzukj.cn

[S28] C：静态变量
来源：http://my.wgjwhj.cn

static int counter = 0;
来源：http://nr.huixiangedu.cn

[S29] C：变参函数
来源：http://cf.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cr.haigaiapp.cn

[S30] C：头文件保护
来源：http://wt.huixinmuqiang.cn

#ifndef X_H
来源：http://jh.bjjhwx.cn

#define X_H
来源：http://ca.bookmarksfly.cn

#endif
来源：http://yw.521024.cn

[S31] C++：Hello World
来源：http://bt.szsharing.cn

#include <iostream>
来源：http://st.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://oq.huanxung.cn

[S32] C++：字符串
来源：http://tv.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://uq.wgjwhj.cn

[S33] C++：vector 增删
来源：http://fr.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kt.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://id.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://jo.wgjwhj.cn

[S35] C++：map
来源：http://hl.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zm.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://on.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hl.chemitech.net.cn

[S37] C++：set
来源：http://ei.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vc.yuexingan06.cn

[S38] C++：排序
来源：http://wt.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://xf.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://sp.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gh.asd995.cn

[S40] C++：查找元素
来源：http://lu.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ar.gzmigu.cn

[S41] C++：类与构造函数
来源：http://sg.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ar.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://rb.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://ls.9csxet.cn

[S43] C++：智能指针
来源：http://gi.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://zt.yuexingan06.cn

[S44] C++：引用传参
来源：http://ds.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ya.yuexingan06.cn

[S45] C++：lambda
来源：http://cv.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://et.haigaiapp.cn

[S46] C++：函数模板
来源：http://vz.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://br.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://wz.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hn.szxytkj.cn

[S48] C++：逐行读文件
来源：http://tq.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dc.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://mu.hnjuh.cn

[S49] C++：写文件
来源：http://gd.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kh.jctech888.com.cn

[S50] C++：格式化数字
来源：http://jf.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dv.shxzukj.cn

[S51] C++：显式类型转换
来源：http://gu.hahajie.cn

static_cast<double>(a) / b
来源：http://es.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://nm.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://ie.haigaiapp.cn

[S53] C++：移动语义
来源：http://qm.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://cz.muxihuayi.cn

[S54] C++：异常处理
来源：http://jl.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mq.shxzskj.cn

[S55] C++：结构化绑定
来源：http://nu.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ff.gzmigu.cn

[S56] C++：optional
来源：http://vk.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dj.521024.cn

[S57] C++：编译期常量
来源：http://ut.muxihuayi.cn

constexpr int N = 10;
来源：http://fl.szxytkj.cn

[S58] C++：命名空间
来源：http://of.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://zb.huanxung.cn

[S59] C++：静态断言
来源：http://bk.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yh.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://in.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wb.haigaiapp.cn

================================================================================
来源：http://gk.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oy.shxzukj.cn

================================================================================
来源：http://gi.szsharing.cn

[T01] Kotlin：Hello World
来源：http://tf.szxytkj.cn

println("Hello")
来源：http://xc.shtwfgs.cn

[T02] Kotlin：变量
来源：http://ls.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://in.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://nv.hahajie.cn

"值: $b"
来源：http://hf.colortex.cn

[T04] Kotlin：空安全
来源：http://co.nszjky.cn

val n: String? = null;  n?.length
来源：http://sk.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://uh.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hr.asd995.cn

[T06] Kotlin：集合映射
来源：http://hg.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rc.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://qq.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ju.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://nq.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://hr.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://sd.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://ar.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://gx.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hj.asd995.cn

[T11] Kotlin：协程
来源：http://sr.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jr.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://mb.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://re.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://uv.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://xz.yuexingan06.cn

[T14] Kotlin：循环
来源：http://ra.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://ve.bjjhwx.cn

[T15] Kotlin：接口
来源：http://vn.hahajie.cn

interface Shape { fun area(): Double }
来源：http://pe.wgjwhj.cn

[T16] Swift：Hello World
来源：http://kk.huixiangedu.cn

print("Hello")
来源：http://kt.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://nn.szxytkj.cn

var a = 1;  let b = 2
来源：http://wr.gzmigu.cn

[T18] Swift：字符串插值
来源：http://it.9csxet.cn

"值: \(b)"
来源：http://nt.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://ci.hnjuh.cn

if let n = opt { print(n) }
来源：http://dv.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://if.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vi.panjiajie.cn

[T21] Swift：遍历
来源：http://qo.huixinmuqiang.cn

for x in a { print(x) }
来源：http://ha.panjiajie.cn

[T22] Swift：字典
来源：http://pd.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xn.shxzskj.cn

[T23] Swift：函数
来源：http://ep.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fo.521024.cn

[T24] Swift：闭包
来源：http://xg.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gt.haigaiapp.cn

[T25] Swift：结构体
来源：http://ac.panjiajie.cn

struct P { var x: Int }
来源：http://na.shtwfgs.cn

[T26] Swift：类与重写
来源：http://td.9csxet.cn

class A: Base { override func f() {} }
来源：http://rs.huixiangedu.cn

[T27] Swift：错误处理
来源：http://ka.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://ec.shxzskj.cn

[T28] Swift：枚举
来源：http://pg.newstarts.cn

enum Color { case red, green }
来源：http://ec.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://gz.nszjky.cn

guard let x = opt else { return }
来源：http://bs.asd995.cn

[T30] Swift：协议
来源：http://pp.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://xr.nszjky.cn

[T31] Lua：Hello World
来源：http://gl.9csxet.cn

print("Hello")
来源：http://wz.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://qs.chemitech.net.cn

local a = 1
来源：http://xq.colortex.cn

[T33] Lua：表（数组）
来源：http://tw.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mk.huanxung.cn

[T34] Lua：遍历表
来源：http://fm.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://od.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://gd.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://jq.shxzskj.cn

[T36] Lua：函数
来源：http://db.nicolike.cn

function add(a, b) return a + b end
来源：http://yd.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://ar.jianghongdianzi.cn

"a" .. "b"
来源：http://ft.szxytkj.cn

[T38] Lua：条件
来源：http://ic.wgjwhj.cn

if x > 0 then print("正") end
来源：http://yh.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://qh.hahajie.cn

string.find(s, "%d+")
来源：http://hz.nicolike.cn

[T40] Lua：元表
来源：http://eq.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://qv.szxytkj.cn

[T41] Perl：Hello World
来源：http://ie.huanxung.cn

print "Hello\n";
来源：http://np.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://tu.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://js.gzmigu.cn

[T43] Perl：字符串插值
来源：http://zc.colortex.cn

"值: $a"
来源：http://jc.shxzukj.cn

[T44] Perl：条件
来源：http://wd.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://sc.panjiajie.cn

[T45] Perl：数组遍历
来源：http://lp.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://zn.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://bf.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vc.hahajie.cn

[T47] Perl：正则捕获
来源：http://hz.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ae.hnjuh.cn

[T48] Perl：正则替换
来源：http://hk.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://sg.gzmigu.cn

[T49] Perl：函数
来源：http://nu.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://po.521024.cn

[T50] Perl：逐行读文件
来源：http://yb.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xo.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://uh.szxytkj.cn

[T51] Scala：Hello World
来源：http://be.haigaiapp.cn

println("Hello")
来源：http://dq.newstarts.cn

[T52] Scala：变量
来源：http://kc.bjjhwx.cn

val a = 1;  var b = 2
来源：http://mt.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://tv.huanxung.cn

s"值: $b"
来源：http://cg.nicolike.cn

[T54] Scala：集合映射
来源：http://qv.shxzukj.cn


<!-- 参考信息 -->