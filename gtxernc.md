代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://id.panjiajie.cn

[R16] until 等待条件
来源：http://tx.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bn.shxzukj.cn

[R17] 数组定义与取值
来源：http://xk.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hs.panjiajie.cn

[R18] 遍历数组
来源：http://kl.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dx.bookmarksfly.cn

[R19] 数组长度
来源：http://ur.lnxyls.cn

echo "${#arr[@]}"
来源：http://fz.szxytkj.cn

[R20] 关联数组（字典）
来源：http://bz.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ph.jianghongdianzi.cn

[R21] 字符串长度
来源：http://dw.shxzskj.cn

echo "${#s}"
来源：http://gs.yuntaijiaju.cn

[R22] 截取子串
来源：http://wc.bjjhwx.cn

echo "${s:0:5}"
来源：http://lt.shtwfgs.cn

[R23] 字符串替换
来源：http://zg.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ww.yuexingan06.cn

[R24] 大小写转换
来源：http://le.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zj.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://qd.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cx.521024.cn

[R26] 命令替换
来源：http://tk.521024.cn

now=$(date +%F); echo "$now"
来源：http://ld.newstarts.cn

[R27] 算术展开
来源：http://kf.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://ly.521024.cn

[R28] 浮点运算
来源：http://ek.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://xd.chemitech.net.cn

[R29] 定义函数
来源：http://tx.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uk.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://ei.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://qx.asd995.cn

[R31] 局部变量
来源：http://he.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://bh.jctech888.com.cn

[R32] 参数个数校验
来源：http://px.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pn.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://cs.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dj.shxzskj.cn

[R34] 退出时清理
来源：http://is.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://se.szxytkj.cn

[R35] 后台执行并等待
来源：http://eb.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dl.asd995.cn

[R36] 并发执行多个任务
来源：http://kz.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sq.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://wh.szsharing.cn

files=$(ls -1)
来源：http://za.huanxung.cn

[R38] 管道串联
来源：http://gg.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://ay.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://lg.panjiajie.cn

cmd > out.log 2>&1
来源：http://ig.wgjwhj.cn

[R40] 追加写日志
来源：http://is.521024.cn

echo "log" >> out.log
来源：http://qb.jctech888.com.cn

[R41] 丢弃输出
来源：http://ix.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://lb.hahajie.cn

[R42] 输入重定向
来源：http://eo.jianghongdianzi.cn

wc -l < a.txt
来源：http://lw.szxytkj.cn

[R43] 按名字查找文件
来源：http://gj.panjiajie.cn

find . -name "*.log" -type f
来源：http://fi.yuexingan06.cn

[R44] 按修改时间查找
来源：http://zw.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://ky.newstarts.cn

[R45] 批量删除
来源：http://ib.9csxet.cn

find . -name "*.tmp" -delete
来源：http://ze.hnjuh.cn

[R46] 递归替换文件内容
来源：http://dn.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dq.colortex.cn

[R47] sed 单行替换
来源：http://qw.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ye.colortex.cn

[R48] awk 取指定列
来源：http://qi.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://ju.shxzukj.cn

[R49] awk 带条件
来源：http://ev.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hv.huixiangedu.cn

[R50] awk 求和
来源：http://vc.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hr.chemitech.net.cn

[R51] 排序去重取前几
来源：http://dy.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bc.newstarts.cn

[R52] 统计行数
来源：http://pt.lnxyls.cn

wc -l a.txt
来源：http://nt.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://jv.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ad.panjiajie.cn

[R54] 比较两个文件
来源：http://gr.shxzskj.cn

diff a.txt b.txt
来源：http://ec.szxytkj.cn

[R55] 压缩与解压
来源：http://bx.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dn.bjjhwx.cn

[R56] 远程拷贝
来源：http://am.nicolike.cn

scp file user@host:/path/
来源：http://pu.9csxet.cn

[R57] 远程执行命令
来源：http://bz.haigaiapp.cn

ssh user@host 'uptime'
来源：http://oc.nicolike.cn

[R58] 下载文件
来源：http://es.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ze.lnxyls.cn

[R59] 发 POST JSON
来源：http://jl.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wq.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://ul.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://et.yuexingan06.cn

[R61] 磁盘占用
来源：http://oy.yuntaijiaju.cn

df -h;  du -sh *
来源：http://za.newstarts.cn

[R62] 找最占空间的文件
来源：http://hf.asd995.cn

