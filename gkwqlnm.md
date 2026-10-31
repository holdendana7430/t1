代发 wailian999

case "$1" in
来源：http://sq.haigaiapp.cn

start) echo "启动" ;;
来源：http://iu.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://on.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://vy.colortex.cn

esac
来源：http://tm.bjjhwx.cn

[R12] for 遍历文件
来源：http://on.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://kp.shtwfgs.cn

[R13] for 计数循环
来源：http://si.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://lf.szsharing.cn

[R14] C 风格 for
来源：http://cf.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rj.hnjuh.cn

[R15] while 逐行读文件
来源：http://vz.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://og.lnxyls.cn

[R16] until 等待条件
来源：http://js.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xn.huanxung.cn

[R17] 数组定义与取值
来源：http://ii.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bg.szsharing.cn

[R18] 遍历数组
来源：http://gr.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ph.hnjuh.cn

[R19] 数组长度
来源：http://au.newstarts.cn

echo "${#arr[@]}"
来源：http://le.hahajie.cn

[R20] 关联数组（字典）
来源：http://gt.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sd.chemitech.net.cn

[R21] 字符串长度
来源：http://ix.hahajie.cn

echo "${#s}"
来源：http://le.yuntaijiaju.cn

[R22] 截取子串
来源：http://uw.huixiangedu.cn

echo "${s:0:5}"
来源：http://lg.huixiangedu.cn

[R23] 字符串替换
来源：http://ui.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oo.jianghongdianzi.cn

[R24] 大小写转换
来源：http://oc.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ef.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://js.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dw.nszjky.cn

[R26] 命令替换
来源：http://lp.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://rs.wgjwhj.cn

[R27] 算术展开
来源：http://kh.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://vk.huixinmuqiang.cn

[R28] 浮点运算
来源：http://vt.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://kn.panjiajie.cn

[R29] 定义函数
来源：http://vb.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://os.panjiajie.cn

[R30] 函数返回状态码
来源：http://lw.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://zn.yuexingan06.cn

[R31] 局部变量
来源：http://to.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://mb.jctech888.com.cn

[R32] 参数个数校验
来源：http://sf.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xl.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://pr.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://su.hahajie.cn

[R34] 退出时清理
来源：http://bj.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zr.haigaiapp.cn

[R35] 后台执行并等待
来源：http://mz.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cg.shxzskj.cn

[R36] 并发执行多个任务
来源：http://lg.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ak.hnjuh.cn

[R37] 把输出赋给变量
来源：http://oo.yuntaijiaju.cn

files=$(ls -1)
来源：http://se.haigaiapp.cn

[R38] 管道串联
来源：http://ca.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://mh.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://xe.9csxet.cn

cmd > out.log 2>&1
来源：http://jh.newstarts.cn

[R40] 追加写日志
来源：http://qy.chemitech.net.cn

echo "log" >> out.log
来源：http://ak.szsharing.cn

[R41] 丢弃输出
来源：http://zo.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://wm.shxzukj.cn

[R42] 输入重定向
来源：http://zz.gzmigu.cn

wc -l < a.txt
来源：http://xh.chemitech.net.cn

[R43] 按名字查找文件
来源：http://ga.shxzukj.cn

find . -name "*.log" -type f
来源：http://on.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://yl.nszjky.cn

find . -mtime -7 -type f
来源：http://tr.gzmigu.cn

[R45] 批量删除
来源：http://pl.asd995.cn

find . -name "*.tmp" -delete
来源：http://ld.asd995.cn

[R46] 递归替换文件内容
来源：http://lv.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pf.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://jl.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qw.nicolike.cn

[R48] awk 取指定列
来源：http://db.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://jp.haigaiapp.cn

[R49] awk 带条件
来源：http://vd.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hf.jctech888.com.cn

[R50] awk 求和
来源：http://ur.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tb.shxzskj.cn

[R51] 排序去重取前几
来源：http://je.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ya.shxzukj.cn

[R52] 统计行数
来源：http://dp.haigaiapp.cn

wc -l a.txt
来源：http://es.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://yb.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lz.haigaiapp.cn

[R54] 比较两个文件
来源：http://lf.szsharing.cn

diff a.txt b.txt
来源：http://ca.huanxung.cn

[R55] 压缩与解压
来源：http://le.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vx.9csxet.cn

[R56] 远程拷贝
来源：http://jv.gzmigu.cn

