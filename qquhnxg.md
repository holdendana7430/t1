代发 wailian999

name="${1:-default}"
来源：http://js.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://af.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pu.nszjky.cn

[R07] if 判断文件
来源：http://rs.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fz.bjjhwx.cn

[R08] 数值比较
来源：http://ei.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oj.gzmigu.cn

[R09] 字符串比较
来源：http://gx.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iz.bookmarksfly.cn

[R10] 正则匹配
来源：http://uc.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dz.huanxung.cn

[R11] case 多分支
来源：http://rs.szxytkj.cn

case "$1" in
来源：http://zw.szxytkj.cn

start) echo "启动" ;;
来源：http://vu.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://qj.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://qy.hnjuh.cn

esac
来源：http://gz.yuexingan06.cn

[R12] for 遍历文件
来源：http://qi.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://nz.huixinmuqiang.cn

[R13] for 计数循环
来源：http://bs.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://oe.szsharing.cn

[R14] C 风格 for
来源：http://er.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hq.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://yy.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rh.wgjwhj.cn

[R16] until 等待条件
来源：http://xe.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ff.szxytkj.cn

[R17] 数组定义与取值
来源：http://zn.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vd.bookmarksfly.cn

[R18] 遍历数组
来源：http://yr.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kn.yuntaijiaju.cn

[R19] 数组长度
来源：http://na.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://df.hahajie.cn

[R20] 关联数组（字典）
来源：http://wj.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pb.colortex.cn

[R21] 字符串长度
来源：http://gk.521024.cn

echo "${#s}"
来源：http://pu.wgjwhj.cn

[R22] 截取子串
来源：http://em.newstarts.cn

echo "${s:0:5}"
来源：http://lf.bookmarksfly.cn

[R23] 字符串替换
来源：http://el.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fe.muxihuayi.cn

[R24] 大小写转换
来源：http://wv.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rx.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://dh.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://za.lnxyls.cn

[R26] 命令替换
来源：http://yb.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://lw.nicolike.cn

[R27] 算术展开
来源：http://qh.colortex.cn

echo $((1 + 2 * 3))
来源：http://hi.newstarts.cn

[R28] 浮点运算
来源：http://kx.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://we.yuntaijiaju.cn

[R29] 定义函数
来源：http://ey.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hr.yuexingan06.cn

[R30] 函数返回状态码
来源：http://rx.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://qz.newstarts.cn

[R31] 局部变量
来源：http://gj.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://oo.bookmarksfly.cn

[R32] 参数个数校验
来源：http://ps.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bg.colortex.cn

[R33] 捕获错误并提示行号
来源：http://zm.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cz.yuntaijiaju.cn

[R34] 退出时清理
来源：http://mx.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qn.panjiajie.cn

[R35] 后台执行并等待
来源：http://zl.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wz.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://vc.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fd.colortex.cn

[R37] 把输出赋给变量
来源：http://tl.wgjwhj.cn

files=$(ls -1)
来源：http://um.521024.cn

[R38] 管道串联
来源：http://sm.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://ec.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://sy.wgjwhj.cn

cmd > out.log 2>&1
来源：http://zt.hnjuh.cn

[R40] 追加写日志
来源：http://wa.asd995.cn

echo "log" >> out.log
来源：http://my.chemitech.net.cn

[R41] 丢弃输出
来源：http://pj.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://yd.9csxet.cn

[R42] 输入重定向
来源：http://cb.nszjky.cn

wc -l < a.txt
来源：http://gm.521024.cn

[R43] 按名字查找文件
来源：http://co.nicolike.cn

find . -name "*.log" -type f
来源：http://ro.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://cn.szxytkj.cn

find . -mtime -7 -type f
来源：http://ax.gzmigu.cn

[R45] 批量删除
来源：http://ce.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://cn.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://ek.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://td.nszjky.cn

[R47] sed 单行替换
来源：http://xi.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mp.muxihuayi.cn

[R48] awk 取指定列
来源：http://hp.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://xw.bookmarksfly.cn

[R49] awk 带条件
来源：http://kf.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nc.chemitech.net.cn

[R50] awk 求和
来源：http://pz.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ne.haigaiapp.cn

[R51] 排序去重取前几
来源：http://aq.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ga.nszjky.cn

[R52] 统计行数
来源：http://xy.jianghongdianzi.cn

