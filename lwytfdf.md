代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://pr.hahajie.cn

[R14] C 风格 for
来源：http://tn.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://js.newstarts.cn

[R15] while 逐行读文件
来源：http://uq.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://am.jianghongdianzi.cn

[R16] until 等待条件
来源：http://kn.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://na.9csxet.cn

[R17] 数组定义与取值
来源：http://nz.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qy.yuexingan06.cn

[R18] 遍历数组
来源：http://qg.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://so.521024.cn

[R19] 数组长度
来源：http://cm.muxihuayi.cn

echo "${#arr[@]}"
来源：http://hn.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://ff.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qn.newstarts.cn

[R21] 字符串长度
来源：http://tp.panjiajie.cn

echo "${#s}"
来源：http://jl.yuexingan06.cn

[R22] 截取子串
来源：http://gu.shxzskj.cn

echo "${s:0:5}"
来源：http://eq.bookmarksfly.cn

[R23] 字符串替换
来源：http://ob.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ed.szxytkj.cn

[R24] 大小写转换
来源：http://oh.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vh.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://ox.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oi.bookmarksfly.cn

[R26] 命令替换
来源：http://yw.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://ag.huixiangedu.cn

[R27] 算术展开
来源：http://bm.asd995.cn

echo $((1 + 2 * 3))
来源：http://fm.shxzukj.cn

[R28] 浮点运算
来源：http://mt.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://gu.gzmigu.cn

[R29] 定义函数
来源：http://tn.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qb.shxzukj.cn

[R30] 函数返回状态码
来源：http://zp.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://jw.yuexingan06.cn

[R31] 局部变量
来源：http://vz.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://da.gzmigu.cn

[R32] 参数个数校验
来源：http://ie.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gp.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://uz.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hg.yuntaijiaju.cn

[R34] 退出时清理
来源：http://sv.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://an.chemitech.net.cn

[R35] 后台执行并等待
来源：http://ew.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jw.szxytkj.cn

[R36] 并发执行多个任务
来源：http://cl.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qs.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://ey.colortex.cn

files=$(ls -1)
来源：http://cb.9csxet.cn

[R38] 管道串联
来源：http://dh.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://kc.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://ps.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://nh.bookmarksfly.cn

[R40] 追加写日志
来源：http://qx.wgjwhj.cn

echo "log" >> out.log
来源：http://kn.asd995.cn

[R41] 丢弃输出
来源：http://pd.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://ik.shxzukj.cn

[R42] 输入重定向
来源：http://ps.bjjhwx.cn

wc -l < a.txt
来源：http://oo.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://wb.szsharing.cn

find . -name "*.log" -type f
来源：http://kx.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://hy.wgjwhj.cn

find . -mtime -7 -type f
来源：http://ts.szxytkj.cn

[R45] 批量删除
来源：http://ru.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://nu.9csxet.cn

[R46] 递归替换文件内容
来源：http://or.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wr.wgjwhj.cn

[R47] sed 单行替换
来源：http://yz.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nq.shxzukj.cn

[R48] awk 取指定列
来源：http://er.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://ow.huixinmuqiang.cn

[R49] awk 带条件
来源：http://wi.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kt.newstarts.cn

[R50] awk 求和
来源：http://oq.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ad.panjiajie.cn

[R51] 排序去重取前几
来源：http://ab.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bq.colortex.cn

[R52] 统计行数
来源：http://ts.jianghongdianzi.cn

wc -l a.txt
来源：http://ed.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://mn.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://am.bookmarksfly.cn

[R54] 比较两个文件
来源：http://wh.nszjky.cn

diff a.txt b.txt
来源：http://au.muxihuayi.cn

[R55] 压缩与解压
来源：http://vw.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tb.huixiangedu.cn

[R56] 远程拷贝
来源：http://oo.wgjwhj.cn

scp file user@host:/path/
来源：http://ll.9csxet.cn

[R57] 远程执行命令
来源：http://ns.bjjhwx.cn

ssh user@host 'uptime'
来源：http://md.wgjwhj.cn

[R58] 下载文件
来源：http://iw.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yy.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://gn.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eb.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://ue.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wl.hnjuh.cn

[R61] 磁盘占用
来源：http://vz.shxzskj.cn

