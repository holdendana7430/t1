代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://xe.yuntaijiaju.cn

[R14] C 风格 for
来源：http://lc.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ew.hnjuh.cn

[R15] while 逐行读文件
来源：http://yd.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ye.lnxyls.cn

[R16] until 等待条件
来源：http://sr.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://el.521024.cn

[R17] 数组定义与取值
来源：http://re.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nb.521024.cn

[R18] 遍历数组
来源：http://um.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://da.bookmarksfly.cn

[R19] 数组长度
来源：http://bi.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://lg.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://ym.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uy.gzmigu.cn

[R21] 字符串长度
来源：http://hy.yuntaijiaju.cn

echo "${#s}"
来源：http://up.yuexingan06.cn

[R22] 截取子串
来源：http://el.lnxyls.cn

echo "${s:0:5}"
来源：http://sj.huixinmuqiang.cn

[R23] 字符串替换
来源：http://hm.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ht.yuexingan06.cn

[R24] 大小写转换
来源：http://zx.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wz.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://dy.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mk.szsharing.cn

[R26] 命令替换
来源：http://ib.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://li.9csxet.cn

[R27] 算术展开
来源：http://hu.9csxet.cn

echo $((1 + 2 * 3))
来源：http://cr.huixinmuqiang.cn

[R28] 浮点运算
来源：http://cz.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://iy.shtwfgs.cn

[R29] 定义函数
来源：http://qe.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yt.szsharing.cn

[R30] 函数返回状态码
来源：http://qh.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://rf.nicolike.cn

[R31] 局部变量
来源：http://bk.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://ct.nicolike.cn

[R32] 参数个数校验
来源：http://yi.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gh.colortex.cn

[R33] 捕获错误并提示行号
来源：http://gj.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eu.shxzukj.cn

[R34] 退出时清理
来源：http://kc.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mk.gzmigu.cn

[R35] 后台执行并等待
来源：http://xr.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://aq.szsharing.cn

[R36] 并发执行多个任务
来源：http://co.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oz.szsharing.cn

[R37] 把输出赋给变量
来源：http://ik.asd995.cn

files=$(ls -1)
来源：http://hw.gzmigu.cn

[R38] 管道串联
来源：http://rr.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://xo.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://yr.nicolike.cn

cmd > out.log 2>&1
来源：http://rx.colortex.cn

[R40] 追加写日志
来源：http://sl.hnjuh.cn

echo "log" >> out.log
来源：http://fg.asd995.cn

[R41] 丢弃输出
来源：http://dj.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://te.bjjhwx.cn

[R42] 输入重定向
来源：http://hw.huanxung.cn

wc -l < a.txt
来源：http://sk.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://gw.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://gr.gzmigu.cn

[R44] 按修改时间查找
来源：http://da.hnjuh.cn

find . -mtime -7 -type f
来源：http://ir.asd995.cn

[R45] 批量删除
来源：http://eq.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://qy.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://bk.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mi.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://wr.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nq.colortex.cn

[R48] awk 取指定列
来源：http://ax.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://td.nicolike.cn

[R49] awk 带条件
来源：http://da.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mm.newstarts.cn

[R50] awk 求和
来源：http://xa.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ov.shtwfgs.cn

[R51] 排序去重取前几
来源：http://yz.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ua.panjiajie.cn

[R52] 统计行数
来源：http://bp.gzmigu.cn

wc -l a.txt
来源：http://nn.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://jf.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fa.nszjky.cn

[R54] 比较两个文件
来源：http://bq.gzmigu.cn

diff a.txt b.txt
来源：http://pl.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://ci.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ry.hahajie.cn

[R56] 远程拷贝
来源：http://oz.szxytkj.cn

scp file user@host:/path/
来源：http://rr.huanxung.cn

[R57] 远程执行命令
来源：http://ug.chemitech.net.cn

ssh user@host 'uptime'
来源：http://oc.panjiajie.cn

[R58] 下载文件
来源：http://nm.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ev.nicolike.cn

[R59] 发 POST JSON
来源：http://mq.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://io.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://bn.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tv.9csxet.cn

