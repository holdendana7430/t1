代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://el.chemitech.net.cn

[R08] 数值比较
来源：http://ve.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pv.wgjwhj.cn

[R09] 字符串比较
来源：http://yh.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eh.bjjhwx.cn

[R10] 正则匹配
来源：http://es.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gj.huixinmuqiang.cn

[R11] case 多分支
来源：http://jw.wgjwhj.cn

case "$1" in
来源：http://qh.nszjky.cn

start) echo "启动" ;;
来源：http://df.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://vg.nicolike.cn

*)     echo "未知命令" ;;
来源：http://bs.wgjwhj.cn

esac
来源：http://wi.bookmarksfly.cn

[R12] for 遍历文件
来源：http://vm.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://gv.nicolike.cn

[R13] for 计数循环
来源：http://se.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://wm.nicolike.cn

[R14] C 风格 for
来源：http://wn.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xq.muxihuayi.cn

[R15] while 逐行读文件
来源：http://zg.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tr.nicolike.cn

[R16] until 等待条件
来源：http://on.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yg.9csxet.cn

[R17] 数组定义与取值
来源：http://in.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ck.shtwfgs.cn

[R18] 遍历数组
来源：http://ye.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sa.szxytkj.cn

[R19] 数组长度
来源：http://ul.9csxet.cn

echo "${#arr[@]}"
来源：http://ix.panjiajie.cn

[R20] 关联数组（字典）
来源：http://qe.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://od.nicolike.cn

[R21] 字符串长度
来源：http://uo.521024.cn

echo "${#s}"
来源：http://cg.huixinmuqiang.cn

[R22] 截取子串
来源：http://kj.bookmarksfly.cn

echo "${s:0:5}"
来源：http://jd.yuexingan06.cn

[R23] 字符串替换
来源：http://cy.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rn.yuexingan06.cn

[R24] 大小写转换
来源：http://jd.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nv.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://wi.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cr.colortex.cn

[R26] 命令替换
来源：http://ra.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://xq.jianghongdianzi.cn

[R27] 算术展开
来源：http://qi.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://fo.yuexingan06.cn

[R28] 浮点运算
来源：http://tt.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://to.szsharing.cn

[R29] 定义函数
来源：http://vy.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vb.nicolike.cn

[R30] 函数返回状态码
来源：http://ve.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://du.nszjky.cn

[R31] 局部变量
来源：http://eq.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://pn.haigaiapp.cn

[R32] 参数个数校验
来源：http://cd.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gl.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://on.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nn.muxihuayi.cn

[R34] 退出时清理
来源：http://hc.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nz.gzmigu.cn

[R35] 后台执行并等待
来源：http://ls.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://op.szxytkj.cn

[R36] 并发执行多个任务
来源：http://pk.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yv.asd995.cn

[R37] 把输出赋给变量
来源：http://wb.asd995.cn

files=$(ls -1)
来源：http://ww.yuexingan06.cn

[R38] 管道串联
来源：http://mi.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://qf.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://tu.bjjhwx.cn

cmd > out.log 2>&1
来源：http://zd.haigaiapp.cn

[R40] 追加写日志
来源：http://os.huixinmuqiang.cn

echo "log" >> out.log
来源：http://nz.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://if.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://hx.yuexingan06.cn

[R42] 输入重定向
来源：http://di.shxzukj.cn

wc -l < a.txt
来源：http://yh.hnjuh.cn

[R43] 按名字查找文件
来源：http://ud.szsharing.cn

find . -name "*.log" -type f
来源：http://uo.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://rg.hahajie.cn

find . -mtime -7 -type f
来源：http://as.hnjuh.cn

[R45] 批量删除
来源：http://wx.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://yu.gzmigu.cn

[R46] 递归替换文件内容
来源：http://oi.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sc.nicolike.cn

[R47] sed 单行替换
来源：http://fi.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qf.lnxyls.cn

[R48] awk 取指定列
来源：http://xx.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://js.colortex.cn

[R49] awk 带条件
来源：http://kq.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wc.jianghongdianzi.cn

[R50] awk 求和
来源：http://od.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bh.szxytkj.cn

[R51] 排序去重取前几
来源：http://vx.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zh.newstarts.cn

[R52] 统计行数
来源：http://df.chemitech.net.cn

wc -l a.txt
来源：http://tl.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://gd.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://my.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://jc.hahajie.cn

diff a.txt b.txt
来源：http://qn.bjjhwx.cn

