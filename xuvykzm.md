代发 wailian999

readonly PI=3.14
来源：http://hp.jianghongdianzi.cn

[R04] 位置参数
来源：http://hb.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fm.shtwfgs.cn

[R05] 参数默认值
来源：http://oe.panjiajie.cn

name="${1:-default}"
来源：http://jd.asd995.cn

[R06] 判断命令是否存在
来源：http://ie.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gc.9csxet.cn

[R07] if 判断文件
来源：http://qw.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bb.bookmarksfly.cn

[R08] 数值比较
来源：http://ru.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fh.shxzskj.cn

[R09] 字符串比较
来源：http://na.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uw.chemitech.net.cn

[R10] 正则匹配
来源：http://re.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ga.shtwfgs.cn

[R11] case 多分支
来源：http://wt.nicolike.cn

case "$1" in
来源：http://ny.muxihuayi.cn

start) echo "启动" ;;
来源：http://lx.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://db.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://ry.9csxet.cn

esac
来源：http://ml.shtwfgs.cn

[R12] for 遍历文件
来源：http://kx.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://xo.hnjuh.cn

[R13] for 计数循环
来源：http://zo.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ro.9csxet.cn

[R14] C 风格 for
来源：http://jw.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uo.asd995.cn

[R15] while 逐行读文件
来源：http://wa.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ro.bjjhwx.cn

[R16] until 等待条件
来源：http://ff.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://av.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://nn.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pa.huanxung.cn

[R18] 遍历数组
来源：http://ay.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zd.shxzskj.cn

[R19] 数组长度
来源：http://bh.yuexingan06.cn

echo "${#arr[@]}"
来源：http://tw.hnjuh.cn

[R20] 关联数组（字典）
来源：http://uq.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kq.jctech888.com.cn

[R21] 字符串长度
来源：http://nz.bookmarksfly.cn

echo "${#s}"
来源：http://ni.szsharing.cn

[R22] 截取子串
来源：http://hh.hahajie.cn

echo "${s:0:5}"
来源：http://sa.bookmarksfly.cn

[R23] 字符串替换
来源：http://mx.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oq.shtwfgs.cn

[R24] 大小写转换
来源：http://tg.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cp.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://tg.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xk.wgjwhj.cn

[R26] 命令替换
来源：http://wc.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://sp.hahajie.cn

[R27] 算术展开
来源：http://ov.hahajie.cn

echo $((1 + 2 * 3))
来源：http://iv.huixiangedu.cn

[R28] 浮点运算
来源：http://ft.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://nu.nicolike.cn

[R29] 定义函数
来源：http://eg.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qm.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://ej.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://zt.nicolike.cn

[R31] 局部变量
来源：http://tg.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://me.bookmarksfly.cn

[R32] 参数个数校验
来源：http://nj.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pq.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://gi.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fr.haigaiapp.cn

[R34] 退出时清理
来源：http://lb.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ap.521024.cn

[R35] 后台执行并等待
来源：http://xn.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qs.colortex.cn

[R36] 并发执行多个任务
来源：http://dv.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yp.shxzskj.cn

[R37] 把输出赋给变量
来源：http://tp.asd995.cn

files=$(ls -1)
来源：http://ns.panjiajie.cn

[R38] 管道串联
来源：http://qc.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://ij.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://xy.nszjky.cn

cmd > out.log 2>&1
来源：http://dd.huanxung.cn

[R40] 追加写日志
来源：http://tz.bookmarksfly.cn

echo "log" >> out.log
来源：http://bw.colortex.cn

[R41] 丢弃输出
来源：http://nn.nszjky.cn

cmd >/dev/null 2>&1
来源：http://kq.yuexingan06.cn

[R42] 输入重定向
来源：http://gl.asd995.cn

wc -l < a.txt
来源：http://ez.szxytkj.cn

[R43] 按名字查找文件
来源：http://zt.gzmigu.cn

find . -name "*.log" -type f
来源：http://ov.shtwfgs.cn

[R44] 按修改时间查找
来源：http://pi.hnjuh.cn

find . -mtime -7 -type f
来源：http://ut.muxihuayi.cn

[R45] 批量删除
来源：http://ir.asd995.cn

find . -name "*.tmp" -delete
来源：http://qr.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://qp.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://co.colortex.cn

[R47] sed 单行替换
来源：http://bn.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iy.bjjhwx.cn

[R48] awk 取指定列
来源：http://mc.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://wd.gzmigu.cn

[R49] awk 带条件
来源：http://ac.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rl.haigaiapp.cn

