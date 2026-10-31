代发 wailian999

echo "${#s}"
来源：http://mv.muxihuayi.cn

[R22] 截取子串
来源：http://tj.chemitech.net.cn

echo "${s:0:5}"
来源：http://aa.yuntaijiaju.cn

[R23] 字符串替换
来源：http://bz.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hr.jianghongdianzi.cn

[R24] 大小写转换
来源：http://fi.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://so.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://gr.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://se.lnxyls.cn

[R26] 命令替换
来源：http://rp.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://zn.szxytkj.cn

[R27] 算术展开
来源：http://cf.9csxet.cn

echo $((1 + 2 * 3))
来源：http://ka.yuexingan06.cn

[R28] 浮点运算
来源：http://hn.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://cg.lnxyls.cn

[R29] 定义函数
来源：http://as.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wt.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://di.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://no.szxytkj.cn

[R31] 局部变量
来源：http://xq.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://so.shtwfgs.cn

[R32] 参数个数校验
来源：http://xg.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pk.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://an.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qy.szsharing.cn

[R34] 退出时清理
来源：http://ap.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xb.9csxet.cn

[R35] 后台执行并等待
来源：http://un.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cb.hnjuh.cn

[R36] 并发执行多个任务
来源：http://pg.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wd.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://nz.bjjhwx.cn

files=$(ls -1)
来源：http://qx.huanxung.cn

[R38] 管道串联
来源：http://aj.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://gg.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ja.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://xl.szxytkj.cn

[R40] 追加写日志
来源：http://wh.nszjky.cn

echo "log" >> out.log
来源：http://lp.9csxet.cn

[R41] 丢弃输出
来源：http://in.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://fv.nszjky.cn

[R42] 输入重定向
来源：http://eo.hahajie.cn

wc -l < a.txt
来源：http://ev.szsharing.cn

[R43] 按名字查找文件
来源：http://vr.gzmigu.cn

find . -name "*.log" -type f
来源：http://jz.9csxet.cn

[R44] 按修改时间查找
来源：http://ex.shtwfgs.cn

find . -mtime -7 -type f
来源：http://ky.nszjky.cn

[R45] 批量删除
来源：http://dz.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://iq.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://gg.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bz.521024.cn

[R47] sed 单行替换
来源：http://ki.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mj.shtwfgs.cn

[R48] awk 取指定列
来源：http://mf.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://ry.nszjky.cn

[R49] awk 带条件
来源：http://fu.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ao.521024.cn

[R50] awk 求和
来源：http://sx.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mx.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://lp.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ao.yuntaijiaju.cn

[R52] 统计行数
来源：http://hw.muxihuayi.cn

wc -l a.txt
来源：http://lf.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://hx.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fv.nszjky.cn

[R54] 比较两个文件
来源：http://le.lnxyls.cn

diff a.txt b.txt
来源：http://nc.shxzskj.cn

[R55] 压缩与解压
来源：http://aj.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zk.muxihuayi.cn

[R56] 远程拷贝
来源：http://hc.9csxet.cn

scp file user@host:/path/
来源：http://qk.colortex.cn

[R57] 远程执行命令
来源：http://mt.gzmigu.cn

ssh user@host 'uptime'
来源：http://gy.muxihuayi.cn

[R58] 下载文件
来源：http://ga.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iu.szxytkj.cn

[R59] 发 POST JSON
来源：http://iy.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ii.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://oy.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kk.yuexingan06.cn

[R61] 磁盘占用
来源：http://yf.szxytkj.cn

df -h;  du -sh *
来源：http://wj.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://jj.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://ay.nszjky.cn

[R63] 内存与进程
来源：http://ks.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://lg.panjiajie.cn

[R64] 结束进程
来源：http://yc.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://nn.szsharing.cn

[R65] 查看端口占用
来源：http://uj.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://go.chemitech.net.cn

[R66] 定时任务
来源：http://vr.muxihuayi.cn

crontab -e;  crontab -l
来源：http://ew.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://dz.lnxyls.cn

openssl rand -hex 16
来源：http://mr.nszjky.cn

[R68] 计算文件校验值
来源：http://xh.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pb.szxytkj.cn

[R69] 生成随机密码
来源：http://tk.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://gb.panjiajie.cn