[R61] 磁盘占用
来源：http://qk.jianghongdianzi.cn

df -h;  du -sh *
来源：http://vi.gzmigu.cn

[R62] 找最占空间的文件
来源：http://wa.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://mp.shxzukj.cn

[R63] 内存与进程
来源：http://ti.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://lt.gzmigu.cn

[R64] 结束进程
来源：http://jj.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://yh.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://ma.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dx.newstarts.cn

[R66] 定时任务
来源：http://cf.colortex.cn

crontab -e;  crontab -l
来源：http://wp.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://jq.521024.cn

openssl rand -hex 16
来源：http://ry.chemitech.net.cn

[R68] 计算文件校验值
来源：http://os.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ek.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://yd.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://gl.huixiangedu.cn

[R70] 时间戳与互转
来源：http://pg.asd995.cn

date +%s;  date -d @1700000000
来源：http://tt.nicolike.cn

[R71] 日期格式化
来源：http://ex.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vf.shtwfgs.cn

[R72] 等待端口就绪
来源：http://ew.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vd.wgjwhj.cn

[R73] 分割大日志
来源：http://yr.nszjky.cn

split -l 1000 big.log part_
来源：http://ez.shxzukj.cn

[R74] 批量重命名
来源：http://jz.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://po.nicolike.cn

[R75] 导出环境变量
来源：http://rq.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://ao.newstarts.cn

[R76] 使用临时文件
来源：http://rd.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://md.newstarts.cn

[R77] 读取用户输入
来源：http://ww.hnjuh.cn

read -rp "请输入: " ans
来源：http://db.yuexingan06.cn

[R78] 交互式菜单
来源：http://tc.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://si.panjiajie.cn

[R79] 解析命令行选项
来源：http://dj.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ij.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://on.shtwfgs.cn

time ./run.sh
来源：http://yu.jctech888.com.cn

================================================================================
来源：http://mw.nicolike.cn

S. C / C++ 专题
来源：http://pk.szsharing.cn

================================================================================
来源：http://nw.hnjuh.cn

[S01] C：Hello World
来源：http://fz.asd995.cn

#include <stdio.h>
来源：http://eh.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ft.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://ih.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://ga.huanxung.cn

[S03] C：读入整数
来源：http://qz.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://il.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://zc.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ji.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://hm.szxytkj.cn

strlen(s)
来源：http://tm.shxzskj.cn

[S06] C：字符串比较
来源：http://yg.haigaiapp.cn

strcmp(a, b) == 0
来源：http://rw.colortex.cn

[S07] C：数组遍历求和
来源：http://kb.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ru.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://jf.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ma.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://tk.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://li.gzmigu.cn

[S10] C：指针与解引用
来源：http://du.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://ac.huixiangedu.cn

[S11] C：逐行读文件
来源：http://wt.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://gl.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bp.szxytkj.cn

fclose(f);
来源：http://tl.bjjhwx.cn

[S12] C：写文件
来源：http://kx.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qs.haigaiapp.cn

[S13] C：宏定义
来源：http://lb.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ux.shxzskj.cn

[S14] C：枚举
来源：http://gx.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://th.huixiangedu.cn

[S15] C：类型转换
来源：http://qf.shxzskj.cn

(double) a / b
来源：http://cr.gzmigu.cn

[S16] C：位操作置位
来源：http://vk.muxihuayi.cn

x |= (1 << 3);
来源：http://oe.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://fd.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xj.muxihuayi.cn

[S18] C：命令行参数
来源：http://vk.asd995.cn

int main(int argc, char **argv)
来源：http://vj.lnxyls.cn

[S19] C：快速排序
来源：http://qm.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kf.panjiajie.cn

[S20] C：二分查找
来源：http://dz.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yg.lnxyls.cn

[S21] C：字符类别判断
来源：http://og.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zd.gzmigu.cn

[S22] C：字符串转数字
来源：http://wz.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nn.nicolike.cn

[S23] C：随机数
来源：http://ez.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bj.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://xw.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cb.nszjky.cn

[S25] C：内存拷贝
来源：http://tr.yuexingan06.cn

memcpy(dst, src, n);
来源：http://ki.chemitech.net.cn