[R55] 压缩与解压
来源：http://kr.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ul.yuexingan06.cn

[R56] 远程拷贝
来源：http://jn.jianghongdianzi.cn

scp file user@host:/path/
来源：http://fd.shxzukj.cn

[R57] 远程执行命令
来源：http://fp.hnjuh.cn

ssh user@host 'uptime'
来源：http://ds.panjiajie.cn

[R58] 下载文件
来源：http://yd.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qe.yuexingan06.cn

[R59] 发 POST JSON
来源：http://ds.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lo.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://ew.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ku.shtwfgs.cn

[R61] 磁盘占用
来源：http://wu.jctech888.com.cn

df -h;  du -sh *
来源：http://eh.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://yl.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://sz.szxytkj.cn

[R63] 内存与进程
来源：http://hb.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://sg.lnxyls.cn

[R64] 结束进程
来源：http://lo.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://cg.panjiajie.cn

[R65] 查看端口占用
来源：http://xh.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oy.panjiajie.cn

[R66] 定时任务
来源：http://uc.haigaiapp.cn

crontab -e;  crontab -l
来源：http://ix.nszjky.cn

[R67] 生成随机十六进制串
来源：http://mc.9csxet.cn

openssl rand -hex 16
来源：http://gj.asd995.cn

[R68] 计算文件校验值
来源：http://nh.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ef.panjiajie.cn

[R69] 生成随机密码
来源：http://su.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://rl.gzmigu.cn

[R70] 时间戳与互转
来源：http://od.colortex.cn

date +%s;  date -d @1700000000
来源：http://ku.yuexingan06.cn

[R71] 日期格式化
来源：http://qh.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cc.muxihuayi.cn

[R72] 等待端口就绪
来源：http://dp.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hf.yuexingan06.cn

[R73] 分割大日志
来源：http://dv.521024.cn

split -l 1000 big.log part_
来源：http://ef.yuexingan06.cn

[R74] 批量重命名
来源：http://af.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lr.asd995.cn

[R75] 导出环境变量
来源：http://pi.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://lw.shxzukj.cn

[R76] 使用临时文件
来源：http://qu.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rt.szxytkj.cn

[R77] 读取用户输入
来源：http://nd.panjiajie.cn

read -rp "请输入: " ans
来源：http://ur.wgjwhj.cn

[R78] 交互式菜单
来源：http://jk.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ng.szxytkj.cn

[R79] 解析命令行选项
来源：http://qm.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://js.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://vv.gzmigu.cn

time ./run.sh
来源：http://ll.shxzskj.cn

================================================================================
来源：http://wt.haigaiapp.cn

S. C / C++ 专题
来源：http://xt.huixinmuqiang.cn

================================================================================
来源：http://hm.9csxet.cn

[S01] C：Hello World
来源：http://ow.asd995.cn

#include <stdio.h>
来源：http://xy.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rl.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://ns.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://ku.wgjwhj.cn

[S03] C：读入整数
来源：http://nb.newstarts.cn

int x; scanf("%d", &x);
来源：http://hu.hahajie.cn

[S04] C：字符串复制
来源：http://bf.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hu.asd995.cn

[S05] C：字符串长度
来源：http://xk.jctech888.com.cn

strlen(s)
来源：http://jx.haigaiapp.cn

[S06] C：字符串比较
来源：http://zw.bjjhwx.cn

strcmp(a, b) == 0
来源：http://fu.huanxung.cn

[S07] C：数组遍历求和
来源：http://lj.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uk.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://tg.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lp.521024.cn

[S09] C：结构体定义与初始化
来源：http://nb.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ni.colortex.cn

[S10] C：指针与解引用
来源：http://ek.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://ih.chemitech.net.cn

[S11] C：逐行读文件
来源：http://jx.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://mb.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jf.huixinmuqiang.cn

fclose(f);
来源：http://ct.bookmarksfly.cn

[S12] C：写文件
来源：http://on.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mk.bjjhwx.cn

[S13] C：宏定义
来源：http://bf.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bw.muxihuayi.cn

[S14] C：枚举
来源：http://ye.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://cn.szsharing.cn

[S15] C：类型转换
来源：http://sc.huanxung.cn

(double) a / b
来源：http://ki.nszjky.cn

[S16] C：位操作置位
来源：http://hj.lnxyls.cn

x |= (1 << 3);
来源：http://qg.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://gj.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ym.521024.cn

[S18] C：命令行参数
来源：http://zn.muxihuayi.cn

