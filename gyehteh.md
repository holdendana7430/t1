代发 wailian999

case "$1" in
来源：http://ay.chemitech.net.cn

start) echo "启动" ;;
来源：http://ko.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://yt.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://la.huixiangedu.cn

esac
来源：http://of.shtwfgs.cn

[R12] for 遍历文件
来源：http://bs.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://tp.panjiajie.cn

[R13] for 计数循环
来源：http://gc.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://vx.panjiajie.cn

[R14] C 风格 for
来源：http://ll.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fy.gzmigu.cn

[R15] while 逐行读文件
来源：http://ep.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ou.huanxung.cn

[R16] until 等待条件
来源：http://ww.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ca.haigaiapp.cn

[R17] 数组定义与取值
来源：http://on.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hd.bookmarksfly.cn

[R18] 遍历数组
来源：http://am.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kk.gzmigu.cn

[R19] 数组长度
来源：http://sx.lnxyls.cn

echo "${#arr[@]}"
来源：http://ms.szxytkj.cn

[R20] 关联数组（字典）
来源：http://rx.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jg.bookmarksfly.cn

[R21] 字符串长度
来源：http://nk.gzmigu.cn

echo "${#s}"
来源：http://fm.muxihuayi.cn

[R22] 截取子串
来源：http://ox.jctech888.com.cn

echo "${s:0:5}"
来源：http://dt.wgjwhj.cn

[R23] 字符串替换
来源：http://mn.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ur.asd995.cn

[R24] 大小写转换
来源：http://qs.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qd.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://pb.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://am.muxihuayi.cn

[R26] 命令替换
来源：http://pw.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://up.bookmarksfly.cn

[R27] 算术展开
来源：http://nb.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://fh.521024.cn

[R28] 浮点运算
来源：http://xs.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://ir.hnjuh.cn

[R29] 定义函数
来源：http://rg.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://df.hahajie.cn

[R30] 函数返回状态码
来源：http://xp.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://yw.bjjhwx.cn

[R31] 局部变量
来源：http://vs.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://em.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://qr.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://co.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://xf.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ej.shxzskj.cn

[R34] 退出时清理
来源：http://hv.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dc.jctech888.com.cn

[R35] 后台执行并等待
来源：http://yr.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vl.shxzskj.cn

[R36] 并发执行多个任务
来源：http://zc.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wt.gzmigu.cn

[R37] 把输出赋给变量
来源：http://oc.jctech888.com.cn

files=$(ls -1)
来源：http://he.wgjwhj.cn

[R38] 管道串联
来源：http://zq.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://jr.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://dv.huanxung.cn

cmd > out.log 2>&1
来源：http://pm.yuntaijiaju.cn

[R40] 追加写日志
来源：http://hi.panjiajie.cn

echo "log" >> out.log
来源：http://xd.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://gk.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://ne.shxzskj.cn

[R42] 输入重定向
来源：http://ao.shxzskj.cn

wc -l < a.txt
来源：http://ap.colortex.cn

[R43] 按名字查找文件
来源：http://ud.yuexingan06.cn

find . -name "*.log" -type f
来源：http://hu.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://fq.huixiangedu.cn

find . -mtime -7 -type f
来源：http://hx.gzmigu.cn

[R45] 批量删除
来源：http://lh.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://bh.panjiajie.cn

[R46] 递归替换文件内容
来源：http://qz.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ms.9csxet.cn

[R47] sed 单行替换
来源：http://pl.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hj.panjiajie.cn

[R48] awk 取指定列
来源：http://zk.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://tg.panjiajie.cn

[R49] awk 带条件
来源：http://rz.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nd.huanxung.cn

[R50] awk 求和
来源：http://lg.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jb.nicolike.cn

[R51] 排序去重取前几
来源：http://ph.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pq.huanxung.cn

[R52] 统计行数
来源：http://wu.hahajie.cn

wc -l a.txt
来源：http://ug.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://zo.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gv.jctech888.com.cn

[R54] 比较两个文件
来源：http://sv.9csxet.cn

diff a.txt b.txt
来源：http://zr.nszjky.cn

[R55] 压缩与解压
来源：http://hk.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cf.nicolike.cn

[R56] 远程拷贝
来源：http://wx.shxzskj.cn

scp file user@host:/path/
来源：http://mm.nicolike.cn

