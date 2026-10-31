代发 wailian999

readonly PI=3.14
来源：http://fd.jianghongdianzi.cn

[R04] 位置参数
来源：http://jk.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ga.huixiangedu.cn

[R05] 参数默认值
来源：http://qk.shxzskj.cn

name="${1:-default}"
来源：http://ol.newstarts.cn

[R06] 判断命令是否存在
来源：http://kg.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jj.huanxung.cn

[R07] if 判断文件
来源：http://ym.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oe.yuntaijiaju.cn

[R08] 数值比较
来源：http://cq.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jo.muxihuayi.cn

[R09] 字符串比较
来源：http://ze.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bu.yuntaijiaju.cn

[R10] 正则匹配
来源：http://la.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dm.bjjhwx.cn

[R11] case 多分支
来源：http://em.haigaiapp.cn

case "$1" in
来源：http://cv.lnxyls.cn

start) echo "启动" ;;
来源：http://ed.szsharing.cn

stop)  echo "停止" ;;
来源：http://yz.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://sz.521024.cn

esac
来源：http://va.huixiangedu.cn

[R12] for 遍历文件
来源：http://zo.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://uo.lnxyls.cn

[R13] for 计数循环
来源：http://xo.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://ex.haigaiapp.cn

[R14] C 风格 for
来源：http://sk.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lh.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://pl.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vz.newstarts.cn

[R16] until 等待条件
来源：http://ve.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tu.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://yw.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kh.huixinmuqiang.cn

[R18] 遍历数组
来源：http://ec.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uy.nszjky.cn

[R19] 数组长度
来源：http://xm.szxytkj.cn

echo "${#arr[@]}"
来源：http://av.hnjuh.cn

[R20] 关联数组（字典）
来源：http://uy.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mk.newstarts.cn

[R21] 字符串长度
来源：http://gx.bookmarksfly.cn

echo "${#s}"
来源：http://lw.shxzukj.cn

[R22] 截取子串
来源：http://qu.gzmigu.cn

echo "${s:0:5}"
来源：http://fs.huixiangedu.cn

[R23] 字符串替换
来源：http://uc.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hd.newstarts.cn

[R24] 大小写转换
来源：http://rx.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ss.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://gv.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ln.nszjky.cn

[R26] 命令替换
来源：http://zv.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://ee.jctech888.com.cn

[R27] 算术展开
来源：http://vx.nicolike.cn

echo $((1 + 2 * 3))
来源：http://nb.muxihuayi.cn

[R28] 浮点运算
来源：http://dr.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://dr.haigaiapp.cn

[R29] 定义函数
来源：http://tw.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hi.lnxyls.cn

[R30] 函数返回状态码
来源：http://gq.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://ww.shtwfgs.cn

[R31] 局部变量
来源：http://wm.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://fq.wgjwhj.cn

[R32] 参数个数校验
来源：http://cr.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ms.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://pt.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ht.bookmarksfly.cn

[R34] 退出时清理
来源：http://qa.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hb.gzmigu.cn

[R35] 后台执行并等待
来源：http://hr.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://aa.nicolike.cn

[R36] 并发执行多个任务
来源：http://uf.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nd.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://iz.huixinmuqiang.cn

files=$(ls -1)
来源：http://gv.huixinmuqiang.cn

[R38] 管道串联
来源：http://ge.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://zq.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://cg.jctech888.com.cn

cmd > out.log 2>&1
来源：http://fw.newstarts.cn

[R40] 追加写日志
来源：http://wg.jianghongdianzi.cn

echo "log" >> out.log
来源：http://eq.bookmarksfly.cn

[R41] 丢弃输出
来源：http://ti.hahajie.cn

cmd >/dev/null 2>&1
来源：http://gq.wgjwhj.cn

[R42] 输入重定向
来源：http://zv.chemitech.net.cn

wc -l < a.txt
来源：http://xa.nicolike.cn

[R43] 按名字查找文件
来源：http://qq.colortex.cn

find . -name "*.log" -type f
来源：http://fq.shxzskj.cn

[R44] 按修改时间查找
来源：http://af.shxzukj.cn

find . -mtime -7 -type f
来源：http://oj.nszjky.cn

[R45] 批量删除
来源：http://vc.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://ze.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://jw.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ja.jctech888.com.cn

[R47] sed 单行替换
来源：http://vz.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ed.shxzskj.cn

[R48] awk 取指定列
来源：http://xn.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://lo.szsharing.cn

[R49] awk 带条件
来源：http://zc.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ka.szxytkj.cn

[R50] awk 求和
来源：http://cw.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kq.jctech888.com.cn