int main(int argc, char **argv)
来源：http://vi.bjjhwx.cn

[S19] C：快速排序
来源：http://ta.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xv.wgjwhj.cn

[S20] C：二分查找
来源：http://gn.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://og.panjiajie.cn

[S21] C：字符类别判断
来源：http://qb.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mh.muxihuayi.cn

[S22] C：字符串转数字
来源：http://je.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gi.wgjwhj.cn

[S23] C：随机数
来源：http://kl.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hs.gzmigu.cn

[S24] C：获取本地时间
来源：http://vc.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://py.chemitech.net.cn

[S25] C：内存拷贝
来源：http://dx.shtwfgs.cn

memcpy(dst, src, n);
来源：http://nc.hnjuh.cn

[S26] C：内存清零
来源：http://rv.newstarts.cn

memset(a, 0, sizeof a);
来源：http://hg.hnjuh.cn

[S27] C：定义常量
来源：http://ht.szsharing.cn

const double PI = 3.14159;
来源：http://nq.jctech888.com.cn

[S28] C：静态变量
来源：http://vt.lnxyls.cn

static int counter = 0;
来源：http://dr.yuntaijiaju.cn

[S29] C：变参函数
来源：http://vn.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yn.colortex.cn

[S30] C：头文件保护
来源：http://ie.muxihuayi.cn

#ifndef X_H
来源：http://fp.shxzskj.cn

#define X_H
来源：http://rd.chemitech.net.cn

#endif
来源：http://dg.szsharing.cn

[S31] C++：Hello World
来源：http://ef.shxzskj.cn

#include <iostream>
来源：http://wg.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://nw.shtwfgs.cn

[S32] C++：字符串
来源：http://rv.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://gm.panjiajie.cn

[S33] C++：vector 增删
来源：http://tr.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nn.9csxet.cn

[S34] C++：遍历 vector
来源：http://rh.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ov.shtwfgs.cn

[S35] C++：map
来源：http://ix.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xh.asd995.cn

[S36] C++：unordered_map
来源：http://em.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kn.9csxet.cn

[S37] C++：set
来源：http://ht.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cj.wgjwhj.cn

[S38] C++：排序
来源：http://rb.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://al.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://wl.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zq.szxytkj.cn

[S40] C++：查找元素
来源：http://fz.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qk.9csxet.cn

[S41] C++：类与构造函数
来源：http://dn.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ub.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://bk.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://gk.lnxyls.cn

[S43] C++：智能指针
来源：http://mu.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://zf.chemitech.net.cn

[S44] C++：引用传参
来源：http://xb.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://vf.colortex.cn

[S45] C++：lambda
来源：http://au.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://al.colortex.cn

[S46] C++：函数模板
来源：http://cz.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ch.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://dh.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nx.asd995.cn

[S48] C++：逐行读文件
来源：http://ih.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cr.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://hr.huixinmuqiang.cn

[S49] C++：写文件
来源：http://il.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zv.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://gg.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nx.colortex.cn

[S51] C++：显式类型转换
来源：http://yz.nszjky.cn

static_cast<double>(a) / b
来源：http://qp.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://mh.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://oj.muxihuayi.cn

[S53] C++：移动语义
来源：http://sy.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://rp.nicolike.cn

[S54] C++：异常处理
来源：http://gg.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uo.colortex.cn

[S55] C++：结构化绑定
来源：http://yq.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tt.panjiajie.cn

[S56] C++：optional
来源：http://kx.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ay.shtwfgs.cn

[S57] C++：编译期常量
来源：http://fi.yuexingan06.cn

constexpr int N = 10;
来源：http://or.shtwfgs.cn

[S58] C++：命名空间
来源：http://tv.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://td.lnxyls.cn

[S59] C++：静态断言
来源：http://of.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ug.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://uy.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jc.yuexingan06.cn

================================================================================
来源：http://ac.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xi.huanxung.cn

================================================================================
来源：http://sh.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://oc.asd995.cn

println("Hello")
来源：http://fu.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://wy.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qk.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://df.huanxung.cn

"值: $b"
来源：http://nd.9csxet.cn

[T04] Kotlin：空安全
来源：http://pi.9csxet.cn

val n: String? = null;  n?.length
来源：http://sa.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://cx.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ga.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://uh.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tk.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://lt.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://am.huanxung.cn

[T08] Kotlin：数据类
来源：http://bl.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://nw.haigaiapp.cn


<!-- 参考信息 -->