代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xd.bjjhwx.cn

[R16] until 等待条件
来源：http://uh.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cj.shtwfgs.cn

[R17] 数组定义与取值
来源：http://zr.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fg.nicolike.cn

[R18] 遍历数组
来源：http://aw.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vh.szsharing.cn

[R19] 数组长度
来源：http://fj.521024.cn

echo "${#arr[@]}"
来源：http://up.hahajie.cn

[R20] 关联数组（字典）
来源：http://kz.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lm.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ym.yuexingan06.cn

echo "${#s}"
来源：http://td.huixiangedu.cn

[R22] 截取子串
来源：http://qd.hnjuh.cn

echo "${s:0:5}"
来源：http://zs.521024.cn

[R23] 字符串替换
来源：http://oj.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ru.szxytkj.cn

[R24] 大小写转换
来源：http://gm.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lr.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://jq.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lz.gzmigu.cn

[R26] 命令替换
来源：http://nb.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://qw.bookmarksfly.cn

[R27] 算术展开
来源：http://qg.9csxet.cn

echo $((1 + 2 * 3))
来源：http://rr.panjiajie.cn

[R28] 浮点运算
来源：http://kh.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://vu.huanxung.cn

[R29] 定义函数
来源：http://hp.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://db.wgjwhj.cn

[R30] 函数返回状态码
来源：http://ti.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://ty.colortex.cn

[R31] 局部变量
来源：http://mg.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://zs.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://ha.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pe.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://rt.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ht.shxzukj.cn

[R34] 退出时清理
来源：http://lt.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ry.haigaiapp.cn

[R35] 后台执行并等待
来源：http://ax.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ds.panjiajie.cn

[R36] 并发执行多个任务
来源：http://uj.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sm.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://km.huixinmuqiang.cn

files=$(ls -1)
来源：http://ui.huanxung.cn

[R38] 管道串联
来源：http://zk.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://vb.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://gj.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://tu.bookmarksfly.cn

[R40] 追加写日志
来源：http://zu.colortex.cn

echo "log" >> out.log
来源：http://oz.bjjhwx.cn

[R41] 丢弃输出
来源：http://sc.nszjky.cn

cmd >/dev/null 2>&1
来源：http://kh.asd995.cn

[R42] 输入重定向
来源：http://qr.lnxyls.cn

wc -l < a.txt
来源：http://hr.nicolike.cn

[R43] 按名字查找文件
来源：http://ug.wgjwhj.cn

find . -name "*.log" -type f
来源：http://hs.nicolike.cn

[R44] 按修改时间查找
来源：http://cy.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://jp.shxzskj.cn

[R45] 批量删除
来源：http://fw.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://pk.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://mn.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bk.wgjwhj.cn

[R47] sed 单行替换
来源：http://ch.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bx.szxytkj.cn

[R48] awk 取指定列
来源：http://at.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://mw.shtwfgs.cn

[R49] awk 带条件
来源：http://dr.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zq.muxihuayi.cn

[R50] awk 求和
来源：http://go.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rv.gzmigu.cn

[R51] 排序去重取前几
来源：http://zd.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mp.hnjuh.cn

[R52] 统计行数
来源：http://ao.nszjky.cn

wc -l a.txt
来源：http://ye.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://hq.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wf.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://iv.chemitech.net.cn

diff a.txt b.txt
来源：http://pv.szxytkj.cn

[R55] 压缩与解压
来源：http://ia.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://en.shxzukj.cn

[R56] 远程拷贝
来源：http://pu.chemitech.net.cn

scp file user@host:/path/
来源：http://on.gzmigu.cn

[R57] 远程执行命令
来源：http://an.newstarts.cn

ssh user@host 'uptime'
来源：http://rr.9csxet.cn

[R58] 下载文件
来源：http://hp.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oy.szxytkj.cn

[R59] 发 POST JSON
来源：http://cv.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ro.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://tv.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yb.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://ts.shxzskj.cn

df -h;  du -sh *
来源：http://gh.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://pp.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://dq.jctech888.com.cn

[R63] 内存与进程
来源：http://jh.colortex.cn

free -h;  ps aux | grep nginx
来源：http://zf.newstarts.cn

[R64] 结束进程
来源：http://lk.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://hy.yuexingan06.cn

[R65] 查看端口占用
来源：http://iz.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vf.muxihuayi.cn

