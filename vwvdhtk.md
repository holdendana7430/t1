代发 wailian999

name="${1:-default}"
来源：http://ye.nszjky.cn

[R06] 判断命令是否存在
来源：http://fc.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yb.huixinmuqiang.cn

[R07] if 判断文件
来源：http://ro.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tg.gzmigu.cn

[R08] 数值比较
来源：http://lj.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yz.szxytkj.cn

[R09] 字符串比较
来源：http://sk.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://km.bjjhwx.cn

[R10] 正则匹配
来源：http://qq.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ik.shtwfgs.cn

[R11] case 多分支
来源：http://fh.9csxet.cn

case "$1" in
来源：http://sm.jctech888.com.cn

start) echo "启动" ;;
来源：http://cg.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://ik.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://ju.wgjwhj.cn

esac
来源：http://iv.muxihuayi.cn

[R12] for 遍历文件
来源：http://ad.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://jx.yuexingan06.cn

[R13] for 计数循环
来源：http://nf.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://ai.gzmigu.cn

[R14] C 风格 for
来源：http://zz.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qq.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://yf.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xx.szxytkj.cn

[R16] until 等待条件
来源：http://kg.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ic.gzmigu.cn

[R17] 数组定义与取值
来源：http://es.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gl.jianghongdianzi.cn

[R18] 遍历数组
来源：http://uw.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://au.huixinmuqiang.cn

[R19] 数组长度
来源：http://qy.9csxet.cn

echo "${#arr[@]}"
来源：http://vf.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://of.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jc.colortex.cn

[R21] 字符串长度
来源：http://oi.gzmigu.cn

echo "${#s}"
来源：http://cx.chemitech.net.cn

[R22] 截取子串
来源：http://pt.bookmarksfly.cn

echo "${s:0:5}"
来源：http://na.yuexingan06.cn

[R23] 字符串替换
来源：http://du.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fi.huixiangedu.cn

[R24] 大小写转换
来源：http://da.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rv.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://vj.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rc.jctech888.com.cn

[R26] 命令替换
来源：http://fd.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://yd.bjjhwx.cn

[R27] 算术展开
来源：http://yj.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://ax.shtwfgs.cn

[R28] 浮点运算
来源：http://sy.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://zr.nicolike.cn

[R29] 定义函数
来源：http://jm.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mk.521024.cn

[R30] 函数返回状态码
来源：http://wr.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://vh.hahajie.cn

[R31] 局部变量
来源：http://fs.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://jl.gzmigu.cn

[R32] 参数个数校验
来源：http://xc.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xt.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://cm.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rb.colortex.cn

[R34] 退出时清理
来源：http://vd.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lx.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://jn.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gm.hahajie.cn

[R36] 并发执行多个任务
来源：http://ft.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yu.shxzskj.cn

[R37] 把输出赋给变量
来源：http://da.panjiajie.cn

files=$(ls -1)
来源：http://wh.yuntaijiaju.cn

[R38] 管道串联
来源：http://gg.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://cs.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://vz.9csxet.cn

cmd > out.log 2>&1
来源：http://gl.panjiajie.cn

[R40] 追加写日志
来源：http://qm.bookmarksfly.cn

echo "log" >> out.log
来源：http://jv.shxzskj.cn

[R41] 丢弃输出
来源：http://cl.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://oz.lnxyls.cn

[R42] 输入重定向
来源：http://yo.9csxet.cn

wc -l < a.txt
来源：http://om.huanxung.cn

[R43] 按名字查找文件
来源：http://cf.huixiangedu.cn

find . -name "*.log" -type f
来源：http://gg.yuexingan06.cn

[R44] 按修改时间查找
来源：http://kk.newstarts.cn

find . -mtime -7 -type f
来源：http://qg.hnjuh.cn

[R45] 批量删除
来源：http://oq.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://hj.huanxung.cn

[R46] 递归替换文件内容
来源：http://ze.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wn.muxihuayi.cn

[R47] sed 单行替换
来源：http://tx.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ys.gzmigu.cn

[R48] awk 取指定列
来源：http://vf.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://zh.bjjhwx.cn

[R49] awk 带条件
来源：http://pb.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wv.chemitech.net.cn

[R50] awk 求和
来源：http://ll.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oq.shtwfgs.cn

[R51] 排序去重取前几
来源：http://ek.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nl.szsharing.cn

