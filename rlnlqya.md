代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://te.szsharing.cn

[R10] 正则匹配
来源：http://tv.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gj.nszjky.cn

[R11] case 多分支
来源：http://ye.panjiajie.cn

case "$1" in
来源：http://vw.szsharing.cn

start) echo "启动" ;;
来源：http://we.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://hz.huanxung.cn

*)     echo "未知命令" ;;
来源：http://bp.521024.cn

esac
来源：http://aq.muxihuayi.cn

[R12] for 遍历文件
来源：http://ti.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://iq.szsharing.cn

[R13] for 计数循环
来源：http://gw.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://yd.huixinmuqiang.cn

[R14] C 风格 for
来源：http://bs.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mo.shxzukj.cn

[R15] while 逐行读文件
来源：http://rk.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nk.yuexingan06.cn

[R16] until 等待条件
来源：http://zb.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ak.9csxet.cn

[R17] 数组定义与取值
来源：http://yr.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sn.panjiajie.cn

[R18] 遍历数组
来源：http://dd.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rb.haigaiapp.cn

[R19] 数组长度
来源：http://le.9csxet.cn

echo "${#arr[@]}"
来源：http://xq.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://dy.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mt.shxzukj.cn

[R21] 字符串长度
来源：http://tf.asd995.cn

echo "${#s}"
来源：http://pf.hahajie.cn

[R22] 截取子串
来源：http://oi.szsharing.cn

echo "${s:0:5}"
来源：http://yr.lnxyls.cn

[R23] 字符串替换
来源：http://sy.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fh.nicolike.cn

[R24] 大小写转换
来源：http://qp.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xl.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://jl.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://li.shxzskj.cn

[R26] 命令替换
来源：http://ak.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://vo.bjjhwx.cn

[R27] 算术展开
来源：http://bl.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://wo.9csxet.cn

[R28] 浮点运算
来源：http://gq.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://ci.huixiangedu.cn

[R29] 定义函数
来源：http://wh.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iw.nszjky.cn

[R30] 函数返回状态码
来源：http://ba.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://dz.jianghongdianzi.cn

[R31] 局部变量
来源：http://le.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://oy.521024.cn

[R32] 参数个数校验
来源：http://cs.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jd.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://qn.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zu.lnxyls.cn

[R34] 退出时清理
来源：http://lb.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cn.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://ar.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dy.huanxung.cn

[R36] 并发执行多个任务
来源：http://up.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yd.szxytkj.cn

[R37] 把输出赋给变量
来源：http://jh.wgjwhj.cn

files=$(ls -1)
来源：http://hq.shtwfgs.cn

[R38] 管道串联
来源：http://ud.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://zy.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://qc.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://jv.shxzskj.cn

[R40] 追加写日志
来源：http://mr.wgjwhj.cn

echo "log" >> out.log
来源：http://jz.hahajie.cn

[R41] 丢弃输出
来源：http://ct.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://np.bookmarksfly.cn

[R42] 输入重定向
来源：http://mb.huixiangedu.cn

wc -l < a.txt
来源：http://th.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://cm.wgjwhj.cn

find . -name "*.log" -type f
来源：http://nx.colortex.cn

[R44] 按修改时间查找
来源：http://ow.hnjuh.cn

find . -mtime -7 -type f
来源：http://oz.yuntaijiaju.cn

[R45] 批量删除
来源：http://gj.szsharing.cn

find . -name "*.tmp" -delete
来源：http://zi.nszjky.cn

[R46] 递归替换文件内容
来源：http://ky.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rf.wgjwhj.cn

[R47] sed 单行替换
来源：http://dh.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xq.hnjuh.cn

[R48] awk 取指定列
来源：http://fs.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://zo.haigaiapp.cn

[R49] awk 带条件
来源：http://ms.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zx.shxzukj.cn

[R50] awk 求和
来源：http://ey.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ip.shtwfgs.cn

[R51] 排序去重取前几
来源：http://ix.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uu.jctech888.com.cn

[R52] 统计行数
来源：http://oy.szsharing.cn

wc -l a.txt
来源：http://rs.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://tz.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jb.szsharing.cn

[R54] 比较两个文件
来源：http://ty.nicolike.cn

