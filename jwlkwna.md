代发 wailian999

echo "${#arr[@]}"
来源：http://pi.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://qr.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://az.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ob.shtwfgs.cn

echo "${#s}"
来源：http://vp.haigaiapp.cn

[R22] 截取子串
来源：http://eq.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://nh.asd995.cn

[R23] 字符串替换
来源：http://lk.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rn.jctech888.com.cn

[R24] 大小写转换
来源：http://eq.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zh.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://lu.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hh.asd995.cn

[R26] 命令替换
来源：http://ar.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://mj.newstarts.cn

[R27] 算术展开
来源：http://xk.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://si.bjjhwx.cn

[R28] 浮点运算
来源：http://wa.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://jt.newstarts.cn

[R29] 定义函数
来源：http://ne.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lf.nszjky.cn

[R30] 函数返回状态码
来源：http://sg.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://sn.huixinmuqiang.cn

[R31] 局部变量
来源：http://fy.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://na.nszjky.cn

[R32] 参数个数校验
来源：http://db.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kh.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://mm.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sr.shxzukj.cn

[R34] 退出时清理
来源：http://of.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qu.szxytkj.cn

[R35] 后台执行并等待
来源：http://zs.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yw.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://av.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tu.hnjuh.cn

[R37] 把输出赋给变量
来源：http://yi.hnjuh.cn

files=$(ls -1)
来源：http://bj.muxihuayi.cn

[R38] 管道串联
来源：http://yp.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://oe.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://ek.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://ks.huixiangedu.cn

[R40] 追加写日志
来源：http://yz.huanxung.cn

echo "log" >> out.log
来源：http://hk.nicolike.cn

[R41] 丢弃输出
来源：http://dt.hahajie.cn

cmd >/dev/null 2>&1
来源：http://nb.huixinmuqiang.cn

[R42] 输入重定向
来源：http://bk.asd995.cn

wc -l < a.txt
来源：http://vu.panjiajie.cn

[R43] 按名字查找文件
来源：http://yb.chemitech.net.cn

find . -name "*.log" -type f
来源：http://uk.yuexingan06.cn

[R44] 按修改时间查找
来源：http://gl.shxzukj.cn

find . -mtime -7 -type f
来源：http://jx.hnjuh.cn

[R45] 批量删除
来源：http://ep.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://vk.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://zl.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rj.bjjhwx.cn

[R47] sed 单行替换
来源：http://bj.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pg.nszjky.cn

[R48] awk 取指定列
来源：http://kk.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://eh.nicolike.cn

[R49] awk 带条件
来源：http://nj.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xn.shxzskj.cn

[R50] awk 求和
来源：http://la.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zw.shxzukj.cn

[R51] 排序去重取前几
来源：http://sh.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zx.huixinmuqiang.cn

[R52] 统计行数
来源：http://bv.asd995.cn

wc -l a.txt
来源：http://oy.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://bo.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ro.newstarts.cn

[R54] 比较两个文件
来源：http://ds.szsharing.cn

diff a.txt b.txt
来源：http://ew.hahajie.cn

[R55] 压缩与解压
来源：http://uc.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hb.gzmigu.cn

[R56] 远程拷贝
来源：http://ld.lnxyls.cn

scp file user@host:/path/
来源：http://ej.muxihuayi.cn

[R57] 远程执行命令
来源：http://ec.huanxung.cn

ssh user@host 'uptime'
来源：http://pm.haigaiapp.cn

[R58] 下载文件
来源：http://ba.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nh.lnxyls.cn

[R59] 发 POST JSON
来源：http://if.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://un.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://xs.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kp.wgjwhj.cn

[R61] 磁盘占用
来源：http://he.haigaiapp.cn

df -h;  du -sh *
来源：http://fr.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://pe.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://vy.asd995.cn

[R63] 内存与进程
来源：http://si.colortex.cn

free -h;  ps aux | grep nginx
来源：http://ob.szsharing.cn

[R64] 结束进程
来源：http://aw.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://rj.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://qc.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zr.szxytkj.cn

[R66] 定时任务
来源：http://gf.521024.cn

crontab -e;  crontab -l
来源：http://xl.hahajie.cn

[R67] 生成随机十六进制串
来源：http://fg.nszjky.cn

openssl rand -hex 16
来源：http://yi.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://xg.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jl.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://gu.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://nv.newstarts.cn

[R70] 时间戳与互转
来源：http://pe.9csxet.cn