[R51] 排序去重取前几
来源：http://wx.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dt.szxytkj.cn

[R52] 统计行数
来源：http://zv.gzmigu.cn

wc -l a.txt
来源：http://kz.colortex.cn

[R53] 查看文件头与实时尾
来源：http://zo.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bs.huanxung.cn

[R54] 比较两个文件
来源：http://ic.yuntaijiaju.cn

diff a.txt b.txt
来源：http://na.asd995.cn

[R55] 压缩与解压
来源：http://ju.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mx.9csxet.cn

[R56] 远程拷贝
来源：http://km.521024.cn

scp file user@host:/path/
来源：http://cp.nicolike.cn

[R57] 远程执行命令
来源：http://ys.panjiajie.cn

ssh user@host 'uptime'
来源：http://hr.bjjhwx.cn

[R58] 下载文件
来源：http://gq.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cb.nszjky.cn

[R59] 发 POST JSON
来源：http://rw.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ol.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://ux.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nq.szsharing.cn

[R61] 磁盘占用
来源：http://kg.jctech888.com.cn

df -h;  du -sh *
来源：http://sx.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://vw.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://go.wgjwhj.cn

[R63] 内存与进程
来源：http://go.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://dd.yuntaijiaju.cn

[R64] 结束进程
来源：http://ac.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://xf.shtwfgs.cn

[R65] 查看端口占用
来源：http://mn.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xj.szsharing.cn

[R66] 定时任务
来源：http://gu.hnjuh.cn

crontab -e;  crontab -l
来源：http://yn.newstarts.cn

[R67] 生成随机十六进制串
来源：http://tg.huixiangedu.cn

openssl rand -hex 16
来源：http://zb.colortex.cn

[R68] 计算文件校验值
来源：http://dv.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ga.9csxet.cn

[R69] 生成随机密码
来源：http://th.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://zg.nicolike.cn

[R70] 时间戳与互转
来源：http://hl.colortex.cn

date +%s;  date -d @1700000000
来源：http://sf.shtwfgs.cn

[R71] 日期格式化
来源：http://vb.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wl.nicolike.cn

[R72] 等待端口就绪
来源：http://qr.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ik.chemitech.net.cn

[R73] 分割大日志
来源：http://gb.bjjhwx.cn

split -l 1000 big.log part_
来源：http://zc.lnxyls.cn

[R74] 批量重命名
来源：http://jc.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rs.huanxung.cn

[R75] 导出环境变量
来源：http://vh.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://jw.521024.cn

[R76] 使用临时文件
来源：http://pn.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xo.szsharing.cn

[R77] 读取用户输入
来源：http://ow.gzmigu.cn

read -rp "请输入: " ans
来源：http://el.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://ux.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qb.hahajie.cn

[R79] 解析命令行选项
来源：http://zp.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uz.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://ap.521024.cn

time ./run.sh
来源：http://ey.jctech888.com.cn

================================================================================
来源：http://tl.gzmigu.cn

S. C / C++ 专题
来源：http://kk.newstarts.cn

================================================================================
来源：http://dk.chemitech.net.cn

[S01] C：Hello World
来源：http://ns.9csxet.cn

#include <stdio.h>
来源：http://wg.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mt.newstarts.cn

[S02] C：变量与格式化输出
来源：http://nh.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://ug.shtwfgs.cn

[S03] C：读入整数
来源：http://pn.nszjky.cn

int x; scanf("%d", &x);
来源：http://ac.nicolike.cn

[S04] C：字符串复制
来源：http://tq.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vh.nszjky.cn

[S05] C：字符串长度
来源：http://yr.newstarts.cn

strlen(s)
来源：http://ui.szsharing.cn

[S06] C：字符串比较
来源：http://vv.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://ir.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://zu.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://id.colortex.cn

[S08] C：动态内存分配与释放
来源：http://fy.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lb.colortex.cn

[S09] C：结构体定义与初始化
来源：http://vj.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://il.9csxet.cn

[S10] C：指针与解引用
来源：http://ng.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://di.hnjuh.cn

[S11] C：逐行读文件
来源：http://am.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://ci.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nu.huanxung.cn

fclose(f);
来源：http://oh.asd995.cn

[S12] C：写文件
来源：http://ih.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gr.bookmarksfly.cn

[S13] C：宏定义
来源：http://ad.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xs.hnjuh.cn

[S14] C：枚举
来源：http://dp.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://yl.shxzskj.cn

[S15] C：类型转换
来源：http://vq.yuexingan06.cn

(double) a / b
来源：http://iq.yuexingan06.cn

[S16] C：位操作置位
来源：http://bq.szxytkj.cn