[S26] C：内存清零
来源：http://qm.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://xz.szxytkj.cn

[S27] C：定义常量
来源：http://ob.szsharing.cn

const double PI = 3.14159;
来源：http://bs.shtwfgs.cn

[S28] C：静态变量
来源：http://ql.yuntaijiaju.cn

static int counter = 0;
来源：http://zr.panjiajie.cn

[S29] C：变参函数
来源：http://ml.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bg.hahajie.cn

[S30] C：头文件保护
来源：http://hu.wgjwhj.cn

#ifndef X_H
来源：http://pc.szsharing.cn

#define X_H
来源：http://rv.huixiangedu.cn

#endif
来源：http://da.hnjuh.cn

[S31] C++：Hello World
来源：http://gx.jctech888.com.cn

#include <iostream>
来源：http://iz.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://as.9csxet.cn

[S32] C++：字符串
来源：http://ch.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://wa.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://hn.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ps.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://vf.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://xk.huanxung.cn

[S35] C++：map
来源：http://mb.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dy.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://ue.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ui.szsharing.cn

[S37] C++：set
来源：http://cb.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://py.9csxet.cn

[S38] C++：排序
来源：http://nh.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://qy.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://wz.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xz.shtwfgs.cn

[S40] C++：查找元素
来源：http://cm.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gz.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://qg.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oj.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://vl.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://ia.colortex.cn

[S43] C++：智能指针
来源：http://gi.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://sj.szsharing.cn

[S44] C++：引用传参
来源：http://qu.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://ib.huanxung.cn

[S45] C++：lambda
来源：http://oc.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hs.jctech888.com.cn

[S46] C++：函数模板
来源：http://xt.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lz.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://ze.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pw.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://kz.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wh.asd995.cn

while (std::getline(in, line)) { }
来源：http://wz.haigaiapp.cn

[S49] C++：写文件
来源：http://hn.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xg.9csxet.cn

[S50] C++：格式化数字
来源：http://op.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ev.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://dz.lnxyls.cn

static_cast<double>(a) / b
来源：http://wx.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://fs.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://va.shxzskj.cn

[S53] C++：移动语义
来源：http://si.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://eb.shxzukj.cn

[S54] C++：异常处理
来源：http://jd.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fc.shxzukj.cn

[S55] C++：结构化绑定
来源：http://bx.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jv.hahajie.cn

[S56] C++：optional
来源：http://rq.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wt.jctech888.com.cn

[S57] C++：编译期常量
来源：http://yl.huixinmuqiang.cn

constexpr int N = 10;
来源：http://ba.szsharing.cn

[S58] C++：命名空间
来源：http://qz.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://ui.szsharing.cn

[S59] C++：静态断言
来源：http://bk.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fc.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://ye.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rl.jianghongdianzi.cn

================================================================================
来源：http://yf.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uv.asd995.cn

================================================================================
来源：http://ms.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://vd.wgjwhj.cn

println("Hello")
来源：http://zv.szxytkj.cn

[T02] Kotlin：变量
来源：http://ub.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pt.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://ty.shxzskj.cn

"值: $b"
来源：http://ew.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://pi.nszjky.cn

val n: String? = null;  n?.length
来源：http://nk.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://bi.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nm.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://gv.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xr.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://kj.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lh.hahajie.cn

[T08] Kotlin：数据类
来源：http://rs.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://je.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://ow.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://zf.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://ra.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rd.chemitech.net.cn

[T11] Kotlin：协程
来源：http://go.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ep.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://bq.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://ms.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://se.szsharing.cn

val m = mapOf("a" to 1)
来源：http://sa.asd995.cn

[T14] Kotlin：循环
来源：http://ca.shxzukj.cn

for (i in 1..10) println(i)
来源：http://cw.newstarts.cn

[T15] Kotlin：接口
来源：http://hf.asd995.cn

interface Shape { fun area(): Double }
来源：http://ei.lnxyls.cn

[T16] Swift：Hello World
来源：http://hq.szxytkj.cn

print("Hello")
来源：http://en.huixinmuqiang.cn


<!-- 参考信息 -->