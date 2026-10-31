代发 wailian999

esac
来源：http://eb.szsharing.cn

[R12] for 遍历文件
来源：http://pb.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://ar.yuntaijiaju.cn

[R13] for 计数循环
来源：http://cz.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://vt.shxzukj.cn

[R14] C 风格 for
来源：http://kk.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ab.shtwfgs.cn

[R15] while 逐行读文件
来源：http://xs.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ew.szsharing.cn

[R16] until 等待条件
来源：http://jm.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://to.muxihuayi.cn

[R17] 数组定义与取值
来源：http://ab.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hh.hahajie.cn

[R18] 遍历数组
来源：http://cp.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tq.jctech888.com.cn

[R19] 数组长度
来源：http://mo.shxzukj.cn

echo "${#arr[@]}"
来源：http://ev.shxzskj.cn

[R20] 关联数组（字典）
来源：http://jb.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zd.panjiajie.cn

[R21] 字符串长度
来源：http://xp.521024.cn

echo "${#s}"
来源：http://qq.jctech888.com.cn

[R22] 截取子串
来源：http://ow.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://il.521024.cn

[R23] 字符串替换
来源：http://rh.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oo.jctech888.com.cn

[R24] 大小写转换
来源：http://cv.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://eh.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://rj.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bi.bookmarksfly.cn

[R26] 命令替换
来源：http://ph.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://rm.yuexingan06.cn

[R27] 算术展开
来源：http://xv.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://no.huanxung.cn

[R28] 浮点运算
来源：http://zh.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://xm.nszjky.cn

[R29] 定义函数
来源：http://hh.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://we.bjjhwx.cn

[R30] 函数返回状态码
来源：http://vs.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ia.newstarts.cn

[R31] 局部变量
来源：http://pf.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://qx.yuexingan06.cn

[R32] 参数个数校验
来源：http://zj.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nx.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://al.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ge.colortex.cn

[R34] 退出时清理
来源：http://zz.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bl.shxzskj.cn

[R35] 后台执行并等待
来源：http://bk.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fk.asd995.cn

[R36] 并发执行多个任务
来源：http://lw.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://li.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://sb.hnjuh.cn

files=$(ls -1)
来源：http://lv.yuexingan06.cn

[R38] 管道串联
来源：http://yg.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://di.colortex.cn

[R39] 重定向标准输出与错误
来源：http://ej.colortex.cn

cmd > out.log 2>&1
来源：http://un.9csxet.cn

[R40] 追加写日志
来源：http://ya.muxihuayi.cn

echo "log" >> out.log
来源：http://jt.hahajie.cn

[R41] 丢弃输出
来源：http://nq.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://ww.yuexingan06.cn

[R42] 输入重定向
来源：http://mt.bjjhwx.cn

wc -l < a.txt
来源：http://zg.colortex.cn

[R43] 按名字查找文件
来源：http://ue.nszjky.cn

find . -name "*.log" -type f
来源：http://mo.muxihuayi.cn

[R44] 按修改时间查找
来源：http://mu.asd995.cn

find . -mtime -7 -type f
来源：http://fg.nicolike.cn

[R45] 批量删除
来源：http://sp.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://eh.szxytkj.cn

[R46] 递归替换文件内容
来源：http://oc.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rx.shtwfgs.cn

[R47] sed 单行替换
来源：http://tw.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gm.szsharing.cn

[R48] awk 取指定列
来源：http://hb.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://yv.shxzukj.cn

[R49] awk 带条件
来源：http://ol.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hi.nicolike.cn

[R50] awk 求和
来源：http://pf.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hw.521024.cn

[R51] 排序去重取前几
来源：http://na.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bu.bjjhwx.cn

[R52] 统计行数
来源：http://gl.nszjky.cn

wc -l a.txt
来源：http://hk.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://ti.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kk.shtwfgs.cn

[R54] 比较两个文件
来源：http://ak.gzmigu.cn

diff a.txt b.txt
来源：http://jr.yuexingan06.cn

[R55] 压缩与解压
来源：http://oh.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ym.shtwfgs.cn

[R56] 远程拷贝
来源：http://ry.jianghongdianzi.cn

scp file user@host:/path/
来源：http://jn.jctech888.com.cn

[R57] 远程执行命令
来源：http://kl.shxzskj.cn

