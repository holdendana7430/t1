代发 wailian999

case "$1" in
来源：http://vy.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://zb.gzmigu.cn

stop)  echo "停止" ;;
来源：http://sh.hahajie.cn

*)     echo "未知命令" ;;
来源：http://px.nszjky.cn

esac
来源：http://yh.nicolike.cn

[R12] for 遍历文件
来源：http://pn.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://bo.asd995.cn

[R13] for 计数循环
来源：http://pw.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://mg.521024.cn

[R14] C 风格 for
来源：http://dc.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jv.nszjky.cn

[R15] while 逐行读文件
来源：http://ov.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sp.gzmigu.cn

[R16] until 等待条件
来源：http://ju.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bw.gzmigu.cn

[R17] 数组定义与取值
来源：http://ft.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qh.bjjhwx.cn

[R18] 遍历数组
来源：http://lh.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ot.hahajie.cn

[R19] 数组长度
来源：http://ms.muxihuayi.cn

echo "${#arr[@]}"
来源：http://vu.colortex.cn

[R20] 关联数组（字典）
来源：http://bg.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ug.huixiangedu.cn

[R21] 字符串长度
来源：http://xu.9csxet.cn

echo "${#s}"
来源：http://rn.shxzskj.cn

[R22] 截取子串
来源：http://fy.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://xj.shxzskj.cn

[R23] 字符串替换
来源：http://uv.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ei.panjiajie.cn

[R24] 大小写转换
来源：http://we.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://at.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://yv.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xy.newstarts.cn

[R26] 命令替换
来源：http://xf.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://of.shxzukj.cn

[R27] 算术展开
来源：http://ao.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://pu.huixinmuqiang.cn

[R28] 浮点运算
来源：http://wj.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://ce.yuntaijiaju.cn

[R29] 定义函数
来源：http://lt.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hl.shxzukj.cn

[R30] 函数返回状态码
来源：http://en.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://fr.wgjwhj.cn

[R31] 局部变量
来源：http://ri.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://sq.shxzukj.cn

[R32] 参数个数校验
来源：http://lm.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cm.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://gr.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yq.gzmigu.cn

[R34] 退出时清理
来源：http://ky.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uq.shxzskj.cn

[R35] 后台执行并等待
来源：http://dj.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jb.panjiajie.cn

[R36] 并发执行多个任务
来源：http://gg.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ol.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://fo.huanxung.cn

files=$(ls -1)
来源：http://vs.jctech888.com.cn

[R38] 管道串联
来源：http://xc.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://nr.521024.cn

[R39] 重定向标准输出与错误
来源：http://rq.shtwfgs.cn

cmd > out.log 2>&1
来源：http://ha.haigaiapp.cn

[R40] 追加写日志
来源：http://bb.nszjky.cn

echo "log" >> out.log
来源：http://jj.muxihuayi.cn

[R41] 丢弃输出
来源：http://at.hahajie.cn

cmd >/dev/null 2>&1
来源：http://rw.asd995.cn

[R42] 输入重定向
来源：http://ez.shtwfgs.cn

wc -l < a.txt
来源：http://so.szsharing.cn

[R43] 按名字查找文件
来源：http://pk.haigaiapp.cn

find . -name "*.log" -type f
来源：http://ak.chemitech.net.cn

[R44] 按修改时间查找
来源：http://na.yuexingan06.cn

find . -mtime -7 -type f
来源：http://ft.jctech888.com.cn

[R45] 批量删除
来源：http://xl.colortex.cn

find . -name "*.tmp" -delete
来源：http://jo.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://ll.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nj.yuexingan06.cn

[R47] sed 单行替换
来源：http://qx.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bb.9csxet.cn

[R48] awk 取指定列
来源：http://fe.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://ao.huixinmuqiang.cn

[R49] awk 带条件
来源：http://pl.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ww.shtwfgs.cn

[R50] awk 求和
来源：http://zs.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vc.hnjuh.cn

[R51] 排序去重取前几
来源：http://pi.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xc.hnjuh.cn

[R52] 统计行数
来源：http://se.jctech888.com.cn

wc -l a.txt
来源：http://hi.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://su.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tn.521024.cn

[R54] 比较两个文件
来源：http://ae.shxzukj.cn

diff a.txt b.txt
来源：http://wv.nszjky.cn

[R55] 压缩与解压
来源：http://jl.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ta.9csxet.cn

[R56] 远程拷贝
来源：http://je.gzmigu.cn