[R66] 定时任务
来源：http://yk.lnxyls.cn

crontab -e;  crontab -l
来源：http://yz.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://zo.nicolike.cn

openssl rand -hex 16
来源：http://di.nicolike.cn

[R68] 计算文件校验值
来源：http://xe.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fe.szsharing.cn

[R69] 生成随机密码
来源：http://sf.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://jm.szxytkj.cn

[R70] 时间戳与互转
来源：http://ab.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://ox.huixinmuqiang.cn

[R71] 日期格式化
来源：http://im.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ak.shtwfgs.cn

[R72] 等待端口就绪
来源：http://hz.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bd.521024.cn

[R73] 分割大日志
来源：http://hd.nicolike.cn

split -l 1000 big.log part_
来源：http://vw.huixiangedu.cn

[R74] 批量重命名
来源：http://qb.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pa.nicolike.cn

[R75] 导出环境变量
来源：http://gs.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://di.chemitech.net.cn

[R76] 使用临时文件
来源：http://vt.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cc.bookmarksfly.cn

[R77] 读取用户输入
来源：http://jy.yuexingan06.cn

read -rp "请输入: " ans
来源：http://jr.lnxyls.cn

[R78] 交互式菜单
来源：http://ot.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ny.colortex.cn

[R79] 解析命令行选项
来源：http://kt.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pz.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://jb.newstarts.cn

time ./run.sh
来源：http://au.521024.cn

================================================================================
来源：http://xu.shtwfgs.cn

S. C / C++ 专题
来源：http://hy.hahajie.cn

================================================================================
来源：http://lk.yuexingan06.cn

[S01] C：Hello World
来源：http://mw.hahajie.cn

#include <stdio.h>
来源：http://sf.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sx.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://fl.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://xy.asd995.cn

[S03] C：读入整数
来源：http://vz.shxzskj.cn

int x; scanf("%d", &x);
来源：http://en.panjiajie.cn

[S04] C：字符串复制
来源：http://un.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://io.asd995.cn

[S05] C：字符串长度
来源：http://hl.haigaiapp.cn

strlen(s)
来源：http://pb.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://qf.nszjky.cn

strcmp(a, b) == 0
来源：http://yl.newstarts.cn

[S07] C：数组遍历求和
来源：http://xq.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://za.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://ag.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ri.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://rk.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xj.521024.cn

[S10] C：指针与解引用
来源：http://po.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://tx.yuexingan06.cn

[S11] C：逐行读文件
来源：http://kd.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://ye.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sd.huanxung.cn

fclose(f);
来源：http://ec.panjiajie.cn

[S12] C：写文件
来源：http://eq.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gv.shxzukj.cn

[S13] C：宏定义
来源：http://jm.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzmigu.cn

[S14] C：枚举
来源：http://dx.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://gb.huixiangedu.cn

[S15] C：类型转换
来源：http://pq.shtwfgs.cn

(double) a / b
来源：http://fg.gzmigu.cn

[S16] C：位操作置位
来源：http://bk.panjiajie.cn

x |= (1 << 3);
来源：http://ir.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://kd.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hb.yuexingan06.cn

[S18] C：命令行参数
来源：http://rn.521024.cn

int main(int argc, char **argv)
来源：http://ur.shxzukj.cn

[S19] C：快速排序
来源：http://tt.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vv.shtwfgs.cn

[S20] C：二分查找
来源：http://fu.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mv.newstarts.cn

[S21] C：字符类别判断
来源：http://ns.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ff.hahajie.cn

[S22] C：字符串转数字
来源：http://kp.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://es.huixinmuqiang.cn

[S23] C：随机数
来源：http://fa.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zb.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://tc.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lf.shxzskj.cn

[S25] C：内存拷贝
来源：http://xj.colortex.cn

memcpy(dst, src, n);
来源：http://db.yuexingan06.cn

[S26] C：内存清零
来源：http://xw.hahajie.cn

memset(a, 0, sizeof a);
来源：http://vh.jianghongdianzi.cn

[S27] C：定义常量
来源：http://yi.colortex.cn

const double PI = 3.14159;
来源：http://nv.yuexingan06.cn

[S28] C：静态变量
来源：http://br.muxihuayi.cn

static int counter = 0;
来源：http://wm.9csxet.cn

