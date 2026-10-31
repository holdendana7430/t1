代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hp.gzmigu.cn

[R16] until 等待条件
来源：http://wj.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dp.yuexingan06.cn

[R17] 数组定义与取值
来源：http://uk.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://at.bjjhwx.cn

[R18] 遍历数组
来源：http://ps.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mw.nszjky.cn

[R19] 数组长度
来源：http://bc.chemitech.net.cn

echo "${#arr[@]}"
来源：http://oa.shxzskj.cn

[R20] 关联数组（字典）
来源：http://ud.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fv.hahajie.cn

[R21] 字符串长度
来源：http://ry.jianghongdianzi.cn

echo "${#s}"
来源：http://fg.huixiangedu.cn

[R22] 截取子串
来源：http://yy.lnxyls.cn

echo "${s:0:5}"
来源：http://rv.yuexingan06.cn

[R23] 字符串替换
来源：http://ex.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xj.huanxung.cn

[R24] 大小写转换
来源：http://bk.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ie.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://dp.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dr.lnxyls.cn

[R26] 命令替换
来源：http://ra.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://bp.jianghongdianzi.cn

[R27] 算术展开
来源：http://gd.hahajie.cn

echo $((1 + 2 * 3))
来源：http://rq.gzmigu.cn

[R28] 浮点运算
来源：http://os.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://cj.jctech888.com.cn

[R29] 定义函数
来源：http://hd.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zd.bjjhwx.cn

[R30] 函数返回状态码
来源：http://lb.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://hs.chemitech.net.cn

[R31] 局部变量
来源：http://gu.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://qs.szxytkj.cn

[R32] 参数个数校验
来源：http://kq.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ja.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://cb.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qm.yuexingan06.cn

[R34] 退出时清理
来源：http://mi.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tf.nszjky.cn

[R35] 后台执行并等待
来源：http://av.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vo.szsharing.cn

[R36] 并发执行多个任务
来源：http://vh.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wo.szxytkj.cn

[R37] 把输出赋给变量
来源：http://wk.yuntaijiaju.cn

files=$(ls -1)
来源：http://fz.chemitech.net.cn

[R38] 管道串联
来源：http://ak.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://mu.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://sx.shxzskj.cn

cmd > out.log 2>&1
来源：http://go.lnxyls.cn

[R40] 追加写日志
来源：http://kf.9csxet.cn

echo "log" >> out.log
来源：http://sq.lnxyls.cn

[R41] 丢弃输出
来源：http://up.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://xn.521024.cn

[R42] 输入重定向
来源：http://an.shxzskj.cn

wc -l < a.txt
来源：http://ox.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://iq.lnxyls.cn

find . -name "*.log" -type f
来源：http://oa.szxytkj.cn

[R44] 按修改时间查找
来源：http://wh.shtwfgs.cn

find . -mtime -7 -type f
来源：http://bp.huixinmuqiang.cn

[R45] 批量删除
来源：http://js.asd995.cn

find . -name "*.tmp" -delete
来源：http://fc.nicolike.cn

[R46] 递归替换文件内容
来源：http://we.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eg.nszjky.cn

[R47] sed 单行替换
来源：http://vg.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vh.9csxet.cn

[R48] awk 取指定列
来源：http://kk.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://pd.nicolike.cn

[R49] awk 带条件
来源：http://zy.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://en.yuexingan06.cn

[R50] awk 求和
来源：http://mo.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zl.panjiajie.cn

[R51] 排序去重取前几
来源：http://lx.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jn.nicolike.cn

[R52] 统计行数
来源：http://ha.haigaiapp.cn

wc -l a.txt
来源：http://fi.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://cj.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://se.huixiangedu.cn

[R54] 比较两个文件
来源：http://fu.huixinmuqiang.cn

diff a.txt b.txt
来源：http://fl.chemitech.net.cn

[R55] 压缩与解压
来源：http://qt.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ec.chemitech.net.cn

[R56] 远程拷贝
来源：http://yz.shxzskj.cn

scp file user@host:/path/
来源：http://ed.jctech888.com.cn

[R57] 远程执行命令
来源：http://sl.hnjuh.cn

ssh user@host 'uptime'
来源：http://bc.panjiajie.cn

[R58] 下载文件
来源：http://vw.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kn.9csxet.cn

