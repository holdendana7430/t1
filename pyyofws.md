代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ng.gzmigu.cn

[R16] until 等待条件
来源：http://uo.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bq.huanxung.cn

[R17] 数组定义与取值
来源：http://bu.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vr.nicolike.cn

[R18] 遍历数组
来源：http://mm.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sl.bookmarksfly.cn

[R19] 数组长度
来源：http://ej.bjjhwx.cn

echo "${#arr[@]}"
来源：http://xz.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://gu.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wp.shxzukj.cn

[R21] 字符串长度
来源：http://ir.yuexingan06.cn

echo "${#s}"
来源：http://os.bjjhwx.cn

[R22] 截取子串
来源：http://gk.huanxung.cn

echo "${s:0:5}"
来源：http://us.shxzukj.cn

[R23] 字符串替换
来源：http://hz.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oj.yuexingan06.cn

[R24] 大小写转换
来源：http://oc.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kg.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://do.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ew.colortex.cn

[R26] 命令替换
来源：http://mu.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://fr.shxzskj.cn

[R27] 算术展开
来源：http://ck.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://ut.huanxung.cn

[R28] 浮点运算
来源：http://tg.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://tv.yuntaijiaju.cn

[R29] 定义函数
来源：http://om.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ip.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://ao.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ub.muxihuayi.cn

[R31] 局部变量
来源：http://bz.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://du.yuexingan06.cn

[R32] 参数个数校验
来源：http://fl.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pk.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://nt.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ho.jianghongdianzi.cn

[R34] 退出时清理
来源：http://lg.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bs.panjiajie.cn

[R35] 后台执行并等待
来源：http://rh.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pg.nszjky.cn

[R36] 并发执行多个任务
来源：http://nc.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dg.lnxyls.cn

[R37] 把输出赋给变量
来源：http://hx.huanxung.cn

files=$(ls -1)
来源：http://aj.bjjhwx.cn

[R38] 管道串联
来源：http://qu.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://kd.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://pk.yuexingan06.cn

cmd > out.log 2>&1
来源：http://qg.shxzukj.cn

[R40] 追加写日志
来源：http://um.szxytkj.cn

echo "log" >> out.log
来源：http://vz.newstarts.cn

[R41] 丢弃输出
来源：http://fi.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://ws.lnxyls.cn

[R42] 输入重定向
来源：http://uu.wgjwhj.cn

wc -l < a.txt
来源：http://jq.szxytkj.cn

[R43] 按名字查找文件
来源：http://nj.yuexingan06.cn

find . -name "*.log" -type f
来源：http://ch.nszjky.cn

[R44] 按修改时间查找
来源：http://pa.hahajie.cn

find . -mtime -7 -type f
来源：http://pw.huixinmuqiang.cn

[R45] 批量删除
来源：http://zu.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://cm.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://ue.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iu.gzmigu.cn

[R47] sed 单行替换
来源：http://tb.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pj.muxihuayi.cn

[R48] awk 取指定列
来源：http://gl.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://js.chemitech.net.cn

[R49] awk 带条件
来源：http://gj.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gp.521024.cn

[R50] awk 求和
来源：http://vn.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vs.colortex.cn

[R51] 排序去重取前几
来源：http://yq.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vi.bookmarksfly.cn

[R52] 统计行数
来源：http://wq.muxihuayi.cn

wc -l a.txt
来源：http://kh.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://sh.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xj.newstarts.cn

[R54] 比较两个文件
来源：http://jb.yuexingan06.cn

diff a.txt b.txt
来源：http://pq.521024.cn

[R55] 压缩与解压
来源：http://fc.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pz.szsharing.cn

[R56] 远程拷贝
来源：http://cu.shtwfgs.cn

scp file user@host:/path/
来源：http://rh.newstarts.cn

[R57] 远程执行命令
来源：http://hx.hahajie.cn

ssh user@host 'uptime'
来源：http://oh.shtwfgs.cn

[R58] 下载文件
来源：http://ba.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pk.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://ru.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xm.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://pt.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://db.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://ht.hnjuh.cn

df -h;  du -sh *
来源：http://hd.szxytkj.cn

[R62] 找最占空间的文件
来源：http://ze.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://ty.wgjwhj.cn

[R63] 内存与进程
来源：http://xy.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://hb.521024.cn

[R64] 结束进程
来源：http://hc.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://im.szxytkj.cn