[R70] 时间戳与互转
来源：http://hz.asd995.cn

date +%s;  date -d @1700000000
来源：http://ig.9csxet.cn

[R71] 日期格式化
来源：http://bh.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yf.9csxet.cn

[R72] 等待端口就绪
来源：http://gj.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ig.muxihuayi.cn

[R73] 分割大日志
来源：http://hc.521024.cn

split -l 1000 big.log part_
来源：http://lx.lnxyls.cn

[R74] 批量重命名
来源：http://wv.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pf.asd995.cn

[R75] 导出环境变量
来源：http://xz.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://qr.muxihuayi.cn

[R76] 使用临时文件
来源：http://wv.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qv.szsharing.cn

[R77] 读取用户输入
来源：http://gi.haigaiapp.cn

read -rp "请输入: " ans
来源：http://yc.521024.cn

[R78] 交互式菜单
来源：http://db.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vk.huanxung.cn

[R79] 解析命令行选项
来源：http://yo.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yc.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://tx.newstarts.cn

time ./run.sh
来源：http://td.jianghongdianzi.cn

================================================================================
来源：http://sa.panjiajie.cn

S. C / C++ 专题
来源：http://hj.bjjhwx.cn

================================================================================
来源：http://jk.muxihuayi.cn

[S01] C：Hello World
来源：http://xh.9csxet.cn

#include <stdio.h>
来源：http://eh.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ku.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://eh.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://eg.bookmarksfly.cn

[S03] C：读入整数
来源：http://sy.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://zp.newstarts.cn

[S04] C：字符串复制
来源：http://kz.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nu.bjjhwx.cn

[S05] C：字符串长度
来源：http://gb.panjiajie.cn

strlen(s)
来源：http://zc.colortex.cn

[S06] C：字符串比较
来源：http://ga.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://dp.panjiajie.cn

[S07] C：数组遍历求和
来源：http://ef.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dv.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://xm.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yv.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://sc.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vr.asd995.cn

[S10] C：指针与解引用
来源：http://id.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://mq.szsharing.cn

[S11] C：逐行读文件
来源：http://si.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://qe.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vc.yuntaijiaju.cn

fclose(f);
来源：http://cf.yuntaijiaju.cn

[S12] C：写文件
来源：http://uu.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kp.jctech888.com.cn

[S13] C：宏定义
来源：http://pm.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rk.gzmigu.cn

[S14] C：枚举
来源：http://rq.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://kv.bjjhwx.cn

[S15] C：类型转换
来源：http://ih.muxihuayi.cn

(double) a / b
来源：http://bc.huixiangedu.cn

[S16] C：位操作置位
来源：http://uq.bjjhwx.cn

x |= (1 << 3);
来源：http://fc.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://du.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zn.szxytkj.cn

[S18] C：命令行参数
来源：http://do.huanxung.cn

int main(int argc, char **argv)
来源：http://de.lnxyls.cn

[S19] C：快速排序
来源：http://hp.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://la.shxzukj.cn

[S20] C：二分查找
来源：http://le.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wu.9csxet.cn

[S21] C：字符类别判断
来源：http://ls.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://he.newstarts.cn

[S22] C：字符串转数字
来源：http://ma.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yv.huanxung.cn

[S23] C：随机数
来源：http://oq.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ao.chemitech.net.cn

[S24] C：获取本地时间
来源：http://hv.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sn.muxihuayi.cn

[S25] C：内存拷贝
来源：http://ys.lnxyls.cn

memcpy(dst, src, n);
来源：http://ms.huixinmuqiang.cn

[S26] C：内存清零
来源：http://re.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://rn.jianghongdianzi.cn

[S27] C：定义常量
来源：http://vg.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://jw.jctech888.com.cn

[S28] C：静态变量
来源：http://ao.wgjwhj.cn

static int counter = 0;
来源：http://rx.colortex.cn

[S29] C：变参函数
来源：http://eg.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zv.9csxet.cn

[S30] C：头文件保护
来源：http://uq.asd995.cn

#ifndef X_H
来源：http://xy.yuexingan06.cn

#define X_H
来源：http://mb.hahajie.cn

#endif
来源：http://hp.colortex.cn

[S31] C++：Hello World
来源：http://gb.huanxung.cn

#include <iostream>
来源：http://oq.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://fh.nszjky.cn