ssh user@host 'uptime'
来源：http://ya.shxzskj.cn

[R58] 下载文件
来源：http://jc.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ip.jctech888.com.cn

[R59] 发 POST JSON
来源：http://gm.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sf.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://xk.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oh.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://fb.hnjuh.cn

df -h;  du -sh *
来源：http://kq.newstarts.cn

[R62] 找最占空间的文件
来源：http://ub.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://lb.shxzskj.cn

[R63] 内存与进程
来源：http://fd.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://vj.shtwfgs.cn

[R64] 结束进程
来源：http://bp.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://bj.521024.cn

[R65] 查看端口占用
来源：http://mv.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aq.muxihuayi.cn

[R66] 定时任务
来源：http://ln.jctech888.com.cn

crontab -e;  crontab -l
来源：http://ds.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://gv.panjiajie.cn

openssl rand -hex 16
来源：http://sl.521024.cn

[R68] 计算文件校验值
来源：http://ms.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zd.9csxet.cn

[R69] 生成随机密码
来源：http://ux.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://xe.chemitech.net.cn

[R70] 时间戳与互转
来源：http://af.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://zk.bjjhwx.cn

[R71] 日期格式化
来源：http://dq.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sr.nicolike.cn

[R72] 等待端口就绪
来源：http://he.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ml.wgjwhj.cn

[R73] 分割大日志
来源：http://xx.gzmigu.cn

split -l 1000 big.log part_
来源：http://it.shxzskj.cn

[R74] 批量重命名
来源：http://sq.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kt.wgjwhj.cn

[R75] 导出环境变量
来源：http://hu.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://ii.haigaiapp.cn

[R76] 使用临时文件
来源：http://xv.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oa.panjiajie.cn

[R77] 读取用户输入
来源：http://vb.shtwfgs.cn

read -rp "请输入: " ans
来源：http://ed.wgjwhj.cn

[R78] 交互式菜单
来源：http://mv.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uy.chemitech.net.cn

[R79] 解析命令行选项
来源：http://ag.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gm.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://jy.panjiajie.cn

time ./run.sh
来源：http://ej.yuntaijiaju.cn

================================================================================
来源：http://ea.panjiajie.cn

S. C / C++ 专题
来源：http://zo.newstarts.cn

================================================================================
来源：http://ta.jctech888.com.cn

[S01] C：Hello World
来源：http://nn.bjjhwx.cn

#include <stdio.h>
来源：http://sh.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kx.huanxung.cn

[S02] C：变量与格式化输出
来源：http://xe.521024.cn

int a = 10; printf("%d\n", a);
来源：http://xf.chemitech.net.cn

[S03] C：读入整数
来源：http://gw.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://xe.hnjuh.cn

[S04] C：字符串复制
来源：http://sl.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qg.nszjky.cn

[S05] C：字符串长度
来源：http://ky.haigaiapp.cn

strlen(s)
来源：http://wd.gzmigu.cn

[S06] C：字符串比较
来源：http://tz.wgjwhj.cn

strcmp(a, b) == 0
来源：http://ve.szxytkj.cn

[S07] C：数组遍历求和
来源：http://kk.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wy.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://vl.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gi.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://lg.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nc.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://um.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://gc.521024.cn

[S11] C：逐行读文件
来源：http://vw.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://qg.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ps.huanxung.cn

fclose(f);
来源：http://yk.asd995.cn

[S12] C：写文件
来源：http://ug.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gw.gzmigu.cn

[S13] C：宏定义
来源：http://mz.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rl.hahajie.cn

[S14] C：枚举
来源：http://cm.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://uv.shtwfgs.cn

[S15] C：类型转换
来源：http://gs.gzmigu.cn

(double) a / b
来源：http://rr.colortex.cn

[S16] C：位操作置位
来源：http://jg.lnxyls.cn

x |= (1 << 3);
来源：http://bc.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://ph.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kl.nszjky.cn

[S18] C：命令行参数
来源：http://aa.bjjhwx.cn

int main(int argc, char **argv)
来源：http://bs.hahajie.cn

[S19] C：快速排序
来源：http://qu.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qv.asd995.cn

[S20] C：二分查找
来源：http://nd.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://we.huanxung.cn

[S21] C：字符类别判断
来源：http://px.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ka.nszjky.cn