[R65] 查看端口占用
来源：http://yb.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sm.newstarts.cn

[R66] 定时任务
来源：http://eu.shtwfgs.cn

crontab -e;  crontab -l
来源：http://de.szsharing.cn

[R67] 生成随机十六进制串
来源：http://zm.shtwfgs.cn

openssl rand -hex 16
来源：http://ft.colortex.cn

[R68] 计算文件校验值
来源：http://da.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oa.colortex.cn

[R69] 生成随机密码
来源：http://cp.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ew.szxytkj.cn

[R70] 时间戳与互转
来源：http://wl.nicolike.cn

date +%s;  date -d @1700000000
来源：http://sw.chemitech.net.cn

[R71] 日期格式化
来源：http://am.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uy.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://ap.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fj.szxytkj.cn

[R73] 分割大日志
来源：http://py.asd995.cn

split -l 1000 big.log part_
来源：http://io.bjjhwx.cn

[R74] 批量重命名
来源：http://me.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gn.nicolike.cn

[R75] 导出环境变量
来源：http://vj.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://nj.colortex.cn

[R76] 使用临时文件
来源：http://xy.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://in.wgjwhj.cn

[R77] 读取用户输入
来源：http://gz.yuexingan06.cn

read -rp "请输入: " ans
来源：http://wq.szxytkj.cn

[R78] 交互式菜单
来源：http://us.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sg.huanxung.cn

[R79] 解析命令行选项
来源：http://ty.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nn.colortex.cn

[R80] 查看脚本执行耗时
来源：http://xr.panjiajie.cn

time ./run.sh
来源：http://xe.521024.cn

================================================================================
来源：http://bi.521024.cn

S. C / C++ 专题
来源：http://kk.yuntaijiaju.cn

================================================================================
来源：http://fj.521024.cn

[S01] C：Hello World
来源：http://ei.wgjwhj.cn

#include <stdio.h>
来源：http://jv.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ru.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://mc.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://fd.shxzskj.cn

[S03] C：读入整数
来源：http://dp.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://ct.lnxyls.cn

[S04] C：字符串复制
来源：http://fx.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hm.hnjuh.cn

[S05] C：字符串长度
来源：http://oa.yuexingan06.cn

strlen(s)
来源：http://ao.chemitech.net.cn

[S06] C：字符串比较
来源：http://lt.newstarts.cn

strcmp(a, b) == 0
来源：http://qi.gzmigu.cn

[S07] C：数组遍历求和
来源：http://wv.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aj.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://ya.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://um.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://jn.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://to.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://io.szsharing.cn

int *p = &a;  *p = 5;
来源：http://ze.shxzskj.cn

[S11] C：逐行读文件
来源：http://id.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://tl.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ot.9csxet.cn

fclose(f);
来源：http://ri.muxihuayi.cn

[S12] C：写文件
来源：http://po.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tz.521024.cn

[S13] C：宏定义
来源：http://ou.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rs.huixiangedu.cn

[S14] C：枚举
来源：http://ic.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://ur.hnjuh.cn

[S15] C：类型转换
来源：http://vy.hahajie.cn

(double) a / b
来源：http://ez.szsharing.cn

[S16] C：位操作置位
来源：http://cv.jctech888.com.cn

x |= (1 << 3);
来源：http://ym.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://ez.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fc.colortex.cn

[S18] C：命令行参数
来源：http://zz.shtwfgs.cn

int main(int argc, char **argv)
来源：http://px.bjjhwx.cn

[S19] C：快速排序
来源：http://kb.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sa.huixinmuqiang.cn

[S20] C：二分查找
来源：http://nk.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oz.szxytkj.cn

[S21] C：字符类别判断
来源：http://co.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xs.panjiajie.cn

[S22] C：字符串转数字
来源：http://bh.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gt.shxzukj.cn

[S23] C：随机数
来源：http://fa.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mc.gzmigu.cn

[S24] C：获取本地时间
来源：http://kd.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qz.9csxet.cn

[S25] C：内存拷贝
来源：http://mn.huanxung.cn

memcpy(dst, src, n);
来源：http://sm.bookmarksfly.cn

[S26] C：内存清零
来源：http://aw.szsharing.cn

memset(a, 0, sizeof a);
来源：http://ew.521024.cn

[S27] C：定义常量
来源：http://ln.huanxung.cn

const double PI = 3.14159;
来源：http://bh.shxzskj.cn

