代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sr.hnjuh.cn

[R10] 正则匹配
来源：http://di.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lh.jianghongdianzi.cn

[R11] case 多分支
来源：http://vz.hnjuh.cn

case "$1" in
来源：http://hz.lnxyls.cn

start) echo "启动" ;;
来源：http://xq.9csxet.cn

stop)  echo "停止" ;;
来源：http://ci.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://zc.szxytkj.cn

esac
来源：http://uq.shtwfgs.cn

[R12] for 遍历文件
来源：http://mg.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://bl.521024.cn

[R13] for 计数循环
来源：http://lg.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://tt.yuntaijiaju.cn

[R14] C 风格 for
来源：http://ra.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aq.shxzukj.cn

[R15] while 逐行读文件
来源：http://xg.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tn.521024.cn

[R16] until 等待条件
来源：http://lx.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ox.lnxyls.cn

[R17] 数组定义与取值
来源：http://qu.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zr.huanxung.cn

[R18] 遍历数组
来源：http://vo.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bd.jctech888.com.cn

[R19] 数组长度
来源：http://so.9csxet.cn

echo "${#arr[@]}"
来源：http://gi.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://za.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sj.nszjky.cn

[R21] 字符串长度
来源：http://ev.lnxyls.cn

echo "${#s}"
来源：http://ii.chemitech.net.cn

[R22] 截取子串
来源：http://fc.szxytkj.cn

echo "${s:0:5}"
来源：http://oi.shxzskj.cn

[R23] 字符串替换
来源：http://mo.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dq.huixinmuqiang.cn

[R24] 大小写转换
来源：http://cw.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dn.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://eo.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gs.szxytkj.cn

[R26] 命令替换
来源：http://dd.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://fq.asd995.cn

[R27] 算术展开
来源：http://kx.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://iz.hnjuh.cn

[R28] 浮点运算
来源：http://ic.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://gg.huixinmuqiang.cn

[R29] 定义函数
来源：http://lk.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lr.asd995.cn

[R30] 函数返回状态码
来源：http://ik.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://re.jctech888.com.cn

[R31] 局部变量
来源：http://xm.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://nx.nszjky.cn

[R32] 参数个数校验
来源：http://mh.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://se.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://kw.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ej.bookmarksfly.cn

[R34] 退出时清理
来源：http://er.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://on.lnxyls.cn

[R35] 后台执行并等待
来源：http://zm.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xt.hahajie.cn

[R36] 并发执行多个任务
来源：http://wq.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qf.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://tf.bjjhwx.cn

files=$(ls -1)
来源：http://lc.9csxet.cn

[R38] 管道串联
来源：http://ur.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://xp.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://cx.shtwfgs.cn

cmd > out.log 2>&1
来源：http://qp.jianghongdianzi.cn

[R40] 追加写日志
来源：http://zx.wgjwhj.cn

echo "log" >> out.log
来源：http://dh.muxihuayi.cn

[R41] 丢弃输出
来源：http://ce.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://on.hahajie.cn

[R42] 输入重定向
来源：http://vk.bjjhwx.cn

wc -l < a.txt
来源：http://bn.hahajie.cn

[R43] 按名字查找文件
来源：http://ky.shxzskj.cn

find . -name "*.log" -type f
来源：http://hr.szsharing.cn

[R44] 按修改时间查找
来源：http://ty.panjiajie.cn

find . -mtime -7 -type f
来源：http://yq.bjjhwx.cn

[R45] 批量删除
来源：http://fe.nszjky.cn

find . -name "*.tmp" -delete
来源：http://mv.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://kq.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vd.gzmigu.cn

[R47] sed 单行替换
来源：http://rh.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ue.hahajie.cn

[R48] awk 取指定列
来源：http://rm.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://aa.chemitech.net.cn

[R49] awk 带条件
来源：http://st.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zr.hnjuh.cn

[R50] awk 求和
来源：http://mb.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rm.nicolike.cn

[R51] 排序去重取前几
来源：http://bb.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cy.shxzukj.cn

[R52] 统计行数
来源：http://ej.muxihuayi.cn

wc -l a.txt
来源：http://gi.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://sn.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fe.asd995.cn

[R54] 比较两个文件
来源：http://em.szxytkj.cn

diff a.txt b.txt
来源：http://hr.jctech888.com.cn

