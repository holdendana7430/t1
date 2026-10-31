代发 wailian999

case "$1" in
来源：http://iv.hnjuh.cn

start) echo "启动" ;;
来源：http://td.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://pz.szsharing.cn

*)     echo "未知命令" ;;
来源：http://uc.shxzskj.cn

esac
来源：http://hw.shxzukj.cn

[R12] for 遍历文件
来源：http://og.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://qh.yuntaijiaju.cn

[R13] for 计数循环
来源：http://tm.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://nl.wgjwhj.cn

[R14] C 风格 for
来源：http://zu.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hq.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://jk.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://so.wgjwhj.cn

[R16] until 等待条件
来源：http://fr.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kd.521024.cn

[R17] 数组定义与取值
来源：http://kd.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yx.chemitech.net.cn

[R18] 遍历数组
来源：http://tu.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rp.shxzskj.cn

[R19] 数组长度
来源：http://bc.chemitech.net.cn

echo "${#arr[@]}"
来源：http://vs.asd995.cn

[R20] 关联数组（字典）
来源：http://tq.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ed.hnjuh.cn

[R21] 字符串长度
来源：http://ty.shxzskj.cn

echo "${#s}"
来源：http://gq.9csxet.cn

[R22] 截取子串
来源：http://ox.521024.cn

echo "${s:0:5}"
来源：http://uk.jctech888.com.cn

[R23] 字符串替换
来源：http://hc.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kt.yuexingan06.cn

[R24] 大小写转换
来源：http://mt.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pr.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://mv.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tn.9csxet.cn

[R26] 命令替换
来源：http://iw.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://tx.lnxyls.cn

[R27] 算术展开
来源：http://ei.szsharing.cn

echo $((1 + 2 * 3))
来源：http://ix.szxytkj.cn

[R28] 浮点运算
来源：http://lk.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://ri.shtwfgs.cn

[R29] 定义函数
来源：http://sd.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jq.lnxyls.cn

[R30] 函数返回状态码
来源：http://jh.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://hg.jianghongdianzi.cn

[R31] 局部变量
来源：http://be.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://kv.bjjhwx.cn

[R32] 参数个数校验
来源：http://eb.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sr.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://do.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gp.9csxet.cn

[R34] 退出时清理
来源：http://be.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vg.shxzskj.cn

[R35] 后台执行并等待
来源：http://fx.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ah.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://hd.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yj.hnjuh.cn

[R37] 把输出赋给变量
来源：http://iz.szsharing.cn

files=$(ls -1)
来源：http://gl.colortex.cn

[R38] 管道串联
来源：http://sc.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://ou.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://my.9csxet.cn

cmd > out.log 2>&1
来源：http://ui.shtwfgs.cn

[R40] 追加写日志
来源：http://mi.huanxung.cn

echo "log" >> out.log
来源：http://gb.9csxet.cn

[R41] 丢弃输出
来源：http://er.newstarts.cn

cmd >/dev/null 2>&1
来源：http://zf.chemitech.net.cn

[R42] 输入重定向
来源：http://us.jctech888.com.cn

wc -l < a.txt
来源：http://gw.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://pz.gzmigu.cn

find . -name "*.log" -type f
来源：http://pu.asd995.cn

[R44] 按修改时间查找
来源：http://bj.bjjhwx.cn

find . -mtime -7 -type f
来源：http://pe.nicolike.cn

[R45] 批量删除
来源：http://np.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://cn.lnxyls.cn

[R46] 递归替换文件内容
来源：http://vo.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fp.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://op.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ki.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://jb.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://sj.shtwfgs.cn

[R49] awk 带条件
来源：http://li.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://at.wgjwhj.cn

[R50] awk 求和
来源：http://la.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uc.lnxyls.cn

[R51] 排序去重取前几
来源：http://cy.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hx.panjiajie.cn

[R52] 统计行数
来源：http://mi.colortex.cn

wc -l a.txt
来源：http://gn.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://qg.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kg.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://et.nszjky.cn

diff a.txt b.txt
来源：http://xw.huixiangedu.cn

[R55] 压缩与解压
来源：http://jr.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fl.asd995.cn

[R56] 远程拷贝
来源：http://fv.yuexingan06.cn

scp file user@host:/path/
来源：http://ur.muxihuayi.cn

[R57] 远程执行命令
来源：http://em.huixiangedu.cn