diff a.txt b.txt
来源：http://xj.yuexingan06.cn

[R55] 压缩与解压
来源：http://qm.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zg.wgjwhj.cn

[R56] 远程拷贝
来源：http://tg.szsharing.cn

scp file user@host:/path/
来源：http://go.chemitech.net.cn

[R57] 远程执行命令
来源：http://ze.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://ti.hahajie.cn

[R58] 下载文件
来源：http://ua.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tv.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ko.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sd.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://we.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jr.huanxung.cn

[R61] 磁盘占用
来源：http://lk.newstarts.cn

df -h;  du -sh *
来源：http://bl.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://pj.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://xh.muxihuayi.cn

[R63] 内存与进程
来源：http://da.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://ir.yuntaijiaju.cn

[R64] 结束进程
来源：http://mc.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://lj.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://fo.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://td.shtwfgs.cn

[R66] 定时任务
来源：http://xw.bjjhwx.cn

crontab -e;  crontab -l
来源：http://zc.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://ak.newstarts.cn

openssl rand -hex 16
来源：http://pb.shtwfgs.cn

[R68] 计算文件校验值
来源：http://bz.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oj.yuexingan06.cn

[R69] 生成随机密码
来源：http://of.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://vd.colortex.cn

[R70] 时间戳与互转
来源：http://tb.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://op.szsharing.cn

[R71] 日期格式化
来源：http://cw.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pr.huixiangedu.cn

[R72] 等待端口就绪
来源：http://nf.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sq.chemitech.net.cn

[R73] 分割大日志
来源：http://rz.lnxyls.cn

split -l 1000 big.log part_
来源：http://gr.9csxet.cn

[R74] 批量重命名
来源：http://ag.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wf.bjjhwx.cn

[R75] 导出环境变量
来源：http://jo.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://tc.bjjhwx.cn

[R76] 使用临时文件
来源：http://sk.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ie.huanxung.cn

[R77] 读取用户输入
来源：http://tb.panjiajie.cn

read -rp "请输入: " ans
来源：http://pu.9csxet.cn

[R78] 交互式菜单
来源：http://lk.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ls.hahajie.cn

[R79] 解析命令行选项
来源：http://pq.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vq.asd995.cn

[R80] 查看脚本执行耗时
来源：http://bq.bookmarksfly.cn

time ./run.sh
来源：http://tg.jctech888.com.cn

================================================================================
来源：http://nm.hahajie.cn

S. C / C++ 专题
来源：http://th.wgjwhj.cn

================================================================================
来源：http://zn.bjjhwx.cn

[S01] C：Hello World
来源：http://kq.bookmarksfly.cn

#include <stdio.h>
来源：http://wz.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zv.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://ce.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://iy.muxihuayi.cn

[S03] C：读入整数
来源：http://mj.huanxung.cn

int x; scanf("%d", &x);
来源：http://pm.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://qv.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rs.gzmigu.cn

[S05] C：字符串长度
来源：http://sc.nszjky.cn

strlen(s)
来源：http://lj.colortex.cn

[S06] C：字符串比较
来源：http://fa.yuexingan06.cn

strcmp(a, b) == 0
来源：http://fy.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://gf.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jy.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://db.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nd.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://ig.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tz.shtwfgs.cn

[S10] C：指针与解引用
来源：http://dv.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://pc.asd995.cn

[S11] C：逐行读文件
来源：http://os.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ki.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zq.bookmarksfly.cn

fclose(f);
来源：http://mq.muxihuayi.cn

[S12] C：写文件
来源：http://px.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mm.haigaiapp.cn

[S13] C：宏定义
来源：http://rm.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gj.panjiajie.cn

[S14] C：枚举
来源：http://gy.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://gw.muxihuayi.cn

[S15] C：类型转换
来源：http://rq.shtwfgs.cn

(double) a / b
来源：http://ry.asd995.cn

[S16] C：位操作置位
来源：http://dy.521024.cn

x |= (1 << 3);
来源：http://gt.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://cv.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zb.shxzukj.cn

[S18] C：命令行参数
来源：http://ua.asd995.cn

int main(int argc, char **argv)
来源：http://wh.shxzukj.cn