scp file user@host:/path/
来源：http://cp.haigaiapp.cn

[R57] 远程执行命令
来源：http://mc.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ob.gzmigu.cn

[R58] 下载文件
来源：http://xx.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vf.shxzskj.cn

[R59] 发 POST JSON
来源：http://dr.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xv.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://gf.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wh.gzmigu.cn

[R61] 磁盘占用
来源：http://vg.asd995.cn

df -h;  du -sh *
来源：http://xn.shxzukj.cn

[R62] 找最占空间的文件
来源：http://wg.asd995.cn

du -ah . | sort -rh | head -10
来源：http://sy.hahajie.cn

[R63] 内存与进程
来源：http://bs.colortex.cn

free -h;  ps aux | grep nginx
来源：http://fs.521024.cn

[R64] 结束进程
来源：http://or.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://oo.huixiangedu.cn

[R65] 查看端口占用
来源：http://ic.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gc.asd995.cn

[R66] 定时任务
来源：http://zi.9csxet.cn

crontab -e;  crontab -l
来源：http://ty.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://du.panjiajie.cn

openssl rand -hex 16
来源：http://if.jctech888.com.cn

[R68] 计算文件校验值
来源：http://tf.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ll.haigaiapp.cn

[R69] 生成随机密码
来源：http://go.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://oy.asd995.cn

[R70] 时间戳与互转
来源：http://aw.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://ey.huanxung.cn

[R71] 日期格式化
来源：http://vt.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nc.9csxet.cn

[R72] 等待端口就绪
来源：http://pd.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jl.nszjky.cn

[R73] 分割大日志
来源：http://ux.bjjhwx.cn

split -l 1000 big.log part_
来源：http://os.chemitech.net.cn

[R74] 批量重命名
来源：http://kg.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cb.newstarts.cn

[R75] 导出环境变量
来源：http://qt.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://hx.hnjuh.cn

[R76] 使用临时文件
来源：http://ec.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wy.wgjwhj.cn

[R77] 读取用户输入
来源：http://rv.chemitech.net.cn

read -rp "请输入: " ans
来源：http://ok.muxihuayi.cn

[R78] 交互式菜单
来源：http://ac.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pr.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://tm.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vv.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://bf.szsharing.cn

time ./run.sh
来源：http://ov.huixiangedu.cn

================================================================================
来源：http://vw.wgjwhj.cn

S. C / C++ 专题
来源：http://ab.huixinmuqiang.cn

================================================================================
来源：http://vn.yuexingan06.cn

[S01] C：Hello World
来源：http://mq.shtwfgs.cn

#include <stdio.h>
来源：http://zv.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ik.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://hd.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://xy.9csxet.cn

[S03] C：读入整数
来源：http://ms.nicolike.cn

int x; scanf("%d", &x);
来源：http://ny.shtwfgs.cn

[S04] C：字符串复制
来源：http://kz.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yi.shtwfgs.cn

[S05] C：字符串长度
来源：http://ny.panjiajie.cn

strlen(s)
来源：http://xx.muxihuayi.cn

[S06] C：字符串比较
来源：http://fx.hahajie.cn

strcmp(a, b) == 0
来源：http://os.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://ns.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mw.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://gh.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ju.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://on.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ii.chemitech.net.cn

[S10] C：指针与解引用
来源：http://lp.newstarts.cn

int *p = &a;  *p = 5;
来源：http://gn.9csxet.cn

[S11] C：逐行读文件
来源：http://zm.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://hx.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rw.panjiajie.cn

fclose(f);
来源：http://ut.huixinmuqiang.cn

[S12] C：写文件
来源：http://cn.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tw.haigaiapp.cn

[S13] C：宏定义
来源：http://mm.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cu.jctech888.com.cn

[S14] C：枚举
来源：http://ce.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://wh.panjiajie.cn

[S15] C：类型转换
来源：http://dn.panjiajie.cn

(double) a / b
来源：http://mb.shxzskj.cn

[S16] C：位操作置位
来源：http://yv.yuexingan06.cn

x |= (1 << 3);
来源：http://xd.szsharing.cn

[S17] C：安全拼接字符串
来源：http://bt.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ps.haigaiapp.cn

[S18] C：命令行参数
来源：http://sw.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://ny.yuexingan06.cn

[S19] C：快速排序
来源：http://mx.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lf.asd995.cn