wc -l a.txt
来源：http://cy.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://iq.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jr.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://nq.hahajie.cn

diff a.txt b.txt
来源：http://bu.9csxet.cn

[R55] 压缩与解压
来源：http://cg.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://na.shtwfgs.cn

[R56] 远程拷贝
来源：http://dl.lnxyls.cn

scp file user@host:/path/
来源：http://fi.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://be.asd995.cn

ssh user@host 'uptime'
来源：http://ex.asd995.cn

[R58] 下载文件
来源：http://sh.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wq.colortex.cn

[R59] 发 POST JSON
来源：http://bq.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ur.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://cn.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nb.hnjuh.cn

[R61] 磁盘占用
来源：http://uf.gzmigu.cn

df -h;  du -sh *
来源：http://pd.nicolike.cn

[R62] 找最占空间的文件
来源：http://zx.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://xa.521024.cn

[R63] 内存与进程
来源：http://id.521024.cn

free -h;  ps aux | grep nginx
来源：http://bi.huixiangedu.cn

[R64] 结束进程
来源：http://zh.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://vn.huixiangedu.cn

[R65] 查看端口占用
来源：http://ok.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uc.shtwfgs.cn

[R66] 定时任务
来源：http://rh.lnxyls.cn

crontab -e;  crontab -l
来源：http://mm.huanxung.cn

[R67] 生成随机十六进制串
来源：http://ki.chemitech.net.cn

openssl rand -hex 16
来源：http://cv.shxzskj.cn

[R68] 计算文件校验值
来源：http://ab.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cq.colortex.cn

[R69] 生成随机密码
来源：http://ta.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://cb.newstarts.cn

[R70] 时间戳与互转
来源：http://ha.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://ko.hnjuh.cn

[R71] 日期格式化
来源：http://ms.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fo.colortex.cn

[R72] 等待端口就绪
来源：http://mr.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tr.shtwfgs.cn

[R73] 分割大日志
来源：http://lq.shtwfgs.cn

split -l 1000 big.log part_
来源：http://me.hahajie.cn

[R74] 批量重命名
来源：http://tc.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xd.colortex.cn

[R75] 导出环境变量
来源：http://zc.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://cq.colortex.cn

[R76] 使用临时文件
来源：http://tn.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ni.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://cb.szxytkj.cn

read -rp "请输入: " ans
来源：http://vw.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://lf.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://da.9csxet.cn

[R79] 解析命令行选项
来源：http://ec.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://si.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://lt.colortex.cn

time ./run.sh
来源：http://tp.nszjky.cn

================================================================================
来源：http://ok.yuntaijiaju.cn

S. C / C++ 专题
来源：http://rb.szxytkj.cn

================================================================================
来源：http://pz.nicolike.cn

[S01] C：Hello World
来源：http://ba.newstarts.cn

#include <stdio.h>
来源：http://ra.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yo.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://fi.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://wk.szsharing.cn

[S03] C：读入整数
来源：http://do.nszjky.cn

int x; scanf("%d", &x);
来源：http://ce.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://jt.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gv.asd995.cn

[S05] C：字符串长度
来源：http://nb.shtwfgs.cn

strlen(s)
来源：http://jv.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://la.muxihuayi.cn

strcmp(a, b) == 0
来源：http://oz.shxzskj.cn

[S07] C：数组遍历求和
来源：http://ky.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uw.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://gm.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hj.521024.cn

[S09] C：结构体定义与初始化
来源：http://ct.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://do.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://wc.asd995.cn

int *p = &a;  *p = 5;
来源：http://jc.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://gy.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://st.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hv.haigaiapp.cn

fclose(f);
来源：http://gl.hnjuh.cn

[S12] C：写文件
来源：http://yd.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vm.bjjhwx.cn

[S13] C：宏定义
来源：http://pv.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vb.nicolike.cn

[S14] C：枚举
来源：http://sk.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://rr.shxzukj.cn

[S15] C：类型转换
来源：http://fd.jianghongdianzi.cn

(double) a / b
来源：http://un.muxihuayi.cn

[S16] C：位操作置位
来源：http://tg.shxzukj.cn

x |= (1 << 3);
来源：http://qy.521024.cn

[S17] C：安全拼接字符串
来源：http://lb.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wk.huanxung.cn