[S29] C：变参函数
来源：http://nt.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wf.szsharing.cn

[S30] C：头文件保护
来源：http://gn.yuntaijiaju.cn

#ifndef X_H
来源：http://ap.muxihuayi.cn

#define X_H
来源：http://yi.huixinmuqiang.cn

#endif
来源：http://zx.bjjhwx.cn

[S31] C++：Hello World
来源：http://bp.wgjwhj.cn

#include <iostream>
来源：http://lt.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://hv.jctech888.com.cn

[S32] C++：字符串
来源：http://nz.asd995.cn

std::string s = "hi";  s += "!";
来源：http://xr.shxzskj.cn

[S33] C++：vector 增删
来源：http://pi.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yi.9csxet.cn

[S34] C++：遍历 vector
来源：http://zq.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://km.jctech888.com.cn

[S35] C++：map
来源：http://cb.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ap.asd995.cn

[S36] C++：unordered_map
来源：http://nb.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mj.muxihuayi.cn

[S37] C++：set
来源：http://el.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rl.newstarts.cn

[S38] C++：排序
来源：http://fo.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://pp.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://wg.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qq.nicolike.cn

[S40] C++：查找元素
来源：http://lk.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bu.newstarts.cn

[S41] C++：类与构造函数
来源：http://py.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://to.szsharing.cn

[S42] C++：继承与虚函数
来源：http://mu.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://eb.hnjuh.cn

[S43] C++：智能指针
来源：http://oi.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://og.huanxung.cn

[S44] C++：引用传参
来源：http://vy.nicolike.cn

void inc(int &x) { ++x; }
来源：http://zo.szxytkj.cn

[S45] C++：lambda
来源：http://iz.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bu.gzmigu.cn

[S46] C++：函数模板
来源：http://wu.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qk.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://ne.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uh.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://ai.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uz.hahajie.cn

while (std::getline(in, line)) { }
来源：http://jc.colortex.cn

[S49] C++：写文件
来源：http://qc.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eq.521024.cn

[S50] C++：格式化数字
来源：http://tt.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yt.asd995.cn

[S51] C++：显式类型转换
来源：http://ax.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://dq.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://fo.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://xt.hahajie.cn

[S53] C++：移动语义
来源：http://zz.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://mp.haigaiapp.cn

[S54] C++：异常处理
来源：http://gr.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ml.panjiajie.cn

[S55] C++：结构化绑定
来源：http://ob.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nr.chemitech.net.cn

[S56] C++：optional
来源：http://qh.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nw.nicolike.cn

[S57] C++：编译期常量
来源：http://cz.huixinmuqiang.cn

constexpr int N = 10;
来源：http://bl.muxihuayi.cn

[S58] C++：命名空间
来源：http://cj.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://nn.lnxyls.cn

[S59] C++：静态断言
来源：http://dh.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zh.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://yz.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qc.521024.cn

================================================================================
来源：http://ad.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zf.jctech888.com.cn

================================================================================
来源：http://ip.hahajie.cn

[T01] Kotlin：Hello World
来源：http://ze.szxytkj.cn

println("Hello")
来源：http://sb.colortex.cn

[T02] Kotlin：变量
来源：http://ys.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fj.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://my.bookmarksfly.cn

"值: $b"
来源：http://jm.asd995.cn

[T04] Kotlin：空安全
来源：http://pm.nicolike.cn

val n: String? = null;  n?.length
来源：http://zf.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://wn.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wc.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://tl.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sc.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://tc.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xo.newstarts.cn

[T08] Kotlin：数据类
来源：http://um.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://vc.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://nh.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://fz.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://ss.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gl.521024.cn

[T11] Kotlin：协程
来源：http://gl.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ka.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://cp.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://ka.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://wx.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://rx.muxihuayi.cn

[T14] Kotlin：循环
来源：http://vg.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://nl.muxihuayi.cn

[T15] Kotlin：接口
来源：http://wn.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://wl.hnjuh.cn

[T16] Swift：Hello World
来源：http://xd.bookmarksfly.cn

print("Hello")
来源：http://wn.szxytkj.cn

[T17] Swift：变量与常量
来源：http://we.huanxung.cn

var a = 1;  let b = 2
来源：http://op.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://uz.wgjwhj.cn

"值: \(b)"
来源：http://xp.haigaiapp.cn


<!-- 参考信息 -->