[S19] C：快速排序
来源：http://xx.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nw.szsharing.cn

[S20] C：二分查找
来源：http://dm.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cv.9csxet.cn

[S21] C：字符类别判断
来源：http://ru.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hy.bjjhwx.cn

[S22] C：字符串转数字
来源：http://tc.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ym.asd995.cn

[S23] C：随机数
来源：http://ye.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kd.shxzskj.cn

[S24] C：获取本地时间
来源：http://yl.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gg.9csxet.cn

[S25] C：内存拷贝
来源：http://ho.szxytkj.cn

memcpy(dst, src, n);
来源：http://yo.panjiajie.cn

[S26] C：内存清零
来源：http://qq.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://zg.huixiangedu.cn

[S27] C：定义常量
来源：http://jf.gzmigu.cn

const double PI = 3.14159;
来源：http://so.huixinmuqiang.cn

[S28] C：静态变量
来源：http://qn.jctech888.com.cn

static int counter = 0;
来源：http://vb.chemitech.net.cn

[S29] C：变参函数
来源：http://qi.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fj.chemitech.net.cn

[S30] C：头文件保护
来源：http://bn.shxzskj.cn

#ifndef X_H
来源：http://px.shxzukj.cn

#define X_H
来源：http://ix.hahajie.cn

#endif
来源：http://vd.bookmarksfly.cn

[S31] C++：Hello World
来源：http://nj.haigaiapp.cn

#include <iostream>
来源：http://jk.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://nh.haigaiapp.cn

[S32] C++：字符串
来源：http://rq.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://df.colortex.cn

[S33] C++：vector 增删
来源：http://hy.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fv.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://nt.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://ae.wgjwhj.cn

[S35] C++：map
来源：http://vf.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lh.huixiangedu.cn

[S36] C++：unordered_map
来源：http://ea.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mv.shxzukj.cn

[S37] C++：set
来源：http://ln.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mx.huanxung.cn

[S38] C++：排序
来源：http://ka.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://tv.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://nh.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ux.hnjuh.cn

[S40] C++：查找元素
来源：http://kt.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yb.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://pj.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hq.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://gg.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://ft.szsharing.cn

[S43] C++：智能指针
来源：http://xr.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://pt.chemitech.net.cn

[S44] C++：引用传参
来源：http://lk.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://wl.jianghongdianzi.cn

[S45] C++：lambda
来源：http://ae.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zh.hahajie.cn

[S46] C++：函数模板
来源：http://yj.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ep.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://pg.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oc.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://kk.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hm.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://dq.jianghongdianzi.cn

[S49] C++：写文件
来源：http://lb.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ib.shxzukj.cn

[S50] C++：格式化数字
来源：http://ik.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ui.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://pn.colortex.cn

static_cast<double>(a) / b
来源：http://iq.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://wt.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://oo.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://ki.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://ux.asd995.cn

[S54] C++：异常处理
来源：http://be.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ne.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://xe.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ib.nszjky.cn

[S56] C++：optional
来源：http://px.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ph.jctech888.com.cn

[S57] C++：编译期常量
来源：http://fi.szxytkj.cn

constexpr int N = 10;
来源：http://ly.asd995.cn

[S58] C++：命名空间
来源：http://qw.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://mm.shxzskj.cn

[S59] C++：静态断言
来源：http://at.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xp.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://ka.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ya.szxytkj.cn

================================================================================
来源：http://ik.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qb.colortex.cn

================================================================================
来源：http://ly.nszjky.cn

[T01] Kotlin：Hello World
来源：http://yn.jctech888.com.cn

println("Hello")
来源：http://lr.colortex.cn

[T02] Kotlin：变量
来源：http://yi.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qh.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://rb.wgjwhj.cn

"值: $b"
来源：http://yy.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://ti.szxytkj.cn

val n: String? = null;  n?.length
来源：http://ge.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://lp.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zy.newstarts.cn

[T06] Kotlin：集合映射
来源：http://at.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dv.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://la.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sv.asd995.cn

[T08] Kotlin：数据类
来源：http://bp.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://fs.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://ku.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://jv.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://rl.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lq.yuexingan06.cn


<!-- 参考信息 -->