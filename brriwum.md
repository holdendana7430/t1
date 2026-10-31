代发 wailian999

readonly PI=3.14
来源：http://mx.521024.cn

[R04] 位置参数
来源：http://wf.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ga.muxihuayi.cn

[R05] 参数默认值
来源：http://bj.huixiangedu.cn

name="${1:-default}"
来源：http://ln.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://da.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rk.asd995.cn

[R07] if 判断文件
来源：http://aa.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eb.hnjuh.cn

[R08] 数值比较
来源：http://hh.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jb.panjiajie.cn

[R09] 字符串比较
来源：http://mi.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cz.muxihuayi.cn

[R10] 正则匹配
来源：http://cy.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kg.jctech888.com.cn

[R11] case 多分支
来源：http://ri.haigaiapp.cn

case "$1" in
来源：http://ll.huixiangedu.cn

start) echo "启动" ;;
来源：http://ui.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://ih.asd995.cn

*)     echo "未知命令" ;;
来源：http://qh.9csxet.cn

esac
来源：http://pv.jctech888.com.cn

[R12] for 遍历文件
来源：http://ih.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://wv.wgjwhj.cn

[R13] for 计数循环
来源：http://ob.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://mg.newstarts.cn

[R14] C 风格 for
来源：http://bf.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ea.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://em.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rr.lnxyls.cn

[R16] until 等待条件
来源：http://ry.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wa.chemitech.net.cn

[R17] 数组定义与取值
来源：http://ba.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sz.shxzskj.cn

[R18] 遍历数组
来源：http://uo.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zw.521024.cn

[R19] 数组长度
来源：http://do.shtwfgs.cn

echo "${#arr[@]}"
来源：http://ux.nicolike.cn

[R20] 关联数组（字典）
来源：http://xa.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://on.panjiajie.cn

[R21] 字符串长度
来源：http://uq.asd995.cn

echo "${#s}"
来源：http://tr.hahajie.cn

[R22] 截取子串
来源：http://os.chemitech.net.cn

echo "${s:0:5}"
来源：http://ez.lnxyls.cn

[R23] 字符串替换
来源：http://ta.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tf.haigaiapp.cn

[R24] 大小写转换
来源：http://um.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zl.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://wf.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bd.nszjky.cn

[R26] 命令替换
来源：http://fw.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://jr.521024.cn

[R27] 算术展开
来源：http://yd.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ei.jianghongdianzi.cn

[R28] 浮点运算
来源：http://vp.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://iv.chemitech.net.cn

[R29] 定义函数
来源：http://sf.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ck.shxzukj.cn

[R30] 函数返回状态码
来源：http://ck.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://lu.huixinmuqiang.cn

[R31] 局部变量
来源：http://ah.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://gb.nszjky.cn

[R32] 参数个数校验
来源：http://qr.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gn.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://je.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fd.szxytkj.cn

[R34] 退出时清理
来源：http://lb.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://td.shtwfgs.cn

[R35] 后台执行并等待
来源：http://wy.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lm.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://bb.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ez.hnjuh.cn

[R37] 把输出赋给变量
来源：http://bu.shxzukj.cn

files=$(ls -1)
来源：http://ht.gzmigu.cn

[R38] 管道串联
来源：http://ux.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://ir.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://uu.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://fq.huixiangedu.cn

[R40] 追加写日志
来源：http://nj.jctech888.com.cn

echo "log" >> out.log
来源：http://uw.colortex.cn

[R41] 丢弃输出
来源：http://zo.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://ju.szxytkj.cn

[R42] 输入重定向
来源：http://hl.shtwfgs.cn

wc -l < a.txt
来源：http://al.shxzskj.cn

[R43] 按名字查找文件
来源：http://ca.gzmigu.cn

find . -name "*.log" -type f
来源：http://ad.colortex.cn

[R44] 按修改时间查找
来源：http://ys.521024.cn

find . -mtime -7 -type f
来源：http://zd.colortex.cn

[R45] 批量删除
来源：http://mu.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://ar.gzmigu.cn

[R46] 递归替换文件内容
来源：http://gl.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cr.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://nm.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sn.hnjuh.cn

[R48] awk 取指定列
来源：http://bc.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://kj.jctech888.com.cn

[R49] awk 带条件
来源：http://fj.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ex.huixiangedu.cn