[S32] C++：字符串
来源：http://xa.asd995.cn

std::string s = "hi";  s += "!";
来源：http://db.shxzskj.cn

[S33] C++：vector 增删
来源：http://wn.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mu.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://xa.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://vc.jctech888.com.cn

[S35] C++：map
来源：http://ah.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lt.panjiajie.cn

[S36] C++：unordered_map
来源：http://hj.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bz.haigaiapp.cn

[S37] C++：set
来源：http://dv.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://md.jctech888.com.cn

[S38] C++：排序
来源：http://ne.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://lu.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://ba.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sg.gzmigu.cn

[S40] C++：查找元素
来源：http://xg.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fe.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://ro.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ek.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://af.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://xd.chemitech.net.cn

[S43] C++：智能指针
来源：http://bq.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://fp.shxzukj.cn

[S44] C++：引用传参
来源：http://lm.nicolike.cn

void inc(int &x) { ++x; }
来源：http://qb.jctech888.com.cn

[S45] C++：lambda
来源：http://rt.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dg.bjjhwx.cn

[S46] C++：函数模板
来源：http://jf.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mz.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://ry.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bn.521024.cn

[S48] C++：逐行读文件
来源：http://fh.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ea.colortex.cn

while (std::getline(in, line)) { }
来源：http://ny.huanxung.cn

[S49] C++：写文件
来源：http://rg.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ts.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://rf.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nz.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://nw.huixiangedu.cn

static_cast<double>(a) / b
来源：http://vn.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://aa.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://co.gzmigu.cn

[S53] C++：移动语义
来源：http://yi.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://tj.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://ms.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uc.huanxung.cn

[S55] C++：结构化绑定
来源：http://ld.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qc.gzmigu.cn

[S56] C++：optional
来源：http://rb.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jp.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://ca.jianghongdianzi.cn

constexpr int N = 10;
来源：http://kv.nszjky.cn

[S58] C++：命名空间
来源：http://qm.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://oi.shxzukj.cn

[S59] C++：静态断言
来源：http://ph.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fk.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://la.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rn.asd995.cn

================================================================================
来源：http://dq.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zu.shxzukj.cn

================================================================================
来源：http://yf.nszjky.cn

[T01] Kotlin：Hello World
来源：http://xe.lnxyls.cn

println("Hello")
来源：http://qv.muxihuayi.cn

[T02] Kotlin：变量
来源：http://ge.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://co.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://gj.szsharing.cn

"值: $b"
来源：http://rp.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://dq.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://km.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://bo.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vf.szsharing.cn

[T06] Kotlin：集合映射
来源：http://vf.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://li.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://sh.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vw.nicolike.cn

[T08] Kotlin：数据类
来源：http://rg.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://tj.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://fm.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://sk.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ch.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xa.bjjhwx.cn

[T11] Kotlin：协程
来源：http://xb.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://co.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://rp.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://fn.521024.cn

[T13] Kotlin：只读 Map
来源：http://im.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://kv.shxzukj.cn

[T14] Kotlin：循环
来源：http://dr.panjiajie.cn

for (i in 1..10) println(i)
来源：http://dx.colortex.cn

[T15] Kotlin：接口
来源：http://vi.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://vt.shxzskj.cn

[T16] Swift：Hello World
来源：http://ke.colortex.cn

print("Hello")
来源：http://dl.hnjuh.cn

[T17] Swift：变量与常量
来源：http://in.nszjky.cn

var a = 1;  let b = 2
来源：http://qq.lnxyls.cn

[T18] Swift：字符串插值
来源：http://ab.hnjuh.cn

"值: \(b)"
来源：http://ni.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://db.hnjuh.cn

if let n = opt { print(n) }
来源：http://aa.huanxung.cn

[T20] Swift：数组操作
来源：http://gj.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tf.shxzskj.cn

[T21] Swift：遍历
来源：http://eh.wgjwhj.cn

for x in a { print(x) }
来源：http://ub.hnjuh.cn

[T22] Swift：字典
来源：http://bu.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pn.newstarts.cn

[T23] Swift：函数
来源：http://zr.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aa.huixiangedu.cn

[T24] Swift：闭包
来源：http://ct.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tl.haigaiapp.cn


<!-- 参考信息 -->