[R55] 压缩与解压
来源：http://ke.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vq.szxytkj.cn

[R56] 远程拷贝
来源：http://vd.jianghongdianzi.cn

scp file user@host:/path/
来源：http://fj.wgjwhj.cn

[R57] 远程执行命令
来源：http://ep.huixiangedu.cn

ssh user@host 'uptime'
来源：http://gu.szsharing.cn

[R58] 下载文件
来源：http://kg.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gu.shxzukj.cn

[R59] 发 POST JSON
来源：http://oz.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vz.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://zg.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lj.huanxung.cn

[R61] 磁盘占用
来源：http://mi.muxihuayi.cn

df -h;  du -sh *
来源：http://us.shxzukj.cn

[R62] 找最占空间的文件
来源：http://bf.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://oy.jianghongdianzi.cn

[R63] 内存与进程
来源：http://ng.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://yq.jctech888.com.cn

[R64] 结束进程
来源：http://zi.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://oz.panjiajie.cn

[R65] 查看端口占用
来源：http://yr.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kt.521024.cn

[R66] 定时任务
来源：http://hr.colortex.cn

crontab -e;  crontab -l
来源：http://kc.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://mo.shxzukj.cn

openssl rand -hex 16
来源：http://go.muxihuayi.cn

[R68] 计算文件校验值
来源：http://kv.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zh.haigaiapp.cn

[R69] 生成随机密码
来源：http://qy.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://uy.huixiangedu.cn

[R70] 时间戳与互转
来源：http://uw.newstarts.cn

date +%s;  date -d @1700000000
来源：http://hc.yuexingan06.cn

[R71] 日期格式化
来源：http://iw.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jw.hahajie.cn

[R72] 等待端口就绪
来源：http://sp.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://om.szxytkj.cn

[R73] 分割大日志
来源：http://ga.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://ti.bookmarksfly.cn

[R74] 批量重命名
来源：http://wz.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vp.shxzskj.cn

[R75] 导出环境变量
来源：http://da.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://bp.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://ko.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ng.gzmigu.cn

[R77] 读取用户输入
来源：http://cg.huanxung.cn

read -rp "请输入: " ans
来源：http://ig.hnjuh.cn

[R78] 交互式菜单
来源：http://ly.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dq.shxzskj.cn

[R79] 解析命令行选项
来源：http://dw.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dt.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://qd.hnjuh.cn

time ./run.sh
来源：http://ap.9csxet.cn

================================================================================
来源：http://xy.szxytkj.cn

S. C / C++ 专题
来源：http://km.shxzukj.cn

================================================================================
来源：http://nq.muxihuayi.cn

[S01] C：Hello World
来源：http://hj.yuntaijiaju.cn

#include <stdio.h>
来源：http://oc.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fv.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://sc.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://mz.gzmigu.cn

[S03] C：读入整数
来源：http://yg.nicolike.cn

int x; scanf("%d", &x);
来源：http://yb.colortex.cn

[S04] C：字符串复制
来源：http://sw.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sc.nicolike.cn

[S05] C：字符串长度
来源：http://at.bookmarksfly.cn

strlen(s)
来源：http://ul.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://wo.521024.cn

strcmp(a, b) == 0
来源：http://iw.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://gd.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iq.521024.cn

[S08] C：动态内存分配与释放
来源：http://wm.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://md.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://es.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iz.szxytkj.cn

[S10] C：指针与解引用
来源：http://fn.nszjky.cn

int *p = &a;  *p = 5;
来源：http://hl.hahajie.cn

[S11] C：逐行读文件
来源：http://pg.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://of.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gg.huixiangedu.cn

fclose(f);
来源：http://uk.huixiangedu.cn

[S12] C：写文件
来源：http://jk.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fl.521024.cn

[S13] C：宏定义
来源：http://do.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uu.yuexingan06.cn

[S14] C：枚举
来源：http://sk.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://rr.nszjky.cn

[S15] C：类型转换
来源：http://qz.hahajie.cn

(double) a / b
来源：http://ux.panjiajie.cn

[S16] C：位操作置位
来源：http://et.panjiajie.cn

x |= (1 << 3);
来源：http://xh.9csxet.cn

[S17] C：安全拼接字符串
来源：http://fl.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uj.huixiangedu.cn

[S18] C：命令行参数
来源：http://mg.hnjuh.cn

