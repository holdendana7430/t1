代发 wailian999

case "$1" in
来源：http://pd.panjiajie.cn

start) echo "启动" ;;
来源：http://ee.szsharing.cn

stop)  echo "停止" ;;
来源：http://cq.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://fj.colortex.cn

esac
来源：http://li.nicolike.cn

[R12] for 遍历文件
来源：http://jw.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://ub.asd995.cn

[R13] for 计数循环
来源：http://ei.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://wa.szxytkj.cn

[R14] C 风格 for
来源：http://xv.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nz.521024.cn

[R15] while 逐行读文件
来源：http://rb.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xw.huixinmuqiang.cn

[R16] until 等待条件
来源：http://tz.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qw.asd995.cn

[R17] 数组定义与取值
来源：http://fp.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mu.nicolike.cn

[R18] 遍历数组
来源：http://tg.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://at.9csxet.cn

[R19] 数组长度
来源：http://vw.chemitech.net.cn

echo "${#arr[@]}"
来源：http://cy.asd995.cn

[R20] 关联数组（字典）
来源：http://nt.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://be.chemitech.net.cn

[R21] 字符串长度
来源：http://xe.bookmarksfly.cn

echo "${#s}"
来源：http://ce.newstarts.cn

[R22] 截取子串
来源：http://dj.newstarts.cn

echo "${s:0:5}"
来源：http://sm.panjiajie.cn

[R23] 字符串替换
来源：http://yh.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yq.haigaiapp.cn

[R24] 大小写转换
来源：http://ex.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wd.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://kr.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cf.shtwfgs.cn

[R26] 命令替换
来源：http://jo.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://nu.9csxet.cn

[R27] 算术展开
来源：http://zy.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://la.huixinmuqiang.cn

[R28] 浮点运算
来源：http://rd.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://fy.yuexingan06.cn

[R29] 定义函数
来源：http://sb.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ec.chemitech.net.cn

[R30] 函数返回状态码
来源：http://wm.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://sn.asd995.cn

[R31] 局部变量
来源：http://px.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://iz.panjiajie.cn

[R32] 参数个数校验
来源：http://px.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qd.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://qm.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mg.521024.cn

[R34] 退出时清理
来源：http://ak.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://we.haigaiapp.cn

[R35] 后台执行并等待
来源：http://tk.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lb.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://zv.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ss.colortex.cn

[R37] 把输出赋给变量
来源：http://fu.szsharing.cn

files=$(ls -1)
来源：http://ej.chemitech.net.cn

[R38] 管道串联
来源：http://fz.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://qd.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://jf.szxytkj.cn

cmd > out.log 2>&1
来源：http://et.huixiangedu.cn

[R40] 追加写日志
来源：http://gl.gzmigu.cn

echo "log" >> out.log
来源：http://fi.chemitech.net.cn

[R41] 丢弃输出
来源：http://vs.9csxet.cn

cmd >/dev/null 2>&1
来源：http://af.shxzukj.cn

[R42] 输入重定向
来源：http://gi.nszjky.cn

wc -l < a.txt
来源：http://md.wgjwhj.cn

[R43] 按名字查找文件
来源：http://qy.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://fj.huanxung.cn

[R44] 按修改时间查找
来源：http://gr.9csxet.cn

find . -mtime -7 -type f
来源：http://hw.asd995.cn

[R45] 批量删除
来源：http://kl.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://qe.9csxet.cn

[R46] 递归替换文件内容
来源：http://yb.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wl.jctech888.com.cn

[R47] sed 单行替换
来源：http://hd.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jf.muxihuayi.cn

[R48] awk 取指定列
来源：http://jg.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://am.jianghongdianzi.cn

[R49] awk 带条件
来源：http://rf.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tn.szsharing.cn

[R50] awk 求和
来源：http://cu.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hx.wgjwhj.cn

[R51] 排序去重取前几
来源：http://dk.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ez.huixinmuqiang.cn

[R52] 统计行数
来源：http://du.gzmigu.cn

wc -l a.txt
来源：http://fi.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://dc.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sx.shxzskj.cn

[R54] 比较两个文件
来源：http://sx.jianghongdianzi.cn

diff a.txt b.txt
来源：http://lo.shtwfgs.cn

[R55] 压缩与解压
来源：http://hj.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zi.shxzukj.cn