x |= (1 << 3);
来源：http://xx.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://yz.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dd.521024.cn

[S18] C：命令行参数
来源：http://hd.521024.cn

int main(int argc, char **argv)
来源：http://tx.szsharing.cn

[S19] C：快速排序
来源：http://rx.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ef.bookmarksfly.cn

[S20] C：二分查找
来源：http://rx.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://os.bjjhwx.cn

[S21] C：字符类别判断
来源：http://zk.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bb.newstarts.cn

[S22] C：字符串转数字
来源：http://tu.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://on.panjiajie.cn

[S23] C：随机数
来源：http://dz.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xj.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://oy.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ta.newstarts.cn

[S25] C：内存拷贝
来源：http://ym.huanxung.cn

memcpy(dst, src, n);
来源：http://oy.9csxet.cn

[S26] C：内存清零
来源：http://fr.nszjky.cn

memset(a, 0, sizeof a);
来源：http://ax.huanxung.cn

[S27] C：定义常量
来源：http://yb.yuexingan06.cn

const double PI = 3.14159;
来源：http://bw.gzmigu.cn

[S28] C：静态变量
来源：http://rw.wgjwhj.cn

static int counter = 0;
来源：http://td.yuntaijiaju.cn

[S29] C：变参函数
来源：http://mn.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ra.nicolike.cn

[S30] C：头文件保护
来源：http://td.yuntaijiaju.cn

#ifndef X_H
来源：http://cf.bookmarksfly.cn

#define X_H
来源：http://fa.bookmarksfly.cn

#endif
来源：http://qb.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://xv.shxzukj.cn

#include <iostream>
来源：http://gt.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://uf.panjiajie.cn

[S32] C++：字符串
来源：http://rp.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://dw.shxzukj.cn

[S33] C++：vector 增删
来源：http://cf.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iu.9csxet.cn

[S34] C++：遍历 vector
来源：http://hk.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://ie.newstarts.cn

[S35] C++：map
来源：http://cc.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tw.521024.cn

[S36] C++：unordered_map
来源：http://od.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ol.nszjky.cn

[S37] C++：set
来源：http://bi.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yp.jctech888.com.cn

[S38] C++：排序
来源：http://oj.colortex.cn

std::sort(v.begin(), v.end());
来源：http://bp.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://md.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ye.bookmarksfly.cn

[S40] C++：查找元素
来源：http://dl.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lc.nicolike.cn

[S41] C++：类与构造函数
来源：http://jo.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://of.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://hp.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://no.huanxung.cn

[S43] C++：智能指针
来源：http://zm.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://oi.jctech888.com.cn

[S44] C++：引用传参
来源：http://sj.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ad.lnxyls.cn

[S45] C++：lambda
来源：http://jd.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ro.shxzskj.cn

[S46] C++：函数模板
来源：http://uz.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zj.521024.cn

[S47] C++：结构化绑定遍历
来源：http://ii.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://on.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://rx.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ub.colortex.cn

while (std::getline(in, line)) { }
来源：http://wn.bjjhwx.cn

[S49] C++：写文件
来源：http://eh.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://is.gzmigu.cn

[S50] C++：格式化数字
来源：http://sb.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wy.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://hx.wgjwhj.cn

static_cast<double>(a) / b
来源：http://hw.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://sy.nicolike.cn

int size() const noexcept { return n_; }
来源：http://nv.jctech888.com.cn

[S53] C++：移动语义
来源：http://dz.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://no.szsharing.cn

[S54] C++：异常处理
来源：http://ff.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jd.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://au.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ui.shtwfgs.cn

[S56] C++：optional
来源：http://ch.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nv.szxytkj.cn

[S57] C++：编译期常量
来源：http://pr.521024.cn

constexpr int N = 10;
来源：http://dp.wgjwhj.cn

[S58] C++：命名空间
来源：http://xr.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://vd.shxzskj.cn

[S59] C++：静态断言
来源：http://ts.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://id.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://ny.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mp.9csxet.cn

================================================================================
来源：http://rm.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hn.chemitech.net.cn

================================================================================
来源：http://bf.hahajie.cn

[T01] Kotlin：Hello World
来源：http://lb.huixiangedu.cn

println("Hello")
来源：http://tg.jctech888.com.cn

[T02] Kotlin：变量
来源：http://nz.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wj.521024.cn

[T03] Kotlin：字符串模板
来源：http://bx.jctech888.com.cn

"值: $b"
来源：http://th.521024.cn

[T04] Kotlin：空安全
来源：http://qw.nicolike.cn

val n: String? = null;  n?.length
来源：http://pr.bookmarksfly.cn


<!-- 参考信息 -->