scp file user@host:/path/
来源：http://jo.shtwfgs.cn

[R57] 远程执行命令
来源：http://jz.chemitech.net.cn

ssh user@host 'uptime'
来源：http://tt.521024.cn

[R58] 下载文件
来源：http://kg.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zd.lnxyls.cn

[R59] 发 POST JSON
来源：http://qj.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lu.521024.cn

[R60] 只看 HTTP 状态码
来源：http://wk.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yg.gzmigu.cn

[R61] 磁盘占用
来源：http://qo.521024.cn

df -h;  du -sh *
来源：http://mq.szxytkj.cn

[R62] 找最占空间的文件
来源：http://ir.colortex.cn

du -ah . | sort -rh | head -10
来源：http://up.521024.cn

[R63] 内存与进程
来源：http://ur.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://sc.newstarts.cn

[R64] 结束进程
来源：http://pk.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://ho.jctech888.com.cn

[R65] 查看端口占用
来源：http://sx.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cj.panjiajie.cn

[R66] 定时任务
来源：http://pj.haigaiapp.cn

crontab -e;  crontab -l
来源：http://it.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://qh.bjjhwx.cn

openssl rand -hex 16
来源：http://ul.shtwfgs.cn

[R68] 计算文件校验值
来源：http://dw.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bi.nicolike.cn

[R69] 生成随机密码
来源：http://zh.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://ti.yuexingan06.cn

[R70] 时间戳与互转
来源：http://rf.colortex.cn

date +%s;  date -d @1700000000
来源：http://tz.9csxet.cn

[R71] 日期格式化
来源：http://ww.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tf.hahajie.cn

[R72] 等待端口就绪
来源：http://hp.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ji.bookmarksfly.cn

[R73] 分割大日志
来源：http://ck.yuexingan06.cn

split -l 1000 big.log part_
来源：http://dm.hnjuh.cn

[R74] 批量重命名
来源：http://ek.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xl.haigaiapp.cn

[R75] 导出环境变量
来源：http://xv.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://ak.huixiangedu.cn

[R76] 使用临时文件
来源：http://ej.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fi.haigaiapp.cn

[R77] 读取用户输入
来源：http://ci.asd995.cn

read -rp "请输入: " ans
来源：http://ht.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://uh.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tf.asd995.cn

[R79] 解析命令行选项
来源：http://sg.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tg.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://re.chemitech.net.cn

time ./run.sh
来源：http://xc.hahajie.cn

================================================================================
来源：http://rv.shxzukj.cn

S. C / C++ 专题
来源：http://jj.9csxet.cn

================================================================================
来源：http://ay.huixinmuqiang.cn

[S01] C：Hello World
来源：http://ad.wgjwhj.cn

#include <stdio.h>
来源：http://qe.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zm.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://fv.521024.cn

int a = 10; printf("%d\n", a);
来源：http://ud.521024.cn

[S03] C：读入整数
来源：http://yj.hahajie.cn

int x; scanf("%d", &x);
来源：http://jn.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://xq.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://re.nszjky.cn

[S05] C：字符串长度
来源：http://ck.yuntaijiaju.cn

strlen(s)
来源：http://fh.szxytkj.cn

[S06] C：字符串比较
来源：http://ad.muxihuayi.cn

strcmp(a, b) == 0
来源：http://on.panjiajie.cn

[S07] C：数组遍历求和
来源：http://tq.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bm.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://vl.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qi.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://ct.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bh.shxzukj.cn

[S10] C：指针与解引用
来源：http://gy.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://tk.9csxet.cn

[S11] C：逐行读文件
来源：http://fs.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://zz.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mt.gzmigu.cn

fclose(f);
来源：http://zc.hnjuh.cn

[S12] C：写文件
来源：http://hm.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yz.9csxet.cn

[S13] C：宏定义
来源：http://zw.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nl.huixinmuqiang.cn

[S14] C：枚举
来源：http://kt.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://am.colortex.cn

[S15] C：类型转换
来源：http://sv.yuntaijiaju.cn

(double) a / b
来源：http://cu.newstarts.cn

[S16] C：位操作置位
来源：http://vc.asd995.cn

x |= (1 << 3);
来源：http://yz.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://jq.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ez.szxytkj.cn

[S18] C：命令行参数
来源：http://xx.hnjuh.cn

int main(int argc, char **argv)
来源：http://fb.bookmarksfly.cn