[S28] C：静态变量
来源：http://fd.colortex.cn

static int counter = 0;
来源：http://oc.huixinmuqiang.cn

[S29] C：变参函数
来源：http://ll.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ll.nicolike.cn

[S30] C：头文件保护
来源：http://vy.wgjwhj.cn

#ifndef X_H
来源：http://ls.shxzskj.cn

#define X_H
来源：http://sl.huanxung.cn

#endif
来源：http://mg.gzmigu.cn

[S31] C++：Hello World
来源：http://cf.shtwfgs.cn

#include <iostream>
来源：http://pf.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://ho.szxytkj.cn

[S32] C++：字符串
来源：http://qv.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://kl.szsharing.cn

[S33] C++：vector 增删
来源：http://iu.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://op.gzmigu.cn

[S34] C++：遍历 vector
来源：http://eg.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://ua.newstarts.cn

[S35] C++：map
来源：http://wj.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pi.bjjhwx.cn

[S36] C++：unordered_map
来源：http://lu.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qe.yuntaijiaju.cn

[S37] C++：set
来源：http://od.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ud.jianghongdianzi.cn

[S38] C++：排序
来源：http://fc.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://gd.asd995.cn

[S39] C++：自定义比较器排序
来源：http://oq.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xm.panjiajie.cn

[S40] C++：查找元素
来源：http://db.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xd.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://qi.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://om.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://zr.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://qo.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://ap.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://wk.shxzskj.cn

[S44] C++：引用传参
来源：http://ay.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://mk.gzmigu.cn

[S45] C++：lambda
来源：http://pt.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dl.panjiajie.cn

[S46] C++：函数模板
来源：http://zq.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sw.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://zl.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jh.nszjky.cn

[S48] C++：逐行读文件
来源：http://ob.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hu.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://yw.nicolike.cn

[S49] C++：写文件
来源：http://tq.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ki.szxytkj.cn

[S50] C++：格式化数字
来源：http://vw.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://do.nszjky.cn

[S51] C++：显式类型转换
来源：http://gc.muxihuayi.cn

static_cast<double>(a) / b
来源：http://bm.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://oy.szsharing.cn

int size() const noexcept { return n_; }
来源：http://xp.newstarts.cn

[S53] C++：移动语义
来源：http://zl.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://dq.bjjhwx.cn

[S54] C++：异常处理
来源：http://xo.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wp.colortex.cn

[S55] C++：结构化绑定
来源：http://ss.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://un.bookmarksfly.cn

[S56] C++：optional
来源：http://qx.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wc.gzmigu.cn

[S57] C++：编译期常量
来源：http://ep.colortex.cn

constexpr int N = 10;
来源：http://xo.hahajie.cn

[S58] C++：命名空间
来源：http://lw.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://cu.shtwfgs.cn

[S59] C++：静态断言
来源：http://fl.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vj.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://zf.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://as.jctech888.com.cn

================================================================================
来源：http://sm.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ki.colortex.cn

================================================================================
来源：http://pk.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://rj.hnjuh.cn

println("Hello")
来源：http://dx.huanxung.cn

[T02] Kotlin：变量
来源：http://wb.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sa.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://lw.huixinmuqiang.cn

"值: $b"
来源：http://gb.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://tz.shxzskj.cn

val n: String? = null;  n?.length
来源：http://hn.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://jg.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sr.asd995.cn

[T06] Kotlin：集合映射
来源：http://yl.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tp.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://mb.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jg.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://td.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://oz.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://jp.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://gy.asd995.cn

[T10] Kotlin：默认参数
来源：http://sm.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://km.asd995.cn

[T11] Kotlin：协程
来源：http://wh.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ft.9csxet.cn

[T12] Kotlin：解构声明
来源：http://un.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://wx.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://ok.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://ka.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://xo.asd995.cn

for (i in 1..10) println(i)
来源：http://pw.chemitech.net.cn

[T15] Kotlin：接口
来源：http://gy.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://oc.shtwfgs.cn

[T16] Swift：Hello World
来源：http://sr.szsharing.cn

print("Hello")
来源：http://gn.hnjuh.cn

[T17] Swift：变量与常量
来源：http://af.szsharing.cn

var a = 1;  let b = 2
来源：http://jd.hahajie.cn

[T18] Swift：字符串插值
来源：http://os.haigaiapp.cn

"值: \(b)"
来源：http://vw.panjiajie.cn


<!-- 参考信息 -->