[S22] C：字符串转数字
来源：http://ie.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pn.huixiangedu.cn

[S23] C：随机数
来源：http://jm.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnjuh.cn

[S24] C：获取本地时间
来源：http://fi.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kx.9csxet.cn

[S25] C：内存拷贝
来源：http://rg.newstarts.cn

memcpy(dst, src, n);
来源：http://dd.huixiangedu.cn

[S26] C：内存清零
来源：http://ba.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://jd.newstarts.cn

[S27] C：定义常量
来源：http://ge.lnxyls.cn

const double PI = 3.14159;
来源：http://yj.shtwfgs.cn

[S28] C：静态变量
来源：http://va.szsharing.cn

static int counter = 0;
来源：http://fk.shxzukj.cn

[S29] C：变参函数
来源：http://jh.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wc.huanxung.cn

[S30] C：头文件保护
来源：http://dy.huixiangedu.cn

#ifndef X_H
来源：http://io.chemitech.net.cn

#define X_H
来源：http://lw.nszjky.cn

#endif
来源：http://if.panjiajie.cn

[S31] C++：Hello World
来源：http://kk.hahajie.cn

#include <iostream>
来源：http://az.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://fg.colortex.cn

[S32] C++：字符串
来源：http://bh.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://bz.jctech888.com.cn

[S33] C++：vector 增删
来源：http://nb.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rg.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://qi.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://kg.9csxet.cn

[S35] C++：map
来源：http://xm.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vn.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://pt.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pp.shxzukj.cn

[S37] C++：set
来源：http://vl.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gg.hnjuh.cn

[S38] C++：排序
来源：http://hg.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://rn.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://up.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bv.shtwfgs.cn

[S40] C++：查找元素
来源：http://be.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vu.colortex.cn

[S41] C++：类与构造函数
来源：http://pn.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gt.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://za.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://qo.huanxung.cn

[S43] C++：智能指针
来源：http://yi.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://jf.521024.cn

[S44] C++：引用传参
来源：http://sk.nszjky.cn

void inc(int &x) { ++x; }
来源：http://cm.bookmarksfly.cn

[S45] C++：lambda
来源：http://ng.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cn.shxzskj.cn

[S46] C++：函数模板
来源：http://ge.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jp.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://ve.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ym.hahajie.cn

[S48] C++：逐行读文件
来源：http://rg.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bx.521024.cn

while (std::getline(in, line)) { }
来源：http://xg.shtwfgs.cn

[S49] C++：写文件
来源：http://rk.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zq.asd995.cn

[S50] C++：格式化数字
来源：http://gb.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ro.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://gx.jctech888.com.cn

static_cast<double>(a) / b
来源：http://un.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://ua.huanxung.cn

int size() const noexcept { return n_; }
来源：http://kz.huixiangedu.cn

[S53] C++：移动语义
来源：http://us.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://is.shxzskj.cn

[S54] C++：异常处理
来源：http://zs.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hb.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://lt.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://li.panjiajie.cn

[S56] C++：optional
来源：http://rb.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pm.yuexingan06.cn

[S57] C++：编译期常量
来源：http://lp.yuexingan06.cn

constexpr int N = 10;
来源：http://oh.jctech888.com.cn

[S58] C++：命名空间
来源：http://yr.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://mn.hahajie.cn

[S59] C++：静态断言
来源：http://xu.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dj.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://ug.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cr.szsharing.cn

================================================================================
来源：http://nr.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eu.shxzukj.cn

================================================================================
来源：http://xk.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://zm.bookmarksfly.cn

println("Hello")
来源：http://pg.521024.cn

[T02] Kotlin：变量
来源：http://pp.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fn.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://mo.nicolike.cn

"值: $b"
来源：http://ne.lnxyls.cn

[T04] Kotlin：空安全
来源：http://xb.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://ib.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://vu.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gr.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://nj.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ne.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://lp.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://da.colortex.cn

[T08] Kotlin：数据类
来源：http://ui.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ah.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://dg.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://zn.hahajie.cn

[T10] Kotlin：默认参数
来源：http://ra.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pm.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://qn.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oj.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://lg.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://la.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://pe.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://ce.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://ni.szxytkj.cn

for (i in 1..10) println(i)
来源：http://um.shxzskj.cn


<!-- 参考信息 -->