[R59] 发 POST JSON
来源：http://tl.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tw.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://av.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cl.yuexingan06.cn

[R61] 磁盘占用
来源：http://rt.haigaiapp.cn

df -h;  du -sh *
来源：http://jz.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://kf.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://co.huixinmuqiang.cn

[R63] 内存与进程
来源：http://ij.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://xk.wgjwhj.cn

[R64] 结束进程
来源：http://rr.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://na.shxzukj.cn

[R65] 查看端口占用
来源：http://ck.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://th.jianghongdianzi.cn

[R66] 定时任务
来源：http://xu.asd995.cn

crontab -e;  crontab -l
来源：http://mz.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://bb.nicolike.cn

openssl rand -hex 16
来源：http://kn.yuexingan06.cn

[R68] 计算文件校验值
来源：http://iq.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nw.muxihuayi.cn

[R69] 生成随机密码
来源：http://kr.521024.cn

head -c 16 /dev/urandom | base64
来源：http://zd.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://nc.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://kc.wgjwhj.cn

[R71] 日期格式化
来源：http://db.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://al.gzmigu.cn

[R72] 等待端口就绪
来源：http://hr.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ua.shxzukj.cn

[R73] 分割大日志
来源：http://bx.jctech888.com.cn

split -l 1000 big.log part_
来源：http://ky.shxzskj.cn

[R74] 批量重命名
来源：http://yc.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cq.jctech888.com.cn

[R75] 导出环境变量
来源：http://at.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ao.hahajie.cn

[R76] 使用临时文件
来源：http://iz.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vp.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://ok.hnjuh.cn

read -rp "请输入: " ans
来源：http://nu.huixiangedu.cn

[R78] 交互式菜单
来源：http://um.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bv.newstarts.cn

[R79] 解析命令行选项
来源：http://go.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aw.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://su.521024.cn

time ./run.sh
来源：http://ar.lnxyls.cn

================================================================================
来源：http://zz.szsharing.cn

S. C / C++ 专题
来源：http://tj.jctech888.com.cn

================================================================================
来源：http://st.huanxung.cn

[S01] C：Hello World
来源：http://bz.huixinmuqiang.cn

#include <stdio.h>
来源：http://ef.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xt.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://ym.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://se.shxzukj.cn

[S03] C：读入整数
来源：http://vb.hahajie.cn

int x; scanf("%d", &x);
来源：http://rn.colortex.cn

[S04] C：字符串复制
来源：http://fw.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dl.colortex.cn

[S05] C：字符串长度
来源：http://pg.yuexingan06.cn

strlen(s)
来源：http://eg.szsharing.cn

[S06] C：字符串比较
来源：http://mv.szxytkj.cn

strcmp(a, b) == 0
来源：http://px.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://ia.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lg.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://ar.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ha.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://pe.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ro.521024.cn

[S10] C：指针与解引用
来源：http://eh.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://ee.jctech888.com.cn

[S11] C：逐行读文件
来源：http://nn.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://rj.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bj.huixiangedu.cn

fclose(f);
来源：http://tq.bjjhwx.cn

[S12] C：写文件
来源：http://nj.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qa.wgjwhj.cn

[S13] C：宏定义
来源：http://jv.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://le.shtwfgs.cn

[S14] C：枚举
来源：http://yo.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://ac.shtwfgs.cn

[S15] C：类型转换
来源：http://yy.yuexingan06.cn

(double) a / b
来源：http://eh.9csxet.cn

[S16] C：位操作置位
来源：http://ws.shxzukj.cn

x |= (1 << 3);
来源：http://li.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://ag.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hp.nicolike.cn

[S18] C：命令行参数
来源：http://rv.asd995.cn

int main(int argc, char **argv)
来源：http://kz.yuexingan06.cn

[S19] C：快速排序
来源：http://ox.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lq.shtwfgs.cn

[S20] C：二分查找
来源：http://ks.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eb.newstarts.cn

[S21] C：字符类别判断
来源：http://ps.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://am.shxzskj.cn

[S22] C：字符串转数字
来源：http://sk.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zc.newstarts.cn

[S23] C：随机数
来源：http://po.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pj.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://kd.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eh.huanxung.cn

[S25] C：内存拷贝
来源：http://lv.haigaiapp.cn

