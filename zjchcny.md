代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://os.panjiajie.cn

[R24] 大小写转换
来源：http://nb.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ua.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://sw.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jl.lnxyls.cn

[R26] 命令替换
来源：http://py.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://sz.shtwfgs.cn

[R27] 算术展开
来源：http://dd.nicolike.cn

echo $((1 + 2 * 3))
来源：http://ym.bjjhwx.cn

[R28] 浮点运算
来源：http://wq.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://kb.haigaiapp.cn

[R29] 定义函数
来源：http://lr.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mg.huanxung.cn

[R30] 函数返回状态码
来源：http://dh.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://fw.chemitech.net.cn

[R31] 局部变量
来源：http://jf.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://xi.muxihuayi.cn

[R32] 参数个数校验
来源：http://vf.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ds.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://vv.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wt.lnxyls.cn

[R34] 退出时清理
来源：http://mm.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://io.lnxyls.cn

[R35] 后台执行并等待
来源：http://ok.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ct.521024.cn

[R36] 并发执行多个任务
来源：http://aj.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eo.lnxyls.cn

[R37] 把输出赋给变量
来源：http://fh.shxzukj.cn

files=$(ls -1)
来源：http://ke.nszjky.cn

[R38] 管道串联
来源：http://it.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://ih.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://fd.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://zp.muxihuayi.cn

[R40] 追加写日志
来源：http://yn.bookmarksfly.cn

echo "log" >> out.log
来源：http://hj.shxzskj.cn

[R41] 丢弃输出
来源：http://en.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://ix.chemitech.net.cn

[R42] 输入重定向
来源：http://hr.shxzukj.cn

wc -l < a.txt
来源：http://iq.shtwfgs.cn

[R43] 按名字查找文件
来源：http://fo.hahajie.cn

find . -name "*.log" -type f
来源：http://xr.lnxyls.cn

[R44] 按修改时间查找
来源：http://vz.huixiangedu.cn

find . -mtime -7 -type f
来源：http://th.asd995.cn

[R45] 批量删除
来源：http://hr.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://dr.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://ut.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://su.szsharing.cn

[R47] sed 单行替换
来源：http://mi.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vm.yuexingan06.cn

[R48] awk 取指定列
来源：http://cf.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://ly.wgjwhj.cn

[R49] awk 带条件
来源：http://xl.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pt.shxzskj.cn

[R50] awk 求和
来源：http://nu.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nd.gzmigu.cn

[R51] 排序去重取前几
来源：http://xb.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sc.bookmarksfly.cn

[R52] 统计行数
来源：http://uz.shxzukj.cn

wc -l a.txt
来源：http://js.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://io.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uw.9csxet.cn

[R54] 比较两个文件
来源：http://sd.gzmigu.cn

diff a.txt b.txt
来源：http://fx.lnxyls.cn

[R55] 压缩与解压
来源：http://rx.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://la.gzmigu.cn

[R56] 远程拷贝
来源：http://lv.jianghongdianzi.cn

scp file user@host:/path/
来源：http://vp.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://hm.colortex.cn

ssh user@host 'uptime'
来源：http://em.szsharing.cn

[R58] 下载文件
来源：http://qc.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vi.yuexingan06.cn

[R59] 发 POST JSON
来源：http://no.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fu.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://ue.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gt.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://rg.asd995.cn

df -h;  du -sh *
来源：http://wo.hahajie.cn

[R62] 找最占空间的文件
来源：http://nw.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://un.colortex.cn

[R63] 内存与进程
来源：http://pw.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://ks.haigaiapp.cn

[R64] 结束进程
来源：http://cc.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://yb.wgjwhj.cn

[R65] 查看端口占用
来源：http://sv.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dl.shxzskj.cn

[R66] 定时任务
来源：http://tk.jctech888.com.cn

crontab -e;  crontab -l
来源：http://qi.521024.cn

[R67] 生成随机十六进制串
来源：http://zc.bookmarksfly.cn

openssl rand -hex 16
来源：http://hh.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://gu.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dj.newstarts.cn

[R69] 生成随机密码
来源：http://wi.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://kp.gzmigu.cn

[R70] 时间戳与互转
来源：http://ip.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://rf.szsharing.cn

[R71] 日期格式化
来源：http://bt.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uc.panjiajie.cn

[R72] 等待端口就绪
来源：http://ew.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aq.huixiangedu.cn

[R73] 分割大日志
来源：http://ud.nszjky.cn