df -h;  du -sh *
来源：http://mj.shxzskj.cn

[R62] 找最占空间的文件
来源：http://dr.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://ly.huanxung.cn

[R63] 内存与进程
来源：http://tk.colortex.cn

free -h;  ps aux | grep nginx
来源：http://ze.jctech888.com.cn

[R64] 结束进程
来源：http://vi.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://hz.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://td.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cz.hnjuh.cn

[R66] 定时任务
来源：http://tf.yuexingan06.cn

crontab -e;  crontab -l
来源：http://ip.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://qp.haigaiapp.cn

openssl rand -hex 16
来源：http://wd.lnxyls.cn

[R68] 计算文件校验值
来源：http://yg.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oi.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://zn.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://vy.521024.cn

[R70] 时间戳与互转
来源：http://hl.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://kk.9csxet.cn

[R71] 日期格式化
来源：http://kp.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bg.newstarts.cn

[R72] 等待端口就绪
来源：http://bk.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ne.bookmarksfly.cn

[R73] 分割大日志
来源：http://fo.bjjhwx.cn

split -l 1000 big.log part_
来源：http://fo.jianghongdianzi.cn

[R74] 批量重命名
来源：http://gg.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rp.muxihuayi.cn

[R75] 导出环境变量
来源：http://nk.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://xa.chemitech.net.cn

[R76] 使用临时文件
来源：http://xw.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pu.gzmigu.cn

[R77] 读取用户输入
来源：http://jz.newstarts.cn

read -rp "请输入: " ans
来源：http://qc.szsharing.cn

[R78] 交互式菜单
来源：http://sv.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pu.521024.cn

[R79] 解析命令行选项
来源：http://tm.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ge.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://yu.hnjuh.cn

time ./run.sh
来源：http://ym.shtwfgs.cn

================================================================================
来源：http://pg.shxzukj.cn

S. C / C++ 专题
来源：http://rp.shxzukj.cn

================================================================================
来源：http://iw.huixiangedu.cn

[S01] C：Hello World
来源：http://dk.nicolike.cn

#include <stdio.h>
来源：http://yu.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://je.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://rr.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://et.colortex.cn

[S03] C：读入整数
来源：http://wa.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://hh.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://gd.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vl.colortex.cn

[S05] C：字符串长度
来源：http://kg.szxytkj.cn

strlen(s)
来源：http://pk.bookmarksfly.cn

[S06] C：字符串比较
来源：http://lu.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://kg.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://cv.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ft.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://by.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bq.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://yx.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ut.hnjuh.cn

[S10] C：指针与解引用
来源：http://hc.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://du.szxytkj.cn

[S11] C：逐行读文件
来源：http://ul.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://cj.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kq.gzmigu.cn

fclose(f);
来源：http://wm.shxzukj.cn

[S12] C：写文件
来源：http://yr.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ny.muxihuayi.cn

[S13] C：宏定义
来源：http://vb.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ef.521024.cn

[S14] C：枚举
来源：http://lk.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://ew.jctech888.com.cn

[S15] C：类型转换
来源：http://cq.bookmarksfly.cn

(double) a / b
来源：http://af.huixiangedu.cn

[S16] C：位操作置位
来源：http://et.haigaiapp.cn

x |= (1 << 3);
来源：http://au.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://ic.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yb.jctech888.com.cn

[S18] C：命令行参数
来源：http://jt.huanxung.cn

int main(int argc, char **argv)
来源：http://we.nszjky.cn

[S19] C：快速排序
来源：http://is.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qy.lnxyls.cn

[S20] C：二分查找
来源：http://jr.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mw.wgjwhj.cn

[S21] C：字符类别判断
来源：http://yq.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pu.shxzskj.cn

[S22] C：字符串转数字
来源：http://xe.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ye.szxytkj.cn

[S23] C：随机数
来源：http://nl.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ny.haigaiapp.cn

[S24] C：获取本地时间
来源：http://nf.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iw.muxihuayi.cn

[S25] C：内存拷贝
来源：http://tg.szsharing.cn

memcpy(dst, src, n);
来源：http://xl.haigaiapp.cn

[S26] C：内存清零
来源：http://xz.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://en.muxihuayi.cn