[R50] awk 求和
来源：http://fk.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://us.shtwfgs.cn

[R51] 排序去重取前几
来源：http://gd.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cg.muxihuayi.cn

[R52] 统计行数
来源：http://rt.panjiajie.cn

wc -l a.txt
来源：http://tm.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://oo.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gk.muxihuayi.cn

[R54] 比较两个文件
来源：http://dq.nicolike.cn

diff a.txt b.txt
来源：http://sp.panjiajie.cn

[R55] 压缩与解压
来源：http://mm.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mx.9csxet.cn

[R56] 远程拷贝
来源：http://bf.jctech888.com.cn

scp file user@host:/path/
来源：http://gq.nszjky.cn

[R57] 远程执行命令
来源：http://ye.lnxyls.cn

ssh user@host 'uptime'
来源：http://be.nszjky.cn

[R58] 下载文件
来源：http://dg.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ek.nicolike.cn

[R59] 发 POST JSON
来源：http://tc.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tt.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://bj.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ca.nszjky.cn

[R61] 磁盘占用
来源：http://al.jctech888.com.cn

df -h;  du -sh *
来源：http://ra.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://cp.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://sf.szsharing.cn

[R63] 内存与进程
来源：http://jw.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://rb.jctech888.com.cn

[R64] 结束进程
来源：http://oi.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://po.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://aj.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://js.huixiangedu.cn

[R66] 定时任务
来源：http://ea.panjiajie.cn

crontab -e;  crontab -l
来源：http://pv.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://ct.wgjwhj.cn

openssl rand -hex 16
来源：http://dm.nicolike.cn

[R68] 计算文件校验值
来源：http://wy.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cg.szxytkj.cn

[R69] 生成随机密码
来源：http://fm.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://nw.jctech888.com.cn

[R70] 时间戳与互转
来源：http://ae.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://ba.yuexingan06.cn

[R71] 日期格式化
来源：http://dv.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wi.hnjuh.cn

[R72] 等待端口就绪
来源：http://oo.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bl.bjjhwx.cn

[R73] 分割大日志
来源：http://uz.panjiajie.cn

split -l 1000 big.log part_
来源：http://qs.hahajie.cn

[R74] 批量重命名
来源：http://vb.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ov.panjiajie.cn

[R75] 导出环境变量
来源：http://yi.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ph.yuexingan06.cn

[R76] 使用临时文件
来源：http://iz.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fw.szxytkj.cn

[R77] 读取用户输入
来源：http://ui.chemitech.net.cn

read -rp "请输入: " ans
来源：http://po.bookmarksfly.cn

[R78] 交互式菜单
来源：http://ga.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wl.muxihuayi.cn

[R79] 解析命令行选项
来源：http://fb.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gl.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://zu.jctech888.com.cn

time ./run.sh
来源：http://ji.jctech888.com.cn

================================================================================
来源：http://xp.jianghongdianzi.cn

S. C / C++ 专题
来源：http://si.huixiangedu.cn

================================================================================
来源：http://li.bookmarksfly.cn

[S01] C：Hello World
来源：http://vh.shxzskj.cn

#include <stdio.h>
来源：http://ey.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jn.szsharing.cn

[S02] C：变量与格式化输出
来源：http://hc.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://vj.jctech888.com.cn

[S03] C：读入整数
来源：http://vt.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://dn.newstarts.cn

[S04] C：字符串复制
来源：http://ug.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yi.wgjwhj.cn

[S05] C：字符串长度
来源：http://xf.shxzukj.cn

strlen(s)
来源：http://ne.haigaiapp.cn

[S06] C：字符串比较
来源：http://jn.colortex.cn

strcmp(a, b) == 0
来源：http://ze.521024.cn

[S07] C：数组遍历求和
来源：http://fy.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lf.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://zj.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ix.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://gq.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pk.muxihuayi.cn

[S10] C：指针与解引用
来源：http://bv.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://bo.shxzskj.cn

[S11] C：逐行读文件
来源：http://pm.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://vu.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kf.shxzukj.cn

fclose(f);
来源：http://vg.bookmarksfly.cn

[S12] C：写文件
来源：http://bq.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lr.lnxyls.cn

[S13] C：宏定义
来源：http://vl.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uv.lnxyls.cn

[S14] C：枚举
来源：http://lm.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://zz.jctech888.com.cn