[R52] 统计行数
来源：http://mh.colortex.cn

wc -l a.txt
来源：http://js.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://cd.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oj.muxihuayi.cn

[R54] 比较两个文件
来源：http://bh.huanxung.cn

diff a.txt b.txt
来源：http://zy.wgjwhj.cn

[R55] 压缩与解压
来源：http://ut.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jh.shxzukj.cn

[R56] 远程拷贝
来源：http://zg.huixiangedu.cn

scp file user@host:/path/
来源：http://ka.jctech888.com.cn

[R57] 远程执行命令
来源：http://bj.panjiajie.cn

ssh user@host 'uptime'
来源：http://nz.panjiajie.cn

[R58] 下载文件
来源：http://hl.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aw.newstarts.cn

[R59] 发 POST JSON
来源：http://tq.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jy.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://tt.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mf.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://vm.newstarts.cn

df -h;  du -sh *
来源：http://on.lnxyls.cn

[R62] 找最占空间的文件
来源：http://al.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://fw.haigaiapp.cn

[R63] 内存与进程
来源：http://jk.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://lc.muxihuayi.cn

[R64] 结束进程
来源：http://oh.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://ep.lnxyls.cn

[R65] 查看端口占用
来源：http://ml.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oj.shxzukj.cn

[R66] 定时任务
来源：http://om.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://gu.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://ot.shtwfgs.cn

openssl rand -hex 16
来源：http://gi.shxzskj.cn

[R68] 计算文件校验值
来源：http://cc.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iu.lnxyls.cn

[R69] 生成随机密码
来源：http://ua.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://ns.521024.cn

[R70] 时间戳与互转
来源：http://nz.colortex.cn

date +%s;  date -d @1700000000
来源：http://uw.szxytkj.cn

[R71] 日期格式化
来源：http://he.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fu.hnjuh.cn

[R72] 等待端口就绪
来源：http://vv.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vi.shxzskj.cn

[R73] 分割大日志
来源：http://tf.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://dz.newstarts.cn

[R74] 批量重命名
来源：http://iz.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cs.colortex.cn

[R75] 导出环境变量
来源：http://cf.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://gu.shxzskj.cn

[R76] 使用临时文件
来源：http://si.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ox.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://jd.szsharing.cn

read -rp "请输入: " ans
来源：http://yo.9csxet.cn

[R78] 交互式菜单
来源：http://gg.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://et.hahajie.cn

[R79] 解析命令行选项
来源：http://fa.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lq.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://zt.nicolike.cn

time ./run.sh
来源：http://du.shxzskj.cn

================================================================================
来源：http://rv.hahajie.cn

S. C / C++ 专题
来源：http://pn.nszjky.cn

================================================================================
来源：http://zx.huixinmuqiang.cn

[S01] C：Hello World
来源：http://vh.bookmarksfly.cn

#include <stdio.h>
来源：http://mj.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nj.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://in.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://go.shtwfgs.cn

[S03] C：读入整数
来源：http://lh.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://mm.bookmarksfly.cn

[S04] C：字符串复制
来源：http://et.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rr.panjiajie.cn

[S05] C：字符串长度
来源：http://tv.bookmarksfly.cn

strlen(s)
来源：http://tl.nszjky.cn

[S06] C：字符串比较
来源：http://sv.wgjwhj.cn

strcmp(a, b) == 0
来源：http://bq.huanxung.cn

[S07] C：数组遍历求和
来源：http://am.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vd.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://ey.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ot.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://cy.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zl.nszjky.cn

[S10] C：指针与解引用
来源：http://fg.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://jy.9csxet.cn

[S11] C：逐行读文件
来源：http://vv.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://ph.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ks.9csxet.cn

fclose(f);
来源：http://gu.szsharing.cn

[S12] C：写文件
来源：http://vv.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yr.bookmarksfly.cn

[S13] C：宏定义
来源：http://ny.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hg.newstarts.cn

[S14] C：枚举
来源：http://qx.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ab.colortex.cn

[S15] C：类型转换
来源：http://bd.nicolike.cn

(double) a / b
来源：http://sr.asd995.cn

[S16] C：位操作置位
来源：http://ko.nszjky.cn

x |= (1 << 3);
来源：http://wa.colortex.cn

[S17] C：安全拼接字符串
来源：http://uf.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gg.shxzukj.cn

[S18] C：命令行参数
来源：http://md.hahajie.cn