date +%s;  date -d @1700000000
来源：http://lh.shtwfgs.cn

[R71] 日期格式化
来源：http://zc.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dn.shxzskj.cn

[R72] 等待端口就绪
来源：http://ho.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://su.panjiajie.cn

[R73] 分割大日志
来源：http://wi.gzmigu.cn

split -l 1000 big.log part_
来源：http://sk.9csxet.cn

[R74] 批量重命名
来源：http://gf.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rl.jctech888.com.cn

[R75] 导出环境变量
来源：http://ul.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://hs.nicolike.cn

[R76] 使用临时文件
来源：http://us.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ys.521024.cn

[R77] 读取用户输入
来源：http://yk.szxytkj.cn

read -rp "请输入: " ans
来源：http://ad.newstarts.cn

[R78] 交互式菜单
来源：http://ef.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cu.szsharing.cn

[R79] 解析命令行选项
来源：http://jg.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sc.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://mc.szxytkj.cn

time ./run.sh
来源：http://dt.hahajie.cn

================================================================================
来源：http://xd.colortex.cn

S. C / C++ 专题
来源：http://ep.yuntaijiaju.cn

================================================================================
来源：http://wc.nszjky.cn

[S01] C：Hello World
来源：http://qc.shxzukj.cn

#include <stdio.h>
来源：http://ph.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kc.521024.cn

[S02] C：变量与格式化输出
来源：http://ko.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://ru.nszjky.cn

[S03] C：读入整数
来源：http://bq.hahajie.cn

int x; scanf("%d", &x);
来源：http://ro.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://fe.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rq.huixiangedu.cn

[S05] C：字符串长度
来源：http://mw.nszjky.cn

strlen(s)
来源：http://ro.haigaiapp.cn

[S06] C：字符串比较
来源：http://bb.bjjhwx.cn

strcmp(a, b) == 0
来源：http://zs.9csxet.cn

[S07] C：数组遍历求和
来源：http://rv.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fr.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://ec.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zs.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://uk.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pf.lnxyls.cn

[S10] C：指针与解引用
来源：http://hp.9csxet.cn

int *p = &a;  *p = 5;
来源：http://to.huanxung.cn

[S11] C：逐行读文件
来源：http://pc.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://xx.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://br.szxytkj.cn

fclose(f);
来源：http://iz.asd995.cn

[S12] C：写文件
来源：http://ox.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kc.521024.cn

[S13] C：宏定义
来源：http://dp.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pz.huanxung.cn

[S14] C：枚举
来源：http://dg.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://co.nszjky.cn

[S15] C：类型转换
来源：http://po.9csxet.cn

(double) a / b
来源：http://zj.chemitech.net.cn

[S16] C：位操作置位
来源：http://tj.gzmigu.cn

x |= (1 << 3);
来源：http://gv.asd995.cn

[S17] C：安全拼接字符串
来源：http://rm.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mv.newstarts.cn

[S18] C：命令行参数
来源：http://ok.huixiangedu.cn

int main(int argc, char **argv)
来源：http://pq.hnjuh.cn

[S19] C：快速排序
来源：http://ao.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qf.jctech888.com.cn

[S20] C：二分查找
来源：http://ry.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vp.bjjhwx.cn

[S21] C：字符类别判断
来源：http://po.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ux.asd995.cn

[S22] C：字符串转数字
来源：http://ju.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://it.bookmarksfly.cn

[S23] C：随机数
来源：http://xr.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qz.panjiajie.cn

[S24] C：获取本地时间
来源：http://ds.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://az.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://hj.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://mc.bjjhwx.cn

[S26] C：内存清零
来源：http://ux.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://cp.jianghongdianzi.cn

[S27] C：定义常量
来源：http://ag.huixiangedu.cn

const double PI = 3.14159;
来源：http://iv.shxzskj.cn

[S28] C：静态变量
来源：http://bi.panjiajie.cn

static int counter = 0;
来源：http://cv.haigaiapp.cn

[S29] C：变参函数
来源：http://mo.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iw.hahajie.cn

[S30] C：头文件保护
来源：http://ku.huixinmuqiang.cn

#ifndef X_H
来源：http://ts.szsharing.cn

#define X_H
来源：http://my.haigaiapp.cn

#endif
来源：http://ta.wgjwhj.cn

[S31] C++：Hello World
来源：http://wp.bjjhwx.cn