[R56] 远程拷贝
来源：http://ek.szsharing.cn

scp file user@host:/path/
来源：http://fz.colortex.cn

[R57] 远程执行命令
来源：http://fv.gzmigu.cn

ssh user@host 'uptime'
来源：http://vb.nicolike.cn

[R58] 下载文件
来源：http://sa.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lo.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://nh.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ab.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://oe.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cl.shxzskj.cn

[R61] 磁盘占用
来源：http://mp.shtwfgs.cn

df -h;  du -sh *
来源：http://tk.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://wj.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://gf.yuexingan06.cn

[R63] 内存与进程
来源：http://js.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://gu.huanxung.cn

[R64] 结束进程
来源：http://bj.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://qq.bookmarksfly.cn

[R65] 查看端口占用
来源：http://xi.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ie.jianghongdianzi.cn

[R66] 定时任务
来源：http://tn.huanxung.cn

crontab -e;  crontab -l
来源：http://jd.9csxet.cn

[R67] 生成随机十六进制串
来源：http://ro.szxytkj.cn

openssl rand -hex 16
来源：http://wb.haigaiapp.cn

[R68] 计算文件校验值
来源：http://bh.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jz.521024.cn

[R69] 生成随机密码
来源：http://tu.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://lp.panjiajie.cn

[R70] 时间戳与互转
来源：http://qf.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://yl.nszjky.cn

[R71] 日期格式化
来源：http://by.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hq.yuexingan06.cn

[R72] 等待端口就绪
来源：http://zd.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rl.hahajie.cn

[R73] 分割大日志
来源：http://ms.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://rg.hnjuh.cn

[R74] 批量重命名
来源：http://ru.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oe.asd995.cn

[R75] 导出环境变量
来源：http://lj.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://qs.colortex.cn

[R76] 使用临时文件
来源：http://vo.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pn.lnxyls.cn

[R77] 读取用户输入
来源：http://ne.shxzskj.cn

read -rp "请输入: " ans
来源：http://xe.gzmigu.cn

[R78] 交互式菜单
来源：http://so.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eg.colortex.cn

[R79] 解析命令行选项
来源：http://ie.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://og.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://kp.huixinmuqiang.cn

time ./run.sh
来源：http://zu.colortex.cn

================================================================================
来源：http://bk.panjiajie.cn

S. C / C++ 专题
来源：http://vx.jctech888.com.cn

================================================================================
来源：http://mm.hahajie.cn

[S01] C：Hello World
来源：http://oi.haigaiapp.cn

#include <stdio.h>
来源：http://wf.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qs.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://zj.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://jv.yuexingan06.cn

[S03] C：读入整数
来源：http://wb.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://bf.wgjwhj.cn

[S04] C：字符串复制
来源：http://kd.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fi.huixiangedu.cn

[S05] C：字符串长度
来源：http://zz.huixinmuqiang.cn

strlen(s)
来源：http://rg.muxihuayi.cn

[S06] C：字符串比较
来源：http://sd.gzmigu.cn

strcmp(a, b) == 0
来源：http://st.panjiajie.cn

[S07] C：数组遍历求和
来源：http://oq.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tf.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://bg.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ux.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://md.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yn.newstarts.cn

[S10] C：指针与解引用
来源：http://ko.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://is.shxzskj.cn

[S11] C：逐行读文件
来源：http://ki.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://ci.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://et.yuntaijiaju.cn

fclose(f);
来源：http://ur.haigaiapp.cn

[S12] C：写文件
来源：http://dj.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eg.huixinmuqiang.cn

[S13] C：宏定义
来源：http://ws.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ja.chemitech.net.cn

[S14] C：枚举
来源：http://um.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://zn.nszjky.cn

[S15] C：类型转换
来源：http://zy.yuntaijiaju.cn

(double) a / b
来源：http://mi.yuexingan06.cn

[S16] C：位操作置位
来源：http://mc.szsharing.cn

x |= (1 << 3);
来源：http://kx.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://ig.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dk.muxihuayi.cn

[S18] C：命令行参数
来源：http://ns.9csxet.cn

int main(int argc, char **argv)
来源：http://pm.haigaiapp.cn

[S19] C：快速排序
来源：http://br.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wd.521024.cn