ssh user@host 'uptime'
来源：http://zg.panjiajie.cn

[R58] 下载文件
来源：http://wj.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tk.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://yh.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kk.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://vq.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oe.nicolike.cn

[R61] 磁盘占用
来源：http://cm.haigaiapp.cn

df -h;  du -sh *
来源：http://mg.szxytkj.cn

[R62] 找最占空间的文件
来源：http://pz.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://tb.jianghongdianzi.cn

[R63] 内存与进程
来源：http://ot.asd995.cn

free -h;  ps aux | grep nginx
来源：http://jk.hnjuh.cn

[R64] 结束进程
来源：http://ow.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://oc.hahajie.cn

[R65] 查看端口占用
来源：http://xr.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cz.asd995.cn

[R66] 定时任务
来源：http://uy.colortex.cn

crontab -e;  crontab -l
来源：http://ac.521024.cn

[R67] 生成随机十六进制串
来源：http://un.jctech888.com.cn

openssl rand -hex 16
来源：http://uu.shtwfgs.cn

[R68] 计算文件校验值
来源：http://ew.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ui.asd995.cn

[R69] 生成随机密码
来源：http://yo.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://zz.yuexingan06.cn

[R70] 时间戳与互转
来源：http://xz.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://yy.szxytkj.cn

[R71] 日期格式化
来源：http://dd.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jp.shxzskj.cn

[R72] 等待端口就绪
来源：http://mf.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jl.haigaiapp.cn

[R73] 分割大日志
来源：http://gc.nicolike.cn

split -l 1000 big.log part_
来源：http://st.huixiangedu.cn

[R74] 批量重命名
来源：http://qw.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cl.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://kd.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://qf.asd995.cn

[R76] 使用临时文件
来源：http://oa.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://am.huixiangedu.cn

[R77] 读取用户输入
来源：http://mr.hahajie.cn

read -rp "请输入: " ans
来源：http://cx.huixiangedu.cn

[R78] 交互式菜单
来源：http://bx.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wv.hahajie.cn

[R79] 解析命令行选项
来源：http://fs.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cz.521024.cn

[R80] 查看脚本执行耗时
来源：http://fb.bjjhwx.cn

time ./run.sh
来源：http://fc.shxzskj.cn

================================================================================
来源：http://kq.chemitech.net.cn

S. C / C++ 专题
来源：http://pr.hnjuh.cn

================================================================================
来源：http://kr.panjiajie.cn

[S01] C：Hello World
来源：http://qj.haigaiapp.cn

#include <stdio.h>
来源：http://tu.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zc.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://ru.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://bl.huanxung.cn

[S03] C：读入整数
来源：http://lu.nszjky.cn

int x; scanf("%d", &x);
来源：http://lc.nicolike.cn

[S04] C：字符串复制
来源：http://eg.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://id.szxytkj.cn

[S05] C：字符串长度
来源：http://xi.haigaiapp.cn

strlen(s)
来源：http://rx.gzmigu.cn

[S06] C：字符串比较
来源：http://zl.hnjuh.cn

strcmp(a, b) == 0
来源：http://vz.colortex.cn

[S07] C：数组遍历求和
来源：http://nj.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sx.521024.cn

[S08] C：动态内存分配与释放
来源：http://xn.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kk.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://do.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zt.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://tj.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://pn.9csxet.cn

[S11] C：逐行读文件
来源：http://cc.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://ox.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zs.nicolike.cn

fclose(f);
来源：http://yx.lnxyls.cn

[S12] C：写文件
来源：http://co.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kg.yuntaijiaju.cn

[S13] C：宏定义
来源：http://wy.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kq.huixinmuqiang.cn

[S14] C：枚举
来源：http://mm.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://lq.shxzukj.cn

[S15] C：类型转换
来源：http://sx.hahajie.cn

(double) a / b
来源：http://yn.newstarts.cn

[S16] C：位操作置位
来源：http://dk.newstarts.cn

x |= (1 << 3);
来源：http://my.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://uw.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zt.bookmarksfly.cn

[S18] C：命令行参数
来源：http://qi.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://ig.yuntaijiaju.cn

[S19] C：快速排序
来源：http://sq.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://df.shxzukj.cn

[S20] C：二分查找
来源：http://xq.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vd.colortex.cn

[S21] C：字符类别判断
来源：http://zj.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xa.newstarts.cn