[S19] C：快速排序
来源：http://wr.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ll.521024.cn

[S20] C：二分查找
来源：http://tb.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vf.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://yf.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vq.haigaiapp.cn

[S22] C：字符串转数字
来源：http://fu.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jn.colortex.cn

[S23] C：随机数
来源：http://ob.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ec.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://ih.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://he.panjiajie.cn

[S25] C：内存拷贝
来源：http://oz.asd995.cn

memcpy(dst, src, n);
来源：http://yu.nszjky.cn

[S26] C：内存清零
来源：http://nf.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://go.hnjuh.cn

[S27] C：定义常量
来源：http://qy.shxzukj.cn

const double PI = 3.14159;
来源：http://mc.9csxet.cn

[S28] C：静态变量
来源：http://qv.shxzskj.cn

static int counter = 0;
来源：http://do.haigaiapp.cn

[S29] C：变参函数
来源：http://fk.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kr.nszjky.cn

[S30] C：头文件保护
来源：http://fw.newstarts.cn

#ifndef X_H
来源：http://yf.huixiangedu.cn

#define X_H
来源：http://ce.bjjhwx.cn

#endif
来源：http://zx.newstarts.cn

[S31] C++：Hello World
来源：http://lw.haigaiapp.cn

#include <iostream>
来源：http://rn.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://fr.chemitech.net.cn

[S32] C++：字符串
来源：http://ni.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://id.gzmigu.cn

[S33] C++：vector 增删
来源：http://ie.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iw.nicolike.cn

[S34] C++：遍历 vector
来源：http://un.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://af.bjjhwx.cn

[S35] C++：map
来源：http://sb.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dq.panjiajie.cn

[S36] C++：unordered_map
来源：http://gd.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kh.9csxet.cn

[S37] C++：set
来源：http://hp.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dt.huanxung.cn

[S38] C++：排序
来源：http://zb.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://ef.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://ot.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ot.bookmarksfly.cn

[S40] C++：查找元素
来源：http://qe.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yf.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://ql.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ad.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://vx.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://qx.9csxet.cn

[S43] C++：智能指针
来源：http://mt.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://ng.521024.cn

[S44] C++：引用传参
来源：http://rv.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://bi.yuexingan06.cn

[S45] C++：lambda
来源：http://yq.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dh.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://kx.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ie.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://sd.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://za.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://js.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lk.9csxet.cn

while (std::getline(in, line)) { }
来源：http://zq.bjjhwx.cn

[S49] C++：写文件
来源：http://zc.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ik.gzmigu.cn

[S50] C++：格式化数字
来源：http://bm.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rt.nicolike.cn

[S51] C++：显式类型转换
来源：http://fr.bjjhwx.cn

static_cast<double>(a) / b
来源：http://lq.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://sm.hahajie.cn

int size() const noexcept { return n_; }
来源：http://ms.9csxet.cn

[S53] C++：移动语义
来源：http://hk.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://ey.newstarts.cn

[S54] C++：异常处理
来源：http://ux.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://po.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://ta.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ld.521024.cn

[S56] C++：optional
来源：http://qk.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tk.521024.cn

[S57] C++：编译期常量
来源：http://jn.newstarts.cn

constexpr int N = 10;
来源：http://sm.bookmarksfly.cn

[S58] C++：命名空间
来源：http://br.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://gs.huixiangedu.cn

[S59] C++：静态断言
来源：http://av.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xi.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://fi.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://az.huanxung.cn

================================================================================
来源：http://hh.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://es.haigaiapp.cn

================================================================================
来源：http://za.9csxet.cn

[T01] Kotlin：Hello World
来源：http://fy.9csxet.cn

println("Hello")
来源：http://bm.jctech888.com.cn

[T02] Kotlin：变量
来源：http://ku.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jq.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://uy.huixinmuqiang.cn

"值: $b"
来源：http://ns.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://cz.521024.cn

val n: String? = null;  n?.length
来源：http://ue.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://qu.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vu.colortex.cn

[T06] Kotlin：集合映射
来源：http://if.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jp.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://va.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sm.shxzukj.cn

[T08] Kotlin：数据类
来源：http://ku.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://bv.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://qv.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://hs.newstarts.cn

[T10] Kotlin：默认参数
来源：http://za.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bx.colortex.cn

[T11] Kotlin：协程
来源：http://zz.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uq.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://ah.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://wr.newstarts.cn


<!-- 参考信息 -->