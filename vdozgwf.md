代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://jq.newstarts.cn

[R14] C 风格 for
来源：http://ya.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gi.hnjuh.cn

[R15] while 逐行读文件
来源：http://nv.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pt.shxzukj.cn

[R16] until 等待条件
来源：http://la.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wq.shtwfgs.cn

[R17] 数组定义与取值
来源：http://dk.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jl.huanxung.cn

[R18] 遍历数组
来源：http://la.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rq.bjjhwx.cn

[R19] 数组长度
来源：http://yh.nszjky.cn

echo "${#arr[@]}"
来源：http://xd.9csxet.cn

[R20] 关联数组（字典）
来源：http://lc.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jf.gzmigu.cn

[R21] 字符串长度
来源：http://om.colortex.cn

echo "${#s}"
来源：http://nx.huanxung.cn

[R22] 截取子串
来源：http://iw.yuexingan06.cn

echo "${s:0:5}"
来源：http://tq.hahajie.cn

[R23] 字符串替换
来源：http://vd.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yj.shxzskj.cn

[R24] 大小写转换
来源：http://by.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xh.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://sa.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tl.yuexingan06.cn

[R26] 命令替换
来源：http://fl.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://cw.chemitech.net.cn

[R27] 算术展开
来源：http://eh.huanxung.cn

echo $((1 + 2 * 3))
来源：http://ch.huixinmuqiang.cn

[R28] 浮点运算
来源：http://ht.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://to.lnxyls.cn

[R29] 定义函数
来源：http://qb.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dc.panjiajie.cn

[R30] 函数返回状态码
来源：http://id.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://nj.huixiangedu.cn

[R31] 局部变量
来源：http://fj.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://od.lnxyls.cn

[R32] 参数个数校验
来源：http://vj.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gc.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://fp.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fs.jctech888.com.cn

[R34] 退出时清理
来源：http://yp.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ri.muxihuayi.cn

[R35] 后台执行并等待
来源：http://cf.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bv.panjiajie.cn

[R36] 并发执行多个任务
来源：http://ly.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uu.nszjky.cn

[R37] 把输出赋给变量
来源：http://qm.huixiangedu.cn

files=$(ls -1)
来源：http://wl.huanxung.cn

[R38] 管道串联
来源：http://lr.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://ag.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://oa.wgjwhj.cn

cmd > out.log 2>&1
来源：http://at.asd995.cn

[R40] 追加写日志
来源：http://up.huanxung.cn

echo "log" >> out.log
来源：http://vt.gzmigu.cn

[R41] 丢弃输出
来源：http://lr.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://cj.yuexingan06.cn

[R42] 输入重定向
来源：http://gu.521024.cn

wc -l < a.txt
来源：http://gx.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://vm.bjjhwx.cn

find . -name "*.log" -type f
来源：http://cr.521024.cn

[R44] 按修改时间查找
来源：http://yw.huanxung.cn

find . -mtime -7 -type f
来源：http://ct.hnjuh.cn

[R45] 批量删除
来源：http://oo.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://wp.szsharing.cn

[R46] 递归替换文件内容
来源：http://eu.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ag.muxihuayi.cn

[R47] sed 单行替换
来源：http://le.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kq.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://su.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://ga.panjiajie.cn

[R49] awk 带条件
来源：http://ar.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ve.jianghongdianzi.cn

[R50] awk 求和
来源：http://ex.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xq.haigaiapp.cn

[R51] 排序去重取前几
来源：http://pb.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gq.jianghongdianzi.cn

[R52] 统计行数
来源：http://xm.chemitech.net.cn

wc -l a.txt
来源：http://am.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://oj.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fy.newstarts.cn

[R54] 比较两个文件
来源：http://gt.huixinmuqiang.cn

diff a.txt b.txt
来源：http://gn.panjiajie.cn

[R55] 压缩与解压
来源：http://op.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vy.bjjhwx.cn

[R56] 远程拷贝
来源：http://av.shtwfgs.cn

scp file user@host:/path/
来源：http://we.jctech888.com.cn

[R57] 远程执行命令
来源：http://oe.hnjuh.cn

ssh user@host 'uptime'
来源：http://xw.huixinmuqiang.cn

[R58] 下载文件
来源：http://gs.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vz.lnxyls.cn