[S15] C：类型转换
来源：http://uh.bjjhwx.cn

(double) a / b
来源：http://uy.hnjuh.cn

[S16] C：位操作置位
来源：http://ih.szxytkj.cn

x |= (1 << 3);
来源：http://qk.nszjky.cn

[S17] C：安全拼接字符串
来源：http://lk.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xp.hnjuh.cn

[S18] C：命令行参数
来源：http://wl.9csxet.cn

int main(int argc, char **argv)
来源：http://oj.9csxet.cn

[S19] C：快速排序
来源：http://nc.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://un.nicolike.cn

[S20] C：二分查找
来源：http://gs.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mz.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://zd.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kk.hnjuh.cn

[S22] C：字符串转数字
来源：http://wb.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zm.hahajie.cn

[S23] C：随机数
来源：http://fo.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gg.shxzskj.cn

[S24] C：获取本地时间
来源：http://dr.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nf.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://id.panjiajie.cn

memcpy(dst, src, n);
来源：http://ud.szxytkj.cn

[S26] C：内存清零
来源：http://ul.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://yq.hahajie.cn

[S27] C：定义常量
来源：http://hm.yuexingan06.cn

const double PI = 3.14159;
来源：http://vl.muxihuayi.cn

[S28] C：静态变量
来源：http://gp.shtwfgs.cn

static int counter = 0;
来源：http://kg.chemitech.net.cn

[S29] C：变参函数
来源：http://cr.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zh.muxihuayi.cn

[S30] C：头文件保护
来源：http://qx.panjiajie.cn

#ifndef X_H
来源：http://nt.chemitech.net.cn

#define X_H
来源：http://jy.521024.cn

#endif
来源：http://dq.jctech888.com.cn

[S31] C++：Hello World
来源：http://ni.panjiajie.cn

#include <iostream>
来源：http://kk.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://kn.yuntaijiaju.cn

[S32] C++：字符串
来源：http://di.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://dr.szxytkj.cn

[S33] C++：vector 增删
来源：http://cx.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cw.newstarts.cn

[S34] C++：遍历 vector
来源：http://xh.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://nm.bjjhwx.cn

[S35] C++：map
来源：http://bl.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qg.9csxet.cn

[S36] C++：unordered_map
来源：http://sj.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pf.szxytkj.cn

[S37] C++：set
来源：http://oz.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fh.nszjky.cn

[S38] C++：排序
来源：http://zh.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://ov.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://xk.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jn.haigaiapp.cn

[S40] C++：查找元素
来源：http://dk.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ka.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://rt.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ig.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://va.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://hg.shxzskj.cn

[S43] C++：智能指针
来源：http://fs.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://cd.newstarts.cn

[S44] C++：引用传参
来源：http://jz.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://ou.bjjhwx.cn

[S45] C++：lambda
来源：http://jc.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nq.shtwfgs.cn

[S46] C++：函数模板
来源：http://ia.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ux.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://ap.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xn.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://bx.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rt.9csxet.cn

while (std::getline(in, line)) { }
来源：http://zm.bjjhwx.cn

[S49] C++：写文件
来源：http://pt.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mc.colortex.cn

[S50] C++：格式化数字
来源：http://lf.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zx.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://pg.newstarts.cn

static_cast<double>(a) / b
来源：http://ai.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://hf.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://fq.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://gh.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://gx.lnxyls.cn

[S54] C++：异常处理
来源：http://rh.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fb.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://ze.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://th.bookmarksfly.cn

[S56] C++：optional
来源：http://bj.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mj.wgjwhj.cn

[S57] C++：编译期常量
来源：http://zn.shxzskj.cn

constexpr int N = 10;
来源：http://kl.bjjhwx.cn

[S58] C++：命名空间
来源：http://re.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://ah.bjjhwx.cn

[S59] C++：静态断言
来源：http://qq.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rf.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://vg.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uu.hahajie.cn

================================================================================
来源：http://of.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wy.shxzskj.cn

================================================================================
来源：http://iy.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://in.hnjuh.cn

println("Hello")
来源：http://hn.521024.cn

[T02] Kotlin：变量
来源：http://du.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://om.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://sb.newstarts.cn

"值: $b"
来源：http://ko.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://cj.hnjuh.cn

val n: String? = null;  n?.length
来源：http://fx.szxytkj.cn


<!-- 参考信息 -->