[S20] C：二分查找
来源：http://xf.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ad.wgjwhj.cn

[S21] C：字符类别判断
来源：http://cj.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lw.hahajie.cn

[S22] C：字符串转数字
来源：http://fx.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oi.yuntaijiaju.cn

[S23] C：随机数
来源：http://qc.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ph.wgjwhj.cn

[S24] C：获取本地时间
来源：http://qg.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zf.bjjhwx.cn

[S25] C：内存拷贝
来源：http://bp.szxytkj.cn

memcpy(dst, src, n);
来源：http://so.haigaiapp.cn

[S26] C：内存清零
来源：http://co.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://hz.huanxung.cn

[S27] C：定义常量
来源：http://wh.nszjky.cn

const double PI = 3.14159;
来源：http://gv.huixinmuqiang.cn

[S28] C：静态变量
来源：http://sh.jctech888.com.cn

static int counter = 0;
来源：http://hs.jianghongdianzi.cn

[S29] C：变参函数
来源：http://sh.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dj.hnjuh.cn

[S30] C：头文件保护
来源：http://kl.nszjky.cn

#ifndef X_H
来源：http://zy.yuntaijiaju.cn

#define X_H
来源：http://hh.jianghongdianzi.cn

#endif
来源：http://ht.nszjky.cn

[S31] C++：Hello World
来源：http://hm.shxzukj.cn

#include <iostream>
来源：http://qy.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://kt.yuntaijiaju.cn

[S32] C++：字符串
来源：http://fb.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://th.hahajie.cn

[S33] C++：vector 增删
来源：http://my.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ll.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://rm.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://ja.huixiangedu.cn

[S35] C++：map
来源：http://aa.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jz.521024.cn

[S36] C++：unordered_map
来源：http://ga.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ep.huixinmuqiang.cn

[S37] C++：set
来源：http://dc.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qk.muxihuayi.cn

[S38] C++：排序
来源：http://fm.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://wc.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://vx.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dc.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://zt.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fq.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://za.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vu.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://vu.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://wa.yuexingan06.cn

[S43] C++：智能指针
来源：http://nl.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://eh.gzmigu.cn

[S44] C++：引用传参
来源：http://ne.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://wa.szxytkj.cn

[S45] C++：lambda
来源：http://tm.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hb.hnjuh.cn

[S46] C++：函数模板
来源：http://ia.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ok.521024.cn

[S47] C++：结构化绑定遍历
来源：http://ep.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://td.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://cx.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zp.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://iz.nszjky.cn

[S49] C++：写文件
来源：http://vk.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://be.szxytkj.cn

[S50] C++：格式化数字
来源：http://at.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lu.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://vo.shtwfgs.cn

static_cast<double>(a) / b
来源：http://sh.asd995.cn

[S52] C++：const 与 noexcept
来源：http://fx.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://fp.nicolike.cn

[S53] C++：移动语义
来源：http://ic.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://un.shtwfgs.cn

[S54] C++：异常处理
来源：http://vi.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ns.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://ps.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mx.muxihuayi.cn

[S56] C++：optional
来源：http://pd.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qh.9csxet.cn

[S57] C++：编译期常量
来源：http://hx.shtwfgs.cn

constexpr int N = 10;
来源：http://cr.huanxung.cn

[S58] C++：命名空间
来源：http://xk.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://bg.nicolike.cn

[S59] C++：静态断言
来源：http://wh.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bd.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://hk.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sn.colortex.cn

================================================================================
来源：http://qg.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lu.muxihuayi.cn

================================================================================
来源：http://zk.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://gq.lnxyls.cn

println("Hello")
来源：http://bb.newstarts.cn

[T02] Kotlin：变量
来源：http://ux.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uv.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://gu.hahajie.cn

"值: $b"
来源：http://yy.hahajie.cn

[T04] Kotlin：空安全
来源：http://va.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://tx.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://fo.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ob.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://ij.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cu.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://qq.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zu.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://sx.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://rp.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://uv.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://jo.szsharing.cn

[T10] Kotlin：默认参数
来源：http://zk.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hd.shxzukj.cn

[T11] Kotlin：协程
来源：http://kz.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vc.hahajie.cn

[T12] Kotlin：解构声明
来源：http://jq.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://sb.colortex.cn


<!-- 参考信息 -->