memcpy(dst, src, n);
来源：http://hc.colortex.cn

[S26] C：内存清零
来源：http://zm.9csxet.cn

memset(a, 0, sizeof a);
来源：http://ys.chemitech.net.cn

[S27] C：定义常量
来源：http://xi.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://nf.newstarts.cn

[S28] C：静态变量
来源：http://rd.jianghongdianzi.cn

static int counter = 0;
来源：http://tc.9csxet.cn

[S29] C：变参函数
来源：http://qk.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qu.lnxyls.cn

[S30] C：头文件保护
来源：http://at.jianghongdianzi.cn

#ifndef X_H
来源：http://kh.szxytkj.cn

#define X_H
来源：http://jx.colortex.cn

#endif
来源：http://qn.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://ci.shtwfgs.cn

#include <iostream>
来源：http://ez.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://os.asd995.cn

[S32] C++：字符串
来源：http://nq.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://xy.szxytkj.cn

[S33] C++：vector 增删
来源：http://fr.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jx.nicolike.cn

[S34] C++：遍历 vector
来源：http://kt.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://yi.521024.cn

[S35] C++：map
来源：http://yl.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gd.nicolike.cn

[S36] C++：unordered_map
来源：http://ml.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sm.colortex.cn

[S37] C++：set
来源：http://pz.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fr.hnjuh.cn

[S38] C++：排序
来源：http://lm.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://ja.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://pa.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ha.gzmigu.cn

[S40] C++：查找元素
来源：http://ty.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mh.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://fu.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kw.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://wn.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://uv.521024.cn

[S43] C++：智能指针
来源：http://rf.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://ij.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://av.asd995.cn

void inc(int &x) { ++x; }
来源：http://ii.nicolike.cn

[S45] C++：lambda
来源：http://we.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zd.yuexingan06.cn

[S46] C++：函数模板
来源：http://gy.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://av.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://uk.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jz.shxzskj.cn

[S48] C++：逐行读文件
来源：http://zl.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xd.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://tb.wgjwhj.cn

[S49] C++：写文件
来源：http://mj.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ne.bjjhwx.cn

[S50] C++：格式化数字
来源：http://di.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wx.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://mc.9csxet.cn

static_cast<double>(a) / b
来源：http://it.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://ux.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://kh.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ty.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://ko.asd995.cn

[S54] C++：异常处理
来源：http://vx.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yj.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://zl.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uc.haigaiapp.cn

[S56] C++：optional
来源：http://hp.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bq.wgjwhj.cn

[S57] C++：编译期常量
来源：http://mb.newstarts.cn

constexpr int N = 10;
来源：http://tc.nszjky.cn

[S58] C++：命名空间
来源：http://rb.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://yv.nicolike.cn

[S59] C++：静态断言
来源：http://vo.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ev.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://vo.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ag.huanxung.cn

================================================================================
来源：http://xi.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rs.shxzukj.cn

================================================================================
来源：http://qp.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://ky.huanxung.cn

println("Hello")
来源：http://dt.lnxyls.cn

[T02] Kotlin：变量
来源：http://ka.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ie.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://yc.nszjky.cn

"值: $b"
来源：http://hv.lnxyls.cn

[T04] Kotlin：空安全
来源：http://tp.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://kh.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://kj.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sj.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://oo.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yn.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://eo.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cm.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://yo.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://lt.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://so.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://qb.asd995.cn

[T10] Kotlin：默认参数
来源：http://iv.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://al.hahajie.cn

[T11] Kotlin：协程
来源：http://cu.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vj.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://vm.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://ch.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://vn.nszjky.cn

val m = mapOf("a" to 1)
来源：http://ge.bjjhwx.cn

[T14] Kotlin：循环
来源：http://ag.hahajie.cn

for (i in 1..10) println(i)
来源：http://tr.yuexingan06.cn

[T15] Kotlin：接口
来源：http://hw.nicolike.cn

interface Shape { fun area(): Double }
来源：http://wy.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://xr.bjjhwx.cn

print("Hello")
来源：http://em.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://cf.9csxet.cn

var a = 1;  let b = 2
来源：http://jn.hahajie.cn

[T18] Swift：字符串插值
来源：http://pz.chemitech.net.cn

"值: \(b)"
来源：http://fk.huixiangedu.cn


<!-- 参考信息 -->