[R50] awk 求和
来源：http://em.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bw.9csxet.cn

[R51] 排序去重取前几
来源：http://vi.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qn.yuexingan06.cn

[R52] 统计行数
来源：http://iu.nicolike.cn

wc -l a.txt
来源：http://am.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://pu.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rn.szsharing.cn

[R54] 比较两个文件
来源：http://wu.yuexingan06.cn

diff a.txt b.txt
来源：http://em.newstarts.cn

[R55] 压缩与解压
来源：http://kb.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oy.huanxung.cn

[R56] 远程拷贝
来源：http://oa.haigaiapp.cn

scp file user@host:/path/
来源：http://sh.szxytkj.cn

[R57] 远程执行命令
来源：http://ix.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://vz.asd995.cn

[R58] 下载文件
来源：http://os.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ez.chemitech.net.cn

[R59] 发 POST JSON
来源：http://dw.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fx.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://ki.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://if.bjjhwx.cn

[R61] 磁盘占用
来源：http://od.chemitech.net.cn

df -h;  du -sh *
来源：http://lj.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://vq.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://hp.shxzukj.cn

[R63] 内存与进程
来源：http://ub.asd995.cn

free -h;  ps aux | grep nginx
来源：http://ro.521024.cn

[R64] 结束进程
来源：http://tk.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://yy.szsharing.cn

[R65] 查看端口占用
来源：http://wi.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ui.lnxyls.cn

[R66] 定时任务
来源：http://fn.521024.cn

crontab -e;  crontab -l
来源：http://ot.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://nu.huixiangedu.cn

openssl rand -hex 16
来源：http://zb.szxytkj.cn

[R68] 计算文件校验值
来源：http://yy.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nf.nszjky.cn

[R69] 生成随机密码
来源：http://ts.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://rn.bjjhwx.cn

[R70] 时间戳与互转
来源：http://ds.hahajie.cn

date +%s;  date -d @1700000000
来源：http://si.hahajie.cn

[R71] 日期格式化
来源：http://uf.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wn.lnxyls.cn

[R72] 等待端口就绪
来源：http://zv.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cd.hahajie.cn

[R73] 分割大日志
来源：http://ow.szsharing.cn

split -l 1000 big.log part_
来源：http://bh.asd995.cn

[R74] 批量重命名
来源：http://ng.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://up.521024.cn

[R75] 导出环境变量
来源：http://rb.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://wr.szsharing.cn

[R76] 使用临时文件
来源：http://qn.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eb.hnjuh.cn

[R77] 读取用户输入
来源：http://ir.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://tj.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://ue.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xl.szsharing.cn

[R79] 解析命令行选项
来源：http://zo.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nu.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://ff.hahajie.cn

time ./run.sh
来源：http://lx.lnxyls.cn

================================================================================
来源：http://qf.521024.cn

S. C / C++ 专题
来源：http://wh.shtwfgs.cn

================================================================================
来源：http://fg.huixinmuqiang.cn

[S01] C：Hello World
来源：http://lj.hahajie.cn

#include <stdio.h>
来源：http://um.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qr.nicolike.cn

[S02] C：变量与格式化输出
来源：http://uy.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://xk.szsharing.cn

[S03] C：读入整数
来源：http://ux.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://cg.muxihuayi.cn

[S04] C：字符串复制
来源：http://oj.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://br.shxzskj.cn

[S05] C：字符串长度
来源：http://rt.yuexingan06.cn

strlen(s)
来源：http://gc.jctech888.com.cn

[S06] C：字符串比较
来源：http://ka.szxytkj.cn

strcmp(a, b) == 0
来源：http://yj.asd995.cn

[S07] C：数组遍历求和
来源：http://cj.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fu.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://qk.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dc.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://fr.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cd.hahajie.cn

[S10] C：指针与解引用
来源：http://yv.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://as.wgjwhj.cn

[S11] C：逐行读文件
来源：http://vg.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://hl.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vu.bookmarksfly.cn

fclose(f);
来源：http://bo.haigaiapp.cn

[S12] C：写文件
来源：http://uw.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ws.newstarts.cn

[S13] C：宏定义
来源：http://qu.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zd.bjjhwx.cn

[S14] C：枚举
来源：http://fv.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://gj.shxzukj.cn

[S15] C：类型转换
来源：http://gf.szsharing.cn

(double) a / b
来源：http://up.nicolike.cn

[S16] C：位操作置位
来源：http://lb.521024.cn

x |= (1 << 3);
来源：http://kf.asd995.cn