[R59] 发 POST JSON
来源：http://eq.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vr.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://yl.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://im.haigaiapp.cn

[R61] 磁盘占用
来源：http://ek.shtwfgs.cn

df -h;  du -sh *
来源：http://bm.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://kz.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://sk.nszjky.cn

[R63] 内存与进程
来源：http://ts.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://fy.yuexingan06.cn

[R64] 结束进程
来源：http://qp.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://kz.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://us.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yt.yuexingan06.cn

[R66] 定时任务
来源：http://sr.colortex.cn

crontab -e;  crontab -l
来源：http://ne.newstarts.cn

[R67] 生成随机十六进制串
来源：http://ae.wgjwhj.cn

openssl rand -hex 16
来源：http://tc.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://dd.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ec.wgjwhj.cn

[R69] 生成随机密码
来源：http://je.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://rv.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://bc.colortex.cn

date +%s;  date -d @1700000000
来源：http://cp.huanxung.cn

[R71] 日期格式化
来源：http://zw.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gk.huixiangedu.cn

[R72] 等待端口就绪
来源：http://fz.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gt.huixinmuqiang.cn

[R73] 分割大日志
来源：http://pt.shxzskj.cn

split -l 1000 big.log part_
来源：http://wj.colortex.cn

[R74] 批量重命名
来源：http://ni.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fp.wgjwhj.cn

[R75] 导出环境变量
来源：http://fh.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://hv.huanxung.cn

[R76] 使用临时文件
来源：http://hc.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zn.newstarts.cn

[R77] 读取用户输入
来源：http://zw.nicolike.cn

read -rp "请输入: " ans
来源：http://on.colortex.cn

[R78] 交互式菜单
来源：http://se.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ph.szxytkj.cn

[R79] 解析命令行选项
来源：http://nx.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sv.asd995.cn

[R80] 查看脚本执行耗时
来源：http://gb.hnjuh.cn

time ./run.sh
来源：http://qp.asd995.cn

================================================================================
来源：http://mo.gzmigu.cn

S. C / C++ 专题
来源：http://lq.yuexingan06.cn

================================================================================
来源：http://ww.shtwfgs.cn

[S01] C：Hello World
来源：http://cf.nicolike.cn

#include <stdio.h>
来源：http://ug.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kc.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://ta.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://ta.bookmarksfly.cn

[S03] C：读入整数
来源：http://ru.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://yf.muxihuayi.cn

[S04] C：字符串复制
来源：http://lw.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lr.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://ts.bjjhwx.cn

strlen(s)
来源：http://qp.lnxyls.cn

[S06] C：字符串比较
来源：http://dm.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://cn.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://yj.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xl.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://ck.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://na.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://mx.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gh.colortex.cn

[S10] C：指针与解引用
来源：http://nr.nicolike.cn

int *p = &a;  *p = 5;
来源：http://er.nicolike.cn

[S11] C：逐行读文件
来源：http://iy.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://tr.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hw.hnjuh.cn

fclose(f);
来源：http://lx.9csxet.cn

[S12] C：写文件
来源：http://fn.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ru.hnjuh.cn

[S13] C：宏定义
来源：http://fh.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ta.lnxyls.cn

[S14] C：枚举
来源：http://pe.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://lx.yuexingan06.cn

[S15] C：类型转换
来源：http://qs.hahajie.cn

(double) a / b
来源：http://sx.szxytkj.cn

[S16] C：位操作置位
来源：http://yo.bookmarksfly.cn

x |= (1 << 3);
来源：http://se.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://yk.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jb.gzmigu.cn

[S18] C：命令行参数
来源：http://ir.shtwfgs.cn

int main(int argc, char **argv)
来源：http://ik.shtwfgs.cn

[S19] C：快速排序
来源：http://um.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xq.wgjwhj.cn

[S20] C：二分查找
来源：http://oe.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lk.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://fl.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yv.szxytkj.cn

[S22] C：字符串转数字
来源：http://sx.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://re.huixinmuqiang.cn

[S23] C：随机数
来源：http://ag.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mn.haigaiapp.cn

[S24] C：获取本地时间
来源：http://ra.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qo.jctech888.com.cn

[S25] C：内存拷贝
来源：http://il.haigaiapp.cn

memcpy(dst, src, n);
来源：http://iq.gzmigu.cn