du -ah . | sort -rh | head -10
来源：http://wu.szsharing.cn

[R63] 内存与进程
来源：http://lr.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://ar.shtwfgs.cn

[R64] 结束进程
来源：http://lr.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://ka.huixiangedu.cn

[R65] 查看端口占用
来源：http://vt.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wa.521024.cn

[R66] 定时任务
来源：http://dk.bjjhwx.cn

crontab -e;  crontab -l
来源：http://ie.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://uf.shxzukj.cn

openssl rand -hex 16
来源：http://li.shxzukj.cn

[R68] 计算文件校验值
来源：http://iv.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://us.shtwfgs.cn

[R69] 生成随机密码
来源：http://kd.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://nv.szsharing.cn

[R70] 时间戳与互转
来源：http://mq.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://ob.shxzukj.cn

[R71] 日期格式化
来源：http://zl.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qz.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://zl.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://om.colortex.cn

[R73] 分割大日志
来源：http://yu.szsharing.cn

split -l 1000 big.log part_
来源：http://ha.gzmigu.cn

[R74] 批量重命名
来源：http://hd.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yh.shxzskj.cn

[R75] 导出环境变量
来源：http://pn.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://az.jctech888.com.cn

[R76] 使用临时文件
来源：http://rm.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mn.bjjhwx.cn

[R77] 读取用户输入
来源：http://jq.lnxyls.cn

read -rp "请输入: " ans
来源：http://hl.shxzukj.cn

[R78] 交互式菜单
来源：http://pd.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ev.9csxet.cn

[R79] 解析命令行选项
来源：http://cf.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jl.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://yn.huanxung.cn

time ./run.sh
来源：http://fr.szsharing.cn

================================================================================
来源：http://kv.jianghongdianzi.cn

S. C / C++ 专题
来源：http://gi.bookmarksfly.cn

================================================================================
来源：http://rk.bjjhwx.cn

[S01] C：Hello World
来源：http://ar.chemitech.net.cn

#include <stdio.h>
来源：http://ul.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cg.szsharing.cn

[S02] C：变量与格式化输出
来源：http://vs.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://lv.jctech888.com.cn

[S03] C：读入整数
来源：http://wr.shxzukj.cn

int x; scanf("%d", &x);
来源：http://ur.asd995.cn

[S04] C：字符串复制
来源：http://pz.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ms.chemitech.net.cn

[S05] C：字符串长度
来源：http://yg.bjjhwx.cn

strlen(s)
来源：http://gq.bjjhwx.cn

[S06] C：字符串比较
来源：http://cl.wgjwhj.cn

strcmp(a, b) == 0
来源：http://hz.nicolike.cn

[S07] C：数组遍历求和
来源：http://ww.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ui.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://qq.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xv.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://wf.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uy.9csxet.cn

[S10] C：指针与解引用
来源：http://fa.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://yf.nicolike.cn

[S11] C：逐行读文件
来源：http://qa.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://ib.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nt.huixiangedu.cn

fclose(f);
来源：http://ej.asd995.cn

[S12] C：写文件
来源：http://mv.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bg.bookmarksfly.cn

[S13] C：宏定义
来源：http://hm.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cf.jctech888.com.cn

[S14] C：枚举
来源：http://tk.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://vb.bjjhwx.cn

[S15] C：类型转换
来源：http://ak.shtwfgs.cn

(double) a / b
来源：http://ee.shxzukj.cn

[S16] C：位操作置位
来源：http://lc.jctech888.com.cn

x |= (1 << 3);
来源：http://ih.hahajie.cn

[S17] C：安全拼接字符串
来源：http://vk.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ng.shxzukj.cn

[S18] C：命令行参数
来源：http://np.wgjwhj.cn

int main(int argc, char **argv)
来源：http://ji.wgjwhj.cn

[S19] C：快速排序
来源：http://ng.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dq.521024.cn

[S20] C：二分查找
来源：http://vn.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nd.gzmigu.cn

[S21] C：字符类别判断
来源：http://lu.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tk.lnxyls.cn

[S22] C：字符串转数字
来源：http://ks.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ns.yuntaijiaju.cn

[S23] C：随机数
来源：http://la.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bx.nicolike.cn

[S24] C：获取本地时间
来源：http://dl.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ba.haigaiapp.cn

[S25] C：内存拷贝
来源：http://bo.szxytkj.cn

memcpy(dst, src, n);
来源：http://bf.szsharing.cn