split -l 1000 big.log part_
来源：http://cs.wgjwhj.cn

[R74] 批量重命名
来源：http://wn.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fj.hnjuh.cn

[R75] 导出环境变量
来源：http://ik.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://ev.bjjhwx.cn

[R76] 使用临时文件
来源：http://em.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hf.nicolike.cn

[R77] 读取用户输入
来源：http://nc.521024.cn

read -rp "请输入: " ans
来源：http://wt.yuexingan06.cn

[R78] 交互式菜单
来源：http://cd.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ki.shtwfgs.cn

[R79] 解析命令行选项
来源：http://bm.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xc.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://bj.shxzskj.cn

time ./run.sh
来源：http://qd.szsharing.cn

================================================================================
来源：http://sv.bookmarksfly.cn

S. C / C++ 专题
来源：http://wa.gzmigu.cn

================================================================================
来源：http://ue.bookmarksfly.cn

[S01] C：Hello World
来源：http://dn.jianghongdianzi.cn

#include <stdio.h>
来源：http://wr.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uc.colortex.cn

[S02] C：变量与格式化输出
来源：http://xz.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://kn.lnxyls.cn

[S03] C：读入整数
来源：http://ao.asd995.cn

int x; scanf("%d", &x);
来源：http://tt.shtwfgs.cn

[S04] C：字符串复制
来源：http://fw.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fa.huanxung.cn

[S05] C：字符串长度
来源：http://pd.shtwfgs.cn

strlen(s)
来源：http://qr.9csxet.cn

[S06] C：字符串比较
来源：http://sg.panjiajie.cn

strcmp(a, b) == 0
来源：http://rf.hnjuh.cn

[S07] C：数组遍历求和
来源：http://xo.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://es.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://kb.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ed.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://hb.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gq.nicolike.cn

[S10] C：指针与解引用
来源：http://hd.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://we.nicolike.cn

[S11] C：逐行读文件
来源：http://op.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://kc.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vv.gzmigu.cn

fclose(f);
来源：http://ux.gzmigu.cn

[S12] C：写文件
来源：http://db.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tt.szsharing.cn

[S13] C：宏定义
来源：http://cu.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ve.nicolike.cn

[S14] C：枚举
来源：http://az.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://pr.muxihuayi.cn

[S15] C：类型转换
来源：http://ng.nszjky.cn

(double) a / b
来源：http://fz.newstarts.cn

[S16] C：位操作置位
来源：http://ry.newstarts.cn

x |= (1 << 3);
来源：http://au.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://wi.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ca.newstarts.cn

[S18] C：命令行参数
来源：http://zu.szsharing.cn

int main(int argc, char **argv)
来源：http://eq.nszjky.cn

[S19] C：快速排序
来源：http://hr.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rz.panjiajie.cn

[S20] C：二分查找
来源：http://bu.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ab.szsharing.cn

[S21] C：字符类别判断
来源：http://bc.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kk.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://uu.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xd.huixinmuqiang.cn

[S23] C：随机数
来源：http://uk.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://za.haigaiapp.cn

[S24] C：获取本地时间
来源：http://dd.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cr.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://ns.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://ph.colortex.cn

[S26] C：内存清零
来源：http://wx.nszjky.cn

memset(a, 0, sizeof a);
来源：http://od.shxzukj.cn

[S27] C：定义常量
来源：http://cl.colortex.cn

const double PI = 3.14159;
来源：http://ax.colortex.cn

[S28] C：静态变量
来源：http://ju.colortex.cn

static int counter = 0;
来源：http://mz.shxzskj.cn

[S29] C：变参函数
来源：http://xj.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qe.nicolike.cn

[S30] C：头文件保护
来源：http://ju.szxytkj.cn

#ifndef X_H
来源：http://me.lnxyls.cn

#define X_H
来源：http://jk.shtwfgs.cn

#endif
来源：http://aj.asd995.cn

[S31] C++：Hello World
来源：http://mf.nicolike.cn

#include <iostream>
来源：http://xq.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://ns.hnjuh.cn

[S32] C++：字符串
来源：http://ft.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ch.bjjhwx.cn

[S33] C++：vector 增删
来源：http://fw.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mc.colortex.cn

[S34] C++：遍历 vector
来源：http://ld.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://bs.bookmarksfly.cn

[S35] C++：map
来源：http://eo.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fr.szsharing.cn