[S18] C：命令行参数
来源：http://fa.haigaiapp.cn

int main(int argc, char **argv)
来源：http://tg.huixiangedu.cn

[S19] C：快速排序
来源：http://yf.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vf.haigaiapp.cn

[S20] C：二分查找
来源：http://ld.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vy.9csxet.cn

[S21] C：字符类别判断
来源：http://ls.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mc.chemitech.net.cn

[S22] C：字符串转数字
来源：http://tb.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sf.9csxet.cn

[S23] C：随机数
来源：http://xx.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vi.haigaiapp.cn

[S24] C：获取本地时间
来源：http://as.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uk.bjjhwx.cn

[S25] C：内存拷贝
来源：http://nz.yuexingan06.cn

memcpy(dst, src, n);
来源：http://eg.panjiajie.cn

[S26] C：内存清零
来源：http://oo.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://dz.gzmigu.cn

[S27] C：定义常量
来源：http://eq.hnjuh.cn

const double PI = 3.14159;
来源：http://yd.asd995.cn

[S28] C：静态变量
来源：http://ve.colortex.cn

static int counter = 0;
来源：http://jh.shtwfgs.cn

[S29] C：变参函数
来源：http://ur.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dm.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://hm.huixinmuqiang.cn

#ifndef X_H
来源：http://zv.hahajie.cn

#define X_H
来源：http://ms.9csxet.cn

#endif
来源：http://gg.asd995.cn

[S31] C++：Hello World
来源：http://le.521024.cn

#include <iostream>
来源：http://sk.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://mk.9csxet.cn

[S32] C++：字符串
来源：http://cx.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://tc.yuexingan06.cn

[S33] C++：vector 增删
来源：http://gy.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cv.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://za.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://nh.newstarts.cn

[S35] C++：map
来源：http://zt.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eg.lnxyls.cn

[S36] C++：unordered_map
来源：http://pq.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jo.chemitech.net.cn

[S37] C++：set
来源：http://ri.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://te.bookmarksfly.cn

[S38] C++：排序
来源：http://tu.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://xc.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://dn.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dr.muxihuayi.cn

[S40] C++：查找元素
来源：http://gc.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nz.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://vq.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://to.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://uw.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://oz.bookmarksfly.cn

[S43] C++：智能指针
来源：http://mz.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://me.9csxet.cn

[S44] C++：引用传参
来源：http://uo.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://ix.lnxyls.cn

[S45] C++：lambda
来源：http://qu.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fy.wgjwhj.cn

[S46] C++：函数模板
来源：http://fx.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nk.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://rw.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ok.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://tz.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kr.colortex.cn

while (std::getline(in, line)) { }
来源：http://zv.huanxung.cn

[S49] C++：写文件
来源：http://kh.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cc.9csxet.cn

[S50] C++：格式化数字
来源：http://hy.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pw.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://dt.newstarts.cn

static_cast<double>(a) / b
来源：http://qe.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://rr.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://ht.newstarts.cn

[S53] C++：移动语义
来源：http://zt.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://uu.colortex.cn

[S54] C++：异常处理
来源：http://cr.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hm.szsharing.cn

[S55] C++：结构化绑定
来源：http://hn.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hb.chemitech.net.cn

[S56] C++：optional
来源：http://jh.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iu.nicolike.cn

[S57] C++：编译期常量
来源：http://jk.bjjhwx.cn

constexpr int N = 10;
来源：http://vy.newstarts.cn

[S58] C++：命名空间
来源：http://dz.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://oq.huanxung.cn

[S59] C++：静态断言
来源：http://tc.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ra.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://gf.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://li.jianghongdianzi.cn

================================================================================
来源：http://vw.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nu.yuntaijiaju.cn

================================================================================
来源：http://zz.huanxung.cn

[T01] Kotlin：Hello World
来源：http://ay.521024.cn

println("Hello")
来源：http://zc.szsharing.cn

[T02] Kotlin：变量
来源：http://tp.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://av.colortex.cn

[T03] Kotlin：字符串模板
来源：http://mm.wgjwhj.cn

"值: $b"
来源：http://ux.nszjky.cn

[T04] Kotlin：空安全
来源：http://qy.szxytkj.cn

val n: String? = null;  n?.length
来源：http://hn.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://uy.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wd.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://wl.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fh.szsharing.cn


<!-- 参考信息 -->