#include <iostream>
来源：http://ex.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://hd.colortex.cn

[S32] C++：字符串
来源：http://ir.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://fd.bjjhwx.cn

[S33] C++：vector 增删
来源：http://wt.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sd.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://zo.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://eq.lnxyls.cn

[S35] C++：map
来源：http://ld.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zj.hnjuh.cn

[S36] C++：unordered_map
来源：http://xj.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qi.hnjuh.cn

[S37] C++：set
来源：http://rh.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ew.yuntaijiaju.cn

[S38] C++：排序
来源：http://iw.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://rn.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://ll.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gu.shtwfgs.cn

[S40] C++：查找元素
来源：http://jb.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://be.shxzukj.cn

[S41] C++：类与构造函数
来源：http://jd.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cu.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://dq.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ql.shxzukj.cn

[S43] C++：智能指针
来源：http://nc.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://gr.hnjuh.cn

[S44] C++：引用传参
来源：http://kl.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://ky.shtwfgs.cn

[S45] C++：lambda
来源：http://yl.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://td.shxzukj.cn

[S46] C++：函数模板
来源：http://bw.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sf.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://vp.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lb.shxzukj.cn

[S48] C++：逐行读文件
来源：http://zk.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ui.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://wm.lnxyls.cn

[S49] C++：写文件
来源：http://zl.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fe.muxihuayi.cn

[S50] C++：格式化数字
来源：http://jm.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qx.asd995.cn

[S51] C++：显式类型转换
来源：http://bv.szxytkj.cn

static_cast<double>(a) / b
来源：http://hr.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://qw.newstarts.cn

int size() const noexcept { return n_; }
来源：http://ew.shtwfgs.cn

[S53] C++：移动语义
来源：http://sm.521024.cn

std::vector<int> w = std::move(v);
来源：http://dd.hahajie.cn

[S54] C++：异常处理
来源：http://li.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ba.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://ud.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hm.huixiangedu.cn

[S56] C++：optional
来源：http://ym.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pr.szxytkj.cn

[S57] C++：编译期常量
来源：http://lg.lnxyls.cn

constexpr int N = 10;
来源：http://ca.yuexingan06.cn

[S58] C++：命名空间
来源：http://kv.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://ag.panjiajie.cn

[S59] C++：静态断言
来源：http://kf.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rn.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://yw.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pi.haigaiapp.cn

================================================================================
来源：http://vt.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zr.hahajie.cn

================================================================================
来源：http://yp.nicolike.cn

[T01] Kotlin：Hello World
来源：http://it.chemitech.net.cn

println("Hello")
来源：http://kk.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://yh.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bx.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://lz.lnxyls.cn

"值: $b"
来源：http://at.newstarts.cn

[T04] Kotlin：空安全
来源：http://cc.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://ma.asd995.cn

[T05] Kotlin：when 表达式
来源：http://dk.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dg.nszjky.cn

[T06] Kotlin：集合映射
来源：http://rm.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ct.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://iw.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rh.colortex.cn

[T08] Kotlin：数据类
来源：http://vd.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://tl.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://jf.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://uf.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://vz.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cd.muxihuayi.cn

[T11] Kotlin：协程
来源：http://sm.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://db.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://mq.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://hg.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://iw.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://zz.shxzskj.cn

[T14] Kotlin：循环
来源：http://ik.hnjuh.cn

for (i in 1..10) println(i)
来源：http://au.wgjwhj.cn

[T15] Kotlin：接口
来源：http://to.szsharing.cn

interface Shape { fun area(): Double }
来源：http://rt.huixiangedu.cn

[T16] Swift：Hello World
来源：http://im.lnxyls.cn

print("Hello")
来源：http://tm.szxytkj.cn

[T17] Swift：变量与常量
来源：http://lz.chemitech.net.cn

var a = 1;  let b = 2
来源：http://ed.gzmigu.cn

[T18] Swift：字符串插值
来源：http://tn.hnjuh.cn

"值: \(b)"
来源：http://zo.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://ru.jctech888.com.cn

if let n = opt { print(n) }
来源：http://rl.hnjuh.cn

[T20] Swift：数组操作
来源：http://rg.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://it.nszjky.cn

[T21] Swift：遍历
来源：http://ex.bjjhwx.cn

for x in a { print(x) }
来源：http://wd.hahajie.cn

[T22] Swift：字典
来源：http://sd.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uo.huixinmuqiang.cn


<!-- 参考信息 -->