[S20] C：二分查找
来源：http://hh.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bh.chemitech.net.cn

[S21] C：字符类别判断
来源：http://mn.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ke.shxzskj.cn

[S22] C：字符串转数字
来源：http://dj.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://di.nicolike.cn

[S23] C：随机数
来源：http://ev.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qu.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://ix.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cs.muxihuayi.cn

[S25] C：内存拷贝
来源：http://xz.shtwfgs.cn

memcpy(dst, src, n);
来源：http://ml.jctech888.com.cn

[S26] C：内存清零
来源：http://ei.hahajie.cn

memset(a, 0, sizeof a);
来源：http://vx.muxihuayi.cn

[S27] C：定义常量
来源：http://bc.lnxyls.cn

const double PI = 3.14159;
来源：http://yc.shtwfgs.cn

[S28] C：静态变量
来源：http://jz.chemitech.net.cn

static int counter = 0;
来源：http://vt.szsharing.cn

[S29] C：变参函数
来源：http://ts.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fy.colortex.cn

[S30] C：头文件保护
来源：http://pj.nicolike.cn

#ifndef X_H
来源：http://cu.colortex.cn

#define X_H
来源：http://th.newstarts.cn

#endif
来源：http://rl.nszjky.cn

[S31] C++：Hello World
来源：http://bm.bjjhwx.cn

#include <iostream>
来源：http://dj.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://ei.muxihuayi.cn

[S32] C++：字符串
来源：http://ag.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://ge.muxihuayi.cn

[S33] C++：vector 增删
来源：http://xf.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fv.colortex.cn

[S34] C++：遍历 vector
来源：http://pi.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://me.szxytkj.cn

[S35] C++：map
来源：http://gi.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qj.huanxung.cn

[S36] C++：unordered_map
来源：http://mr.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://if.shxzukj.cn

[S37] C++：set
来源：http://kk.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nw.yuntaijiaju.cn

[S38] C++：排序
来源：http://tr.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://lp.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://kq.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ni.chemitech.net.cn

[S40] C++：查找元素
来源：http://kb.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ma.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://rt.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jl.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://lf.521024.cn

class B : public Base { public: void f() override {} };
来源：http://ps.szxytkj.cn

[S43] C++：智能指针
来源：http://rl.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://zy.asd995.cn

[S44] C++：引用传参
来源：http://md.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://xe.huixinmuqiang.cn

[S45] C++：lambda
来源：http://am.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yc.szxytkj.cn

[S46] C++：函数模板
来源：http://aa.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dq.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://ni.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vi.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://do.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kl.nicolike.cn

while (std::getline(in, line)) { }
来源：http://ir.jianghongdianzi.cn

[S49] C++：写文件
来源：http://im.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://no.yuexingan06.cn

[S50] C++：格式化数字
来源：http://kb.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tv.panjiajie.cn

[S51] C++：显式类型转换
来源：http://gt.shxzskj.cn

static_cast<double>(a) / b
来源：http://jd.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://or.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://im.chemitech.net.cn

[S53] C++：移动语义
来源：http://yi.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://nh.newstarts.cn

[S54] C++：异常处理
来源：http://yo.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://in.nicolike.cn

[S55] C++：结构化绑定
来源：http://ji.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cc.hnjuh.cn

[S56] C++：optional
来源：http://en.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yf.muxihuayi.cn

[S57] C++：编译期常量
来源：http://hz.shxzukj.cn

constexpr int N = 10;
来源：http://fr.huixiangedu.cn

[S58] C++：命名空间
来源：http://pp.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://iz.szsharing.cn

[S59] C++：静态断言
来源：http://vq.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qg.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://on.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ym.szsharing.cn

================================================================================
来源：http://xc.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cs.panjiajie.cn

================================================================================
来源：http://nx.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://nx.muxihuayi.cn

println("Hello")
来源：http://rm.panjiajie.cn

[T02] Kotlin：变量
来源：http://lw.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ht.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://vl.shxzskj.cn

"值: $b"
来源：http://jv.hahajie.cn

[T04] Kotlin：空安全
来源：http://rg.szsharing.cn

val n: String? = null;  n?.length
来源：http://yc.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://vh.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lz.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://oh.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rq.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://cz.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mc.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://yd.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://ee.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://fe.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://xt.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://gh.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hm.szsharing.cn

[T11] Kotlin：协程
来源：http://bq.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kg.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://iq.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://ro.newstarts.cn


<!-- 参考信息 -->