[S17] C：安全拼接字符串
来源：http://jc.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://so.hnjuh.cn

[S18] C：命令行参数
来源：http://je.521024.cn

int main(int argc, char **argv)
来源：http://xa.bjjhwx.cn

[S19] C：快速排序
来源：http://dk.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ik.hahajie.cn

[S20] C：二分查找
来源：http://xf.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wc.gzmigu.cn

[S21] C：字符类别判断
来源：http://eq.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yn.szsharing.cn

[S22] C：字符串转数字
来源：http://cz.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cp.nszjky.cn

[S23] C：随机数
来源：http://xf.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nn.hahajie.cn

[S24] C：获取本地时间
来源：http://cd.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://df.bjjhwx.cn

[S25] C：内存拷贝
来源：http://wy.lnxyls.cn

memcpy(dst, src, n);
来源：http://gu.shxzukj.cn

[S26] C：内存清零
来源：http://wq.asd995.cn

memset(a, 0, sizeof a);
来源：http://yp.yuntaijiaju.cn

[S27] C：定义常量
来源：http://vg.nicolike.cn

const double PI = 3.14159;
来源：http://ej.huixinmuqiang.cn

[S28] C：静态变量
来源：http://xm.9csxet.cn

static int counter = 0;
来源：http://oy.nszjky.cn

[S29] C：变参函数
来源：http://ke.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qv.huixiangedu.cn

[S30] C：头文件保护
来源：http://wo.muxihuayi.cn

#ifndef X_H
来源：http://wc.huanxung.cn

#define X_H
来源：http://kd.bjjhwx.cn

#endif
来源：http://sx.shxzskj.cn

[S31] C++：Hello World
来源：http://wh.yuntaijiaju.cn

#include <iostream>
来源：http://wf.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://eb.muxihuayi.cn

[S32] C++：字符串
来源：http://nf.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://xh.asd995.cn

[S33] C++：vector 增删
来源：http://zv.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fz.newstarts.cn

[S34] C++：遍历 vector
来源：http://il.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://qi.szxytkj.cn

[S35] C++：map
来源：http://pj.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kq.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://dt.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ah.muxihuayi.cn

[S37] C++：set
来源：http://yk.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wx.shtwfgs.cn

[S38] C++：排序
来源：http://oj.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://di.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://rj.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dm.9csxet.cn

[S40] C++：查找元素
来源：http://cu.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wm.panjiajie.cn

[S41] C++：类与构造函数
来源：http://ce.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mg.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://zb.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://nr.colortex.cn

[S43] C++：智能指针
来源：http://rr.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://kp.wgjwhj.cn

[S44] C++：引用传参
来源：http://ht.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://oy.huixiangedu.cn

[S45] C++：lambda
来源：http://zr.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kn.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://og.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ky.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://sn.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oi.9csxet.cn

[S48] C++：逐行读文件
来源：http://bn.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ck.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ez.bookmarksfly.cn

[S49] C++：写文件
来源：http://we.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ue.9csxet.cn

[S50] C++：格式化数字
来源：http://ri.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xm.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://sk.lnxyls.cn

static_cast<double>(a) / b
来源：http://tk.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://sw.521024.cn

int size() const noexcept { return n_; }
来源：http://qc.nszjky.cn

[S53] C++：移动语义
来源：http://dh.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://qe.shxzukj.cn

[S54] C++：异常处理
来源：http://jb.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nc.panjiajie.cn

[S55] C++：结构化绑定
来源：http://sx.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ng.huixinmuqiang.cn

[S56] C++：optional
来源：http://fj.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sj.szxytkj.cn

[S57] C++：编译期常量
来源：http://bl.gzmigu.cn

constexpr int N = 10;
来源：http://kc.chemitech.net.cn

[S58] C++：命名空间
来源：http://iq.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://jf.chemitech.net.cn

[S59] C++：静态断言
来源：http://fx.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cl.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://wy.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ex.9csxet.cn

================================================================================
来源：http://mn.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kl.wgjwhj.cn

================================================================================
来源：http://tl.521024.cn

[T01] Kotlin：Hello World
来源：http://sy.jctech888.com.cn

println("Hello")
来源：http://rw.panjiajie.cn

[T02] Kotlin：变量
来源：http://qe.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ei.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://gn.wgjwhj.cn

"值: $b"
来源：http://nf.shxzukj.cn

[T04] Kotlin：空安全
来源：http://cg.9csxet.cn

val n: String? = null;  n?.length
来源：http://zd.newstarts.cn


<!-- 参考信息 -->