[R57] 远程执行命令
来源：http://ly.521024.cn

ssh user@host 'uptime'
来源：http://cs.lnxyls.cn

[R58] 下载文件
来源：http://hb.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hb.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://qi.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cs.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://qg.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ed.gzmigu.cn

[R61] 磁盘占用
来源：http://jf.haigaiapp.cn

df -h;  du -sh *
来源：http://vs.huanxung.cn

[R62] 找最占空间的文件
来源：http://bh.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://fk.szsharing.cn

[R63] 内存与进程
来源：http://gq.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://rf.szxytkj.cn

[R64] 结束进程
来源：http://jb.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://ks.hahajie.cn

[R65] 查看端口占用
来源：http://ft.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ua.jctech888.com.cn

[R66] 定时任务
来源：http://qn.shxzskj.cn

crontab -e;  crontab -l
来源：http://up.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://xd.wgjwhj.cn

openssl rand -hex 16
来源：http://td.szsharing.cn

[R68] 计算文件校验值
来源：http://tb.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pz.wgjwhj.cn

[R69] 生成随机密码
来源：http://ym.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://pj.lnxyls.cn

[R70] 时间戳与互转
来源：http://ii.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://es.hnjuh.cn

[R71] 日期格式化
来源：http://fs.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nf.szxytkj.cn

[R72] 等待端口就绪
来源：http://ha.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gh.hnjuh.cn

[R73] 分割大日志
来源：http://ha.gzmigu.cn

split -l 1000 big.log part_
来源：http://vn.lnxyls.cn

[R74] 批量重命名
来源：http://kw.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cy.lnxyls.cn

[R75] 导出环境变量
来源：http://ia.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://dl.bjjhwx.cn

[R76] 使用临时文件
来源：http://ab.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ui.bookmarksfly.cn

[R77] 读取用户输入
来源：http://hb.hnjuh.cn

read -rp "请输入: " ans
来源：http://jt.521024.cn

[R78] 交互式菜单
来源：http://vs.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dk.yuexingan06.cn

[R79] 解析命令行选项
来源：http://zc.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rj.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://wh.shtwfgs.cn

time ./run.sh
来源：http://mu.newstarts.cn

================================================================================
来源：http://gg.bookmarksfly.cn

S. C / C++ 专题
来源：http://an.lnxyls.cn

================================================================================
来源：http://kg.lnxyls.cn

[S01] C：Hello World
来源：http://iv.huixiangedu.cn

#include <stdio.h>
来源：http://lo.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hd.szsharing.cn

[S02] C：变量与格式化输出
来源：http://bk.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://mv.wgjwhj.cn

[S03] C：读入整数
来源：http://jh.szsharing.cn

int x; scanf("%d", &x);
来源：http://jq.szxytkj.cn

[S04] C：字符串复制
来源：http://mc.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sw.hahajie.cn

[S05] C：字符串长度
来源：http://vg.jctech888.com.cn

strlen(s)
来源：http://ty.nszjky.cn

[S06] C：字符串比较
来源：http://vc.gzmigu.cn

strcmp(a, b) == 0
来源：http://do.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://mq.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cm.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://mm.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qg.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://qd.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://su.jctech888.com.cn

[S10] C：指针与解引用
来源：http://xa.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://fx.hahajie.cn

[S11] C：逐行读文件
来源：http://jz.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://xu.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://of.asd995.cn

fclose(f);
来源：http://bx.hnjuh.cn

[S12] C：写文件
来源：http://jq.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gj.yuexingan06.cn

[S13] C：宏定义
来源：http://tf.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gr.muxihuayi.cn

[S14] C：枚举
来源：http://jk.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://oa.szsharing.cn

[S15] C：类型转换
来源：http://jd.9csxet.cn

(double) a / b
来源：http://mp.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://fm.bookmarksfly.cn

x |= (1 << 3);
来源：http://hh.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://ka.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hv.nicolike.cn

[S18] C：命令行参数
来源：http://cb.bjjhwx.cn

int main(int argc, char **argv)
来源：http://xy.huixiangedu.cn

[S19] C：快速排序
来源：http://kh.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mb.nicolike.cn

[S20] C：二分查找
来源：http://xp.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bw.yuexingan06.cn

[S21] C：字符类别判断
来源：http://my.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ey.gzmigu.cn