[S26] C：内存清零
来源：http://mb.newstarts.cn

memset(a, 0, sizeof a);
来源：http://kk.gzmigu.cn

[S27] C：定义常量
来源：http://sf.muxihuayi.cn

const double PI = 3.14159;
来源：http://nr.chemitech.net.cn

[S28] C：静态变量
来源：http://bl.wgjwhj.cn

static int counter = 0;
来源：http://jf.bookmarksfly.cn

[S29] C：变参函数
来源：http://wi.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hb.lnxyls.cn

[S30] C：头文件保护
来源：http://bw.hnjuh.cn

#ifndef X_H
来源：http://rl.521024.cn

#define X_H
来源：http://mv.lnxyls.cn

#endif
来源：http://kb.521024.cn

[S31] C++：Hello World
来源：http://qt.newstarts.cn

#include <iostream>
来源：http://xm.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://re.shtwfgs.cn

[S32] C++：字符串
来源：http://yf.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://kf.wgjwhj.cn

[S33] C++：vector 增删
来源：http://pl.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zi.9csxet.cn

[S34] C++：遍历 vector
来源：http://js.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://ql.yuntaijiaju.cn

[S35] C++：map
来源：http://nu.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cl.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://nv.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oi.szxytkj.cn

[S37] C++：set
来源：http://ac.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ez.huixinmuqiang.cn

[S38] C++：排序
来源：http://oy.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://rt.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://at.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://if.huixiangedu.cn

[S40] C++：查找元素
来源：http://oa.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bk.hnjuh.cn

[S41] C++：类与构造函数
来源：http://uc.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jr.nicolike.cn

[S42] C++：继承与虚函数
来源：http://wb.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://ny.wgjwhj.cn

[S43] C++：智能指针
来源：http://vl.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://gf.hnjuh.cn

[S44] C++：引用传参
来源：http://jy.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://pa.muxihuayi.cn

[S45] C++：lambda
来源：http://ef.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dm.jctech888.com.cn

[S46] C++：函数模板
来源：http://si.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://im.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://ur.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nj.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://ct.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dn.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://bj.gzmigu.cn

[S49] C++：写文件
来源：http://ak.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bq.szxytkj.cn

[S50] C++：格式化数字
来源：http://oh.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jn.521024.cn

[S51] C++：显式类型转换
来源：http://av.huixiangedu.cn

static_cast<double>(a) / b
来源：http://ld.asd995.cn

[S52] C++：const 与 noexcept
来源：http://fi.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://my.asd995.cn

[S53] C++：移动语义
来源：http://il.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://bk.bjjhwx.cn

[S54] C++：异常处理
来源：http://ge.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xn.hahajie.cn

[S55] C++：结构化绑定
来源：http://nb.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ra.huixiangedu.cn

[S56] C++：optional
来源：http://iy.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pv.9csxet.cn

[S57] C++：编译期常量
来源：http://mu.bjjhwx.cn

constexpr int N = 10;
来源：http://lj.huixiangedu.cn

[S58] C++：命名空间
来源：http://en.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://cl.lnxyls.cn

[S59] C++：静态断言
来源：http://ig.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ui.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://xe.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://au.shxzskj.cn

================================================================================
来源：http://ty.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jt.newstarts.cn

================================================================================
来源：http://fy.colortex.cn

[T01] Kotlin：Hello World
来源：http://xd.lnxyls.cn

println("Hello")
来源：http://qg.9csxet.cn

[T02] Kotlin：变量
来源：http://td.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ad.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://af.bookmarksfly.cn

"值: $b"
来源：http://hf.colortex.cn

[T04] Kotlin：空安全
来源：http://je.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://lf.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://bi.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nj.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://co.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ar.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://kd.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sj.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://wt.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://zj.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://xq.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://qj.asd995.cn

[T10] Kotlin：默认参数
来源：http://hw.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://et.wgjwhj.cn

[T11] Kotlin：协程
来源：http://zo.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qp.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://mn.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://da.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://va.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://kp.9csxet.cn

[T14] Kotlin：循环
来源：http://tu.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://ae.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://qz.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://qv.hnjuh.cn

[T16] Swift：Hello World
来源：http://le.shxzskj.cn

print("Hello")
来源：http://ef.yuexingan06.cn


<!-- 参考信息 -->