[S22] C：字符串转数字
来源：http://ne.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aq.huixiangedu.cn

[S23] C：随机数
来源：http://mp.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fc.colortex.cn

[S24] C：获取本地时间
来源：http://sx.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gi.nicolike.cn

[S25] C：内存拷贝
来源：http://cx.szsharing.cn

memcpy(dst, src, n);
来源：http://ps.521024.cn

[S26] C：内存清零
来源：http://dc.huanxung.cn

memset(a, 0, sizeof a);
来源：http://fu.gzmigu.cn

[S27] C：定义常量
来源：http://bd.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://kk.panjiajie.cn

[S28] C：静态变量
来源：http://dy.asd995.cn

static int counter = 0;
来源：http://qi.muxihuayi.cn

[S29] C：变参函数
来源：http://wi.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ko.chemitech.net.cn

[S30] C：头文件保护
来源：http://zw.yuntaijiaju.cn

#ifndef X_H
来源：http://zn.asd995.cn

#define X_H
来源：http://jf.hnjuh.cn

#endif
来源：http://ky.huanxung.cn

[S31] C++：Hello World
来源：http://op.shxzukj.cn

#include <iostream>
来源：http://ae.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://ec.colortex.cn

[S32] C++：字符串
来源：http://gw.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://cc.huanxung.cn

[S33] C++：vector 增删
来源：http://ue.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://so.szxytkj.cn

[S34] C++：遍历 vector
来源：http://ja.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://rg.bookmarksfly.cn

[S35] C++：map
来源：http://mb.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bj.wgjwhj.cn

[S36] C++：unordered_map
来源：http://ib.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ul.szsharing.cn

[S37] C++：set
来源：http://ub.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vr.yuntaijiaju.cn

[S38] C++：排序
来源：http://gf.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://lg.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://le.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dr.newstarts.cn

[S40] C++：查找元素
来源：http://gf.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wc.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://yj.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://re.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://nl.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://mo.chemitech.net.cn

[S43] C++：智能指针
来源：http://mb.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://qc.521024.cn

[S44] C++：引用传参
来源：http://xx.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://zk.bjjhwx.cn

[S45] C++：lambda
来源：http://lw.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hs.hnjuh.cn

[S46] C++：函数模板
来源：http://sz.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zs.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://do.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://et.hnjuh.cn

[S48] C++：逐行读文件
来源：http://hu.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iw.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://zd.colortex.cn

[S49] C++：写文件
来源：http://xu.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ye.wgjwhj.cn

[S50] C++：格式化数字
来源：http://ds.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xd.shxzskj.cn

[S51] C++：显式类型转换
来源：http://dp.chemitech.net.cn

static_cast<double>(a) / b
来源：http://cl.521024.cn

[S52] C++：const 与 noexcept
来源：http://wb.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://ax.shxzskj.cn

[S53] C++：移动语义
来源：http://st.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://yu.huanxung.cn

[S54] C++：异常处理
来源：http://xo.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://km.shxzukj.cn

[S55] C++：结构化绑定
来源：http://zc.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zm.hnjuh.cn

[S56] C++：optional
来源：http://vb.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://os.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://kl.jianghongdianzi.cn

constexpr int N = 10;
来源：http://dj.szsharing.cn

[S58] C++：命名空间
来源：http://ep.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://ho.lnxyls.cn

[S59] C++：静态断言
来源：http://kh.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ol.colortex.cn

[S60] C++：遍历并删除元素
来源：http://ga.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rv.jctech888.com.cn

================================================================================
来源：http://ws.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wl.shtwfgs.cn

================================================================================
来源：http://tl.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://qi.huixinmuqiang.cn

println("Hello")
来源：http://mf.9csxet.cn

[T02] Kotlin：变量
来源：http://vq.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xk.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://by.hnjuh.cn

"值: $b"
来源：http://fm.521024.cn

[T04] Kotlin：空安全
来源：http://tw.panjiajie.cn

val n: String? = null;  n?.length
来源：http://yj.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://nz.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wg.szsharing.cn

[T06] Kotlin：集合映射
来源：http://ey.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pz.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://gp.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lh.hahajie.cn

[T08] Kotlin：数据类
来源：http://gl.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://gj.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://ho.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://ju.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://fc.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mq.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ys.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://md.nszjky.cn

[T12] Kotlin：解构声明
来源：http://kx.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://bj.9csxet.cn


<!-- 参考信息 -->