[S26] C：内存清零
来源：http://dn.colortex.cn

memset(a, 0, sizeof a);
来源：http://jc.gzmigu.cn

[S27] C：定义常量
来源：http://li.panjiajie.cn

const double PI = 3.14159;
来源：http://wv.lnxyls.cn

[S28] C：静态变量
来源：http://fg.huixinmuqiang.cn

static int counter = 0;
来源：http://zp.hnjuh.cn

[S29] C：变参函数
来源：http://jf.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xh.nszjky.cn

[S30] C：头文件保护
来源：http://cf.szxytkj.cn

#ifndef X_H
来源：http://ad.yuntaijiaju.cn

#define X_H
来源：http://my.panjiajie.cn

#endif
来源：http://cr.panjiajie.cn

[S31] C++：Hello World
来源：http://qy.shtwfgs.cn

#include <iostream>
来源：http://sz.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://jy.chemitech.net.cn

[S32] C++：字符串
来源：http://en.colortex.cn

std::string s = "hi";  s += "!";
来源：http://tx.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://ij.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xe.asd995.cn

[S34] C++：遍历 vector
来源：http://dn.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://nz.nicolike.cn

[S35] C++：map
来源：http://do.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wn.muxihuayi.cn

[S36] C++：unordered_map
来源：http://or.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bo.nszjky.cn

[S37] C++：set
来源：http://ft.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jk.shxzukj.cn

[S38] C++：排序
来源：http://wb.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://gx.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://mj.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gw.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://ik.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vy.panjiajie.cn

[S41] C++：类与构造函数
来源：http://rf.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eh.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://zx.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://rl.hahajie.cn

[S43] C++：智能指针
来源：http://ww.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://oc.shxzskj.cn

[S44] C++：引用传参
来源：http://bi.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://mh.hahajie.cn

[S45] C++：lambda
来源：http://fa.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dp.lnxyls.cn

[S46] C++：函数模板
来源：http://gd.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qt.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://nt.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dy.hahajie.cn

[S48] C++：逐行读文件
来源：http://jf.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yq.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://dh.lnxyls.cn

[S49] C++：写文件
来源：http://tp.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ps.521024.cn

[S50] C++：格式化数字
来源：http://dz.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xu.szsharing.cn

[S51] C++：显式类型转换
来源：http://yk.wgjwhj.cn

static_cast<double>(a) / b
来源：http://fq.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://ce.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://rp.hahajie.cn

[S53] C++：移动语义
来源：http://do.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://fp.bookmarksfly.cn

[S54] C++：异常处理
来源：http://kk.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gh.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://lq.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xr.bookmarksfly.cn

[S56] C++：optional
来源：http://gg.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mi.shxzukj.cn

[S57] C++：编译期常量
来源：http://an.hahajie.cn

constexpr int N = 10;
来源：http://wj.chemitech.net.cn

[S58] C++：命名空间
来源：http://lv.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://rj.yuexingan06.cn

[S59] C++：静态断言
来源：http://ld.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://az.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://lv.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zu.szsharing.cn

================================================================================
来源：http://vx.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jb.9csxet.cn

================================================================================
来源：http://qi.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://ly.chemitech.net.cn

println("Hello")
来源：http://rc.panjiajie.cn

[T02] Kotlin：变量
来源：http://ob.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ic.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://lr.nszjky.cn

"值: $b"
来源：http://kr.gzmigu.cn

[T04] Kotlin：空安全
来源：http://rn.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://ze.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://qd.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.newstarts.cn

[T06] Kotlin：集合映射
来源：http://ri.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ad.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://sn.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yy.hahajie.cn

[T08] Kotlin：数据类
来源：http://bx.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://sv.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://ez.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://gu.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://il.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pn.panjiajie.cn

[T11] Kotlin：协程
来源：http://ai.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mh.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://bd.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://lg.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://on.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://xh.colortex.cn

[T14] Kotlin：循环
来源：http://qs.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://kt.panjiajie.cn

[T15] Kotlin：接口
来源：http://ue.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://zo.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://dz.wgjwhj.cn

print("Hello")
来源：http://he.hnjuh.cn

[T17] Swift：变量与常量
来源：http://wu.bjjhwx.cn

var a = 1;  let b = 2
来源：http://vh.gzmigu.cn

[T18] Swift：字符串插值
来源：http://nn.wgjwhj.cn

"值: \(b)"
来源：http://yy.huanxung.cn


<!-- 参考信息 -->