int main(int argc, char **argv)
来源：http://ja.9csxet.cn

[S19] C：快速排序
来源：http://kb.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://by.haigaiapp.cn

[S20] C：二分查找
来源：http://ro.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xy.szxytkj.cn

[S21] C：字符类别判断
来源：http://pg.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://br.521024.cn

[S22] C：字符串转数字
来源：http://av.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ht.shtwfgs.cn

[S23] C：随机数
来源：http://ao.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hx.huanxung.cn

[S24] C：获取本地时间
来源：http://ia.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eg.nszjky.cn

[S25] C：内存拷贝
来源：http://ir.shxzskj.cn

memcpy(dst, src, n);
来源：http://mb.9csxet.cn

[S26] C：内存清零
来源：http://zf.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://zg.huanxung.cn

[S27] C：定义常量
来源：http://aq.huanxung.cn

const double PI = 3.14159;
来源：http://fz.newstarts.cn

[S28] C：静态变量
来源：http://vl.yuexingan06.cn

static int counter = 0;
来源：http://pj.bjjhwx.cn

[S29] C：变参函数
来源：http://vo.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ec.huanxung.cn

[S30] C：头文件保护
来源：http://fr.yuntaijiaju.cn

#ifndef X_H
来源：http://fu.newstarts.cn

#define X_H
来源：http://au.gzmigu.cn

#endif
来源：http://kt.huanxung.cn

[S31] C++：Hello World
来源：http://yl.hahajie.cn

#include <iostream>
来源：http://ih.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://sm.yuntaijiaju.cn

[S32] C++：字符串
来源：http://dx.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ib.chemitech.net.cn

[S33] C++：vector 增删
来源：http://hi.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sn.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://lc.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://sc.gzmigu.cn

[S35] C++：map
来源：http://ak.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uf.nszjky.cn

[S36] C++：unordered_map
来源：http://sb.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gz.bjjhwx.cn

[S37] C++：set
来源：http://oh.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hg.szsharing.cn

[S38] C++：排序
来源：http://pc.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://gv.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://oe.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://km.nszjky.cn

[S40] C++：查找元素
来源：http://tw.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ob.lnxyls.cn

[S41] C++：类与构造函数
来源：http://fz.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oc.9csxet.cn

[S42] C++：继承与虚函数
来源：http://qx.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://xt.muxihuayi.cn

[S43] C++：智能指针
来源：http://zf.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://ag.bookmarksfly.cn

[S44] C++：引用传参
来源：http://nk.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://hu.nszjky.cn

[S45] C++：lambda
来源：http://sq.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hi.colortex.cn

[S46] C++：函数模板
来源：http://vj.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ju.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://xp.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nz.hnjuh.cn

[S48] C++：逐行读文件
来源：http://zf.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kt.colortex.cn

while (std::getline(in, line)) { }
来源：http://wz.hnjuh.cn

[S49] C++：写文件
来源：http://ne.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sn.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://zq.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ja.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://er.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://zp.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://yh.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://an.9csxet.cn

[S53] C++：移动语义
来源：http://wd.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://fm.bjjhwx.cn

[S54] C++：异常处理
来源：http://uy.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://io.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://vu.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gg.jianghongdianzi.cn

[S56] C++：optional
来源：http://ja.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wj.panjiajie.cn

[S57] C++：编译期常量
来源：http://rs.9csxet.cn

constexpr int N = 10;
来源：http://ps.9csxet.cn

[S58] C++：命名空间
来源：http://em.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://cr.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://xx.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ke.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://vb.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fu.asd995.cn

================================================================================
来源：http://cs.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oo.chemitech.net.cn

================================================================================
来源：http://fz.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://yf.muxihuayi.cn

println("Hello")
来源：http://us.bjjhwx.cn

[T02] Kotlin：变量
来源：http://rl.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ye.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://di.jianghongdianzi.cn

"值: $b"
来源：http://jx.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://ds.nicolike.cn

val n: String? = null;  n?.length
来源：http://zv.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://em.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://on.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://dp.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://md.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://gp.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ri.szxytkj.cn

[T08] Kotlin：数据类
来源：http://nc.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://xd.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://tq.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://ka.asd995.cn

[T10] Kotlin：默认参数
来源：http://nm.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://im.shxzukj.cn


<!-- 参考信息 -->