[S27] C：定义常量
来源：http://dm.lnxyls.cn

const double PI = 3.14159;
来源：http://li.nszjky.cn

[S28] C：静态变量
来源：http://sy.wgjwhj.cn

static int counter = 0;
来源：http://wq.huanxung.cn

[S29] C：变参函数
来源：http://lp.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ss.gzmigu.cn

[S30] C：头文件保护
来源：http://nh.bjjhwx.cn

#ifndef X_H
来源：http://an.bookmarksfly.cn

#define X_H
来源：http://bj.9csxet.cn

#endif
来源：http://ag.newstarts.cn

[S31] C++：Hello World
来源：http://dz.szxytkj.cn

#include <iostream>
来源：http://kc.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://tg.szxytkj.cn

[S32] C++：字符串
来源：http://ki.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://me.shtwfgs.cn

[S33] C++：vector 增删
来源：http://la.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dc.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://wj.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://mo.haigaiapp.cn

[S35] C++：map
来源：http://xf.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sw.muxihuayi.cn

[S36] C++：unordered_map
来源：http://ff.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rw.asd995.cn

[S37] C++：set
来源：http://nj.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dp.yuntaijiaju.cn

[S38] C++：排序
来源：http://ao.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://ty.asd995.cn

[S39] C++：自定义比较器排序
来源：http://xc.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wc.shxzukj.cn

[S40] C++：查找元素
来源：http://du.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fo.szxytkj.cn

[S41] C++：类与构造函数
来源：http://vh.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tp.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://pv.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://gr.hnjuh.cn

[S43] C++：智能指针
来源：http://su.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://ik.haigaiapp.cn

[S44] C++：引用传参
来源：http://ya.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://qv.newstarts.cn

[S45] C++：lambda
来源：http://cq.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xh.bjjhwx.cn

[S46] C++：函数模板
来源：http://qq.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sn.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://no.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ti.szsharing.cn

[S48] C++：逐行读文件
来源：http://ed.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ly.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://ae.hnjuh.cn

[S49] C++：写文件
来源：http://ro.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ml.huanxung.cn

[S50] C++：格式化数字
来源：http://gr.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ir.szsharing.cn

[S51] C++：显式类型转换
来源：http://zj.shxzukj.cn

static_cast<double>(a) / b
来源：http://zn.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://kk.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://qj.9csxet.cn

[S53] C++：移动语义
来源：http://vb.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://qu.hahajie.cn

[S54] C++：异常处理
来源：http://te.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ki.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://cr.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cv.panjiajie.cn

[S56] C++：optional
来源：http://ck.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gn.szxytkj.cn

[S57] C++：编译期常量
来源：http://vm.huixiangedu.cn

constexpr int N = 10;
来源：http://gh.jctech888.com.cn

[S58] C++：命名空间
来源：http://ql.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://sw.chemitech.net.cn

[S59] C++：静态断言
来源：http://ho.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ii.521024.cn

[S60] C++：遍历并删除元素
来源：http://vw.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gq.panjiajie.cn

================================================================================
来源：http://du.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ua.panjiajie.cn

================================================================================
来源：http://xz.9csxet.cn

[T01] Kotlin：Hello World
来源：http://hp.nszjky.cn

println("Hello")
来源：http://qx.muxihuayi.cn

[T02] Kotlin：变量
来源：http://oq.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wp.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://ef.bjjhwx.cn

"值: $b"
来源：http://ft.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://bx.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://lt.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://kn.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jo.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://xo.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wx.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://pr.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mo.nicolike.cn

[T08] Kotlin：数据类
来源：http://ur.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://vo.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://mm.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://mg.nicolike.cn

[T10] Kotlin：默认参数
来源：http://df.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vo.hahajie.cn

[T11] Kotlin：协程
来源：http://ru.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pc.9csxet.cn

[T12] Kotlin：解构声明
来源：http://tz.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://me.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://xf.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://su.szsharing.cn

[T14] Kotlin：循环
来源：http://aq.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://sb.newstarts.cn

[T15] Kotlin：接口
来源：http://fk.nszjky.cn

interface Shape { fun area(): Double }
来源：http://em.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://yg.9csxet.cn

print("Hello")
来源：http://oa.bjjhwx.cn


<!-- 参考信息 -->