[S22] C：字符串转数字
来源：http://al.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hx.nszjky.cn

[S23] C：随机数
来源：http://po.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://in.hnjuh.cn

[S24] C：获取本地时间
来源：http://wf.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zj.newstarts.cn

[S25] C：内存拷贝
来源：http://il.hahajie.cn

memcpy(dst, src, n);
来源：http://al.wgjwhj.cn

[S26] C：内存清零
来源：http://eo.asd995.cn

memset(a, 0, sizeof a);
来源：http://sj.huanxung.cn

[S27] C：定义常量
来源：http://he.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://ds.huixiangedu.cn

[S28] C：静态变量
来源：http://rv.huixinmuqiang.cn

static int counter = 0;
来源：http://lq.nszjky.cn

[S29] C：变参函数
来源：http://uv.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hp.nszjky.cn

[S30] C：头文件保护
来源：http://ng.wgjwhj.cn

#ifndef X_H
来源：http://za.bookmarksfly.cn

#define X_H
来源：http://lx.newstarts.cn

#endif
来源：http://km.haigaiapp.cn

[S31] C++：Hello World
来源：http://ky.bookmarksfly.cn

#include <iostream>
来源：http://ez.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://sl.shxzskj.cn

[S32] C++：字符串
来源：http://lq.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://zc.gzmigu.cn

[S33] C++：vector 增删
来源：http://lv.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pn.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://yo.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://ta.panjiajie.cn

[S35] C++：map
来源：http://ym.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://av.bjjhwx.cn

[S36] C++：unordered_map
来源：http://ti.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ga.jctech888.com.cn

[S37] C++：set
来源：http://ed.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dh.nszjky.cn

[S38] C++：排序
来源：http://tt.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://bi.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://kv.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bs.szxytkj.cn

[S40] C++：查找元素
来源：http://jz.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lx.szsharing.cn

[S41] C++：类与构造函数
来源：http://wi.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rs.9csxet.cn

[S42] C++：继承与虚函数
来源：http://qy.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://ta.shxzskj.cn

[S43] C++：智能指针
来源：http://dr.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://ba.haigaiapp.cn

[S44] C++：引用传参
来源：http://bq.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://yx.hnjuh.cn

[S45] C++：lambda
来源：http://yi.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pr.asd995.cn

[S46] C++：函数模板
来源：http://tl.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eg.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://rq.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ak.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://ih.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sl.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://pz.shxzukj.cn

[S49] C++：写文件
来源：http://nx.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hw.nszjky.cn

[S50] C++：格式化数字
来源：http://uz.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mj.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://ix.haigaiapp.cn

static_cast<double>(a) / b
来源：http://dp.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://dk.asd995.cn

int size() const noexcept { return n_; }
来源：http://wl.huanxung.cn

[S53] C++：移动语义
来源：http://dx.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://xo.colortex.cn

[S54] C++：异常处理
来源：http://ch.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://da.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://dz.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yu.muxihuayi.cn

[S56] C++：optional
来源：http://ya.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eh.panjiajie.cn

[S57] C++：编译期常量
来源：http://qc.bookmarksfly.cn

constexpr int N = 10;
来源：http://rn.huanxung.cn

[S58] C++：命名空间
来源：http://wg.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://cu.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://ad.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aw.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://gr.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://en.hahajie.cn

================================================================================
来源：http://dj.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mp.nicolike.cn

================================================================================
来源：http://zx.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://zl.shtwfgs.cn

println("Hello")
来源：http://dz.bjjhwx.cn

[T02] Kotlin：变量
来源：http://ef.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oq.521024.cn

[T03] Kotlin：字符串模板
来源：http://pv.muxihuayi.cn

"值: $b"
来源：http://mr.szsharing.cn

[T04] Kotlin：空安全
来源：http://ri.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://os.colortex.cn

[T05] Kotlin：when 表达式
来源：http://rr.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qq.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://nd.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jm.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://ti.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://er.panjiajie.cn

[T08] Kotlin：数据类
来源：http://aw.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://nz.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://ms.521024.cn

fun String.exclaim() = this + "!"
来源：http://yc.huanxung.cn

[T10] Kotlin：默认参数
来源：http://jk.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dk.haigaiapp.cn

[T11] Kotlin：协程
来源：http://vw.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ne.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://wz.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://ys.huixiangedu.cn


<!-- 参考信息 -->