[S36] C++：unordered_map
来源：http://jg.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fl.lnxyls.cn

[S37] C++：set
来源：http://dc.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ll.lnxyls.cn

[S38] C++：排序
来源：http://ug.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://tt.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://nw.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xd.hahajie.cn

[S40] C++：查找元素
来源：http://kj.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vu.panjiajie.cn

[S41] C++：类与构造函数
来源：http://bk.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ur.521024.cn

[S42] C++：继承与虚函数
来源：http://si.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://ng.wgjwhj.cn

[S43] C++：智能指针
来源：http://qf.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://va.yuexingan06.cn

[S44] C++：引用传参
来源：http://rl.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://jk.shtwfgs.cn

[S45] C++：lambda
来源：http://xe.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zi.wgjwhj.cn

[S46] C++：函数模板
来源：http://nm.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://np.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://nn.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jb.nszjky.cn

[S48] C++：逐行读文件
来源：http://of.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wh.hahajie.cn

while (std::getline(in, line)) { }
来源：http://vc.521024.cn

[S49] C++：写文件
来源：http://ys.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yr.huixiangedu.cn

[S50] C++：格式化数字
来源：http://np.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qi.szxytkj.cn

[S51] C++：显式类型转换
来源：http://oj.shxzukj.cn

static_cast<double>(a) / b
来源：http://fh.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://al.asd995.cn

int size() const noexcept { return n_; }
来源：http://mg.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://kn.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://oq.szxytkj.cn

[S54] C++：异常处理
来源：http://qb.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sc.shxzskj.cn

[S55] C++：结构化绑定
来源：http://ji.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kh.chemitech.net.cn

[S56] C++：optional
来源：http://tx.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ij.jctech888.com.cn

[S57] C++：编译期常量
来源：http://fo.huanxung.cn

constexpr int N = 10;
来源：http://au.newstarts.cn

[S58] C++：命名空间
来源：http://jb.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://du.nicolike.cn

[S59] C++：静态断言
来源：http://im.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vt.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://fp.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xu.szsharing.cn

================================================================================
来源：http://cb.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zx.asd995.cn

================================================================================
来源：http://tm.asd995.cn

[T01] Kotlin：Hello World
来源：http://yk.panjiajie.cn

println("Hello")
来源：http://ut.szxytkj.cn

[T02] Kotlin：变量
来源：http://zv.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ja.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://ft.haigaiapp.cn

"值: $b"
来源：http://jd.gzmigu.cn

[T04] Kotlin：空安全
来源：http://np.newstarts.cn

val n: String? = null;  n?.length
来源：http://ff.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://gi.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://si.huanxung.cn

[T06] Kotlin：集合映射
来源：http://an.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tj.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://jy.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wz.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://je.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://ti.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://cz.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://ll.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://ru.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qf.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://vk.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dv.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://aw.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://lg.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://nj.hahajie.cn

val m = mapOf("a" to 1)
来源：http://oe.shxzskj.cn

[T14] Kotlin：循环
来源：http://lu.shxzukj.cn

for (i in 1..10) println(i)
来源：http://wa.shxzskj.cn

[T15] Kotlin：接口
来源：http://eg.9csxet.cn

interface Shape { fun area(): Double }
来源：http://fr.yuexingan06.cn

[T16] Swift：Hello World
来源：http://vp.hnjuh.cn

print("Hello")
来源：http://jj.huanxung.cn

[T17] Swift：变量与常量
来源：http://sk.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://rs.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://at.szsharing.cn

"值: \(b)"
来源：http://zd.colortex.cn

[T19] Swift：可选绑定
来源：http://dg.huanxung.cn

if let n = opt { print(n) }
来源：http://iw.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://he.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xv.newstarts.cn

[T21] Swift：遍历
来源：http://bm.lnxyls.cn

for x in a { print(x) }
来源：http://xm.huanxung.cn

[T22] Swift：字典
来源：http://pq.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ll.muxihuayi.cn

[T23] Swift：函数
来源：http://eo.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fw.haigaiapp.cn

[T24] Swift：闭包
来源：http://fo.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pb.panjiajie.cn

[T25] Swift：结构体
来源：http://yg.colortex.cn

struct P { var x: Int }
来源：http://pq.jctech888.com.cn

[T26] Swift：类与重写
来源：http://hd.szsharing.cn

class A: Base { override func f() {} }
来源：http://jh.gzmigu.cn


<!-- 参考信息 -->