int main(int argc, char **argv)
来源：http://zw.panjiajie.cn

[S19] C：快速排序
来源：http://rp.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mh.jctech888.com.cn

[S20] C：二分查找
来源：http://gy.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lc.9csxet.cn

[S21] C：字符类别判断
来源：http://qf.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fw.szsharing.cn

[S22] C：字符串转数字
来源：http://lt.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kp.panjiajie.cn

[S23] C：随机数
来源：http://kt.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tc.nicolike.cn

[S24] C：获取本地时间
来源：http://yy.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kt.szsharing.cn

[S25] C：内存拷贝
来源：http://bt.wgjwhj.cn

memcpy(dst, src, n);
来源：http://rb.shxzukj.cn

[S26] C：内存清零
来源：http://bk.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://bm.bjjhwx.cn

[S27] C：定义常量
来源：http://ii.nicolike.cn

const double PI = 3.14159;
来源：http://fj.nszjky.cn

[S28] C：静态变量
来源：http://zj.haigaiapp.cn

static int counter = 0;
来源：http://vd.lnxyls.cn

[S29] C：变参函数
来源：http://on.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sl.hahajie.cn

[S30] C：头文件保护
来源：http://jm.haigaiapp.cn

#ifndef X_H
来源：http://jg.nszjky.cn

#define X_H
来源：http://sa.chemitech.net.cn

#endif
来源：http://ag.shtwfgs.cn

[S31] C++：Hello World
来源：http://ax.huanxung.cn

#include <iostream>
来源：http://ji.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://bz.asd995.cn

[S32] C++：字符串
来源：http://qi.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://am.521024.cn

[S33] C++：vector 增删
来源：http://mx.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vu.huanxung.cn

[S34] C++：遍历 vector
来源：http://th.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://oe.wgjwhj.cn

[S35] C++：map
来源：http://mb.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uy.szsharing.cn

[S36] C++：unordered_map
来源：http://qv.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://su.bookmarksfly.cn

[S37] C++：set
来源：http://qc.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://od.hnjuh.cn

[S38] C++：排序
来源：http://qg.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://my.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://fq.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ns.muxihuayi.cn

[S40] C++：查找元素
来源：http://bm.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jc.colortex.cn

[S41] C++：类与构造函数
来源：http://eh.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jf.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://vr.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://se.asd995.cn

[S43] C++：智能指针
来源：http://hh.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://qp.yuexingan06.cn

[S44] C++：引用传参
来源：http://db.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://ma.shxzskj.cn

[S45] C++：lambda
来源：http://or.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nr.nicolike.cn

[S46] C++：函数模板
来源：http://ao.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zh.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://ue.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nq.hnjuh.cn

[S48] C++：逐行读文件
来源：http://dy.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uz.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://cl.nicolike.cn

[S49] C++：写文件
来源：http://ps.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sh.colortex.cn

[S50] C++：格式化数字
来源：http://ty.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kf.panjiajie.cn

[S51] C++：显式类型转换
来源：http://ye.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://nc.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://is.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://ii.hahajie.cn

[S53] C++：移动语义
来源：http://lz.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://nb.nszjky.cn

[S54] C++：异常处理
来源：http://ar.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tg.newstarts.cn

[S55] C++：结构化绑定
来源：http://mh.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ok.huixinmuqiang.cn

[S56] C++：optional
来源：http://vs.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ej.szsharing.cn

[S57] C++：编译期常量
来源：http://bd.gzmigu.cn

constexpr int N = 10;
来源：http://zf.shxzskj.cn

[S58] C++：命名空间
来源：http://au.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://yr.szsharing.cn

[S59] C++：静态断言
来源：http://ty.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eh.asd995.cn

[S60] C++：遍历并删除元素
来源：http://it.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gc.shtwfgs.cn

================================================================================
来源：http://ps.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bs.gzmigu.cn

================================================================================
来源：http://xc.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://sz.shxzskj.cn

println("Hello")
来源：http://da.lnxyls.cn

[T02] Kotlin：变量
来源：http://ej.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lz.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://le.gzmigu.cn

"值: $b"
来源：http://kz.huanxung.cn

[T04] Kotlin：空安全
来源：http://cm.521024.cn

val n: String? = null;  n?.length
来源：http://eo.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://ni.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://be.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://oa.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://to.chemitech.net.cn


<!-- 参考信息 -->