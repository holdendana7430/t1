代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cp.9csxet.cn

[R08] 数值比较
来源：http://ns.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://is.shxzukj.cn

[R09] 字符串比较
来源：http://ew.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ln.muxihuayi.cn

[R10] 正则匹配
来源：http://id.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ki.colortex.cn

[R11] case 多分支
来源：http://vi.yuntaijiaju.cn

case "$1" in
来源：http://hm.shxzskj.cn

start) echo "启动" ;;
来源：http://jz.szsharing.cn

stop)  echo "停止" ;;
来源：http://og.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://la.huanxung.cn

esac
来源：http://bv.nicolike.cn

[R12] for 遍历文件
来源：http://rs.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://fl.haigaiapp.cn

[R13] for 计数循环
来源：http://xx.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://lx.huixinmuqiang.cn

[R14] C 风格 for
来源：http://fi.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nj.jctech888.com.cn

[R15] while 逐行读文件
来源：http://ea.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ss.panjiajie.cn

[R16] until 等待条件
来源：http://qx.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vu.szxytkj.cn

[R17] 数组定义与取值
来源：http://yl.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kc.shxzskj.cn

[R18] 遍历数组
来源：http://us.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://le.huixinmuqiang.cn

[R19] 数组长度
来源：http://xw.bjjhwx.cn

echo "${#arr[@]}"
来源：http://eh.lnxyls.cn

[R20] 关联数组（字典）
来源：http://so.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kq.9csxet.cn

[R21] 字符串长度
来源：http://tq.huixinmuqiang.cn

echo "${#s}"
来源：http://ey.szxytkj.cn

[R22] 截取子串
来源：http://pp.szsharing.cn

echo "${s:0:5}"
来源：http://my.yuntaijiaju.cn

[R23] 字符串替换
来源：http://ed.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ep.panjiajie.cn

[R24] 大小写转换
来源：http://zs.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ei.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://oz.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xj.chemitech.net.cn

[R26] 命令替换
来源：http://do.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://fx.9csxet.cn

[R27] 算术展开
来源：http://xj.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://cw.yuexingan06.cn

[R28] 浮点运算
来源：http://nc.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://jj.nicolike.cn

[R29] 定义函数
来源：http://ux.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cb.panjiajie.cn

[R30] 函数返回状态码
来源：http://vu.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://zg.haigaiapp.cn

[R31] 局部变量
来源：http://xv.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://hr.bookmarksfly.cn

[R32] 参数个数校验
来源：http://wx.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://db.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://hr.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ly.yuexingan06.cn

[R34] 退出时清理
来源：http://qn.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hi.wgjwhj.cn

[R35] 后台执行并等待
来源：http://hp.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gj.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://yr.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dc.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://dp.bookmarksfly.cn

files=$(ls -1)
来源：http://wh.shxzukj.cn

[R38] 管道串联
来源：http://dk.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://ms.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://it.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://qo.haigaiapp.cn

[R40] 追加写日志
来源：http://eg.colortex.cn

echo "log" >> out.log
来源：http://la.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://xg.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://lv.9csxet.cn

[R42] 输入重定向
来源：http://gy.hahajie.cn

wc -l < a.txt
来源：http://fq.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://iv.nicolike.cn

find . -name "*.log" -type f
来源：http://rx.9csxet.cn

[R44] 按修改时间查找
来源：http://ik.szsharing.cn

find . -mtime -7 -type f
来源：http://ig.9csxet.cn

[R45] 批量删除
来源：http://fe.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://or.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://hx.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sc.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://xf.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sr.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://jt.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://qc.yuntaijiaju.cn

[R49] awk 带条件
来源：http://xf.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gy.huixiangedu.cn

[R50] awk 求和
来源：http://bl.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tq.hahajie.cn

[R51] 排序去重取前几
来源：http://wk.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uh.newstarts.cn

[R52] 统计行数
来源：http://bv.jianghongdianzi.cn

wc -l a.txt
来源：http://uv.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://wv.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://od.asd995.cn

[R54] 比较两个文件
来源：http://wg.yuexingan06.cn

diff a.txt b.txt
来源：http://sw.wgjwhj.cn

[R55] 压缩与解压
来源：http://ob.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mk.nicolike.cn

[R56] 远程拷贝
来源：http://fs.colortex.cn

scp file user@host:/path/
来源：http://df.hahajie.cn

[R57] 远程执行命令
来源：http://ga.lnxyls.cn

ssh user@host 'uptime'
来源：http://vd.huixiangedu.cn

[R58] 下载文件
来源：http://iw.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zu.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://db.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jb.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://sn.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cq.haigaiapp.cn

[R61] 磁盘占用
来源：http://tx.szsharing.cn

df -h;  du -sh *
来源：http://cj.szsharing.cn

[R62] 找最占空间的文件
来源：http://wm.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://md.huixinmuqiang.cn

[R63] 内存与进程
来源：http://nj.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://qr.yuntaijiaju.cn

[R64] 结束进程
来源：http://re.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://ii.hahajie.cn

[R65] 查看端口占用
来源：http://sv.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dt.muxihuayi.cn

[R66] 定时任务
来源：http://xd.hahajie.cn

crontab -e;  crontab -l
来源：http://jb.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://wp.wgjwhj.cn

openssl rand -hex 16
来源：http://vk.haigaiapp.cn

[R68] 计算文件校验值
来源：http://ja.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wl.jctech888.com.cn

[R69] 生成随机密码
来源：http://rc.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://wc.9csxet.cn

[R70] 时间戳与互转
来源：http://rr.colortex.cn

date +%s;  date -d @1700000000
来源：http://dy.wgjwhj.cn

[R71] 日期格式化
来源：http://ld.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ba.huanxung.cn

[R72] 等待端口就绪
来源：http://yx.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gt.huanxung.cn

[R73] 分割大日志
来源：http://mw.chemitech.net.cn

split -l 1000 big.log part_
来源：http://gz.newstarts.cn

[R74] 批量重命名
来源：http://mj.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://an.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://hh.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://id.colortex.cn

[R76] 使用临时文件
来源：http://uy.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vr.gzmigu.cn

[R77] 读取用户输入
来源：http://ve.jctech888.com.cn

read -rp "请输入: " ans
来源：http://mt.shxzskj.cn

[R78] 交互式菜单
来源：http://jp.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tb.szxytkj.cn

[R79] 解析命令行选项
来源：http://pt.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hp.colortex.cn

[R80] 查看脚本执行耗时
来源：http://js.shxzukj.cn

time ./run.sh
来源：http://jt.9csxet.cn

================================================================================
来源：http://jj.bookmarksfly.cn

S. C / C++ 专题
来源：http://jk.lnxyls.cn

================================================================================
来源：http://ac.nicolike.cn

[S01] C：Hello World
来源：http://fa.colortex.cn

#include <stdio.h>
来源：http://mw.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rz.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://fn.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://uw.9csxet.cn

[S03] C：读入整数
来源：http://eo.shxzskj.cn

int x; scanf("%d", &x);
来源：http://kg.shxzskj.cn

[S04] C：字符串复制
来源：http://rl.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ir.wgjwhj.cn

[S05] C：字符串长度
来源：http://sw.huanxung.cn

strlen(s)
来源：http://dx.hnjuh.cn

[S06] C：字符串比较
来源：http://zv.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://ay.gzmigu.cn

[S07] C：数组遍历求和
来源：http://kj.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zh.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://mt.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ho.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://ed.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hp.shxzskj.cn

[S10] C：指针与解引用
来源：http://eo.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://on.gzmigu.cn

[S11] C：逐行读文件
来源：http://nu.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://yg.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tl.shtwfgs.cn

fclose(f);
来源：http://fp.huixinmuqiang.cn

[S12] C：写文件
来源：http://pc.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xg.szxytkj.cn

[S13] C：宏定义
来源：http://su.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bv.jianghongdianzi.cn

[S14] C：枚举
来源：http://dj.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ti.szsharing.cn

[S15] C：类型转换
来源：http://tn.huanxung.cn

(double) a / b
来源：http://qm.nszjky.cn

[S16] C：位操作置位
来源：http://ze.gzmigu.cn

x |= (1 << 3);
来源：http://wi.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://ba.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ix.yuexingan06.cn

[S18] C：命令行参数
来源：http://nc.szsharing.cn

int main(int argc, char **argv)
来源：http://wb.newstarts.cn

[S19] C：快速排序
来源：http://hq.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pu.colortex.cn

[S20] C：二分查找
来源：http://al.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ht.gzmigu.cn

[S21] C：字符类别判断
来源：http://zu.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rl.chemitech.net.cn

[S22] C：字符串转数字
来源：http://do.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lm.9csxet.cn

[S23] C：随机数
来源：http://eq.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://is.szsharing.cn

[S24] C：获取本地时间
来源：http://qk.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ll.huanxung.cn

[S25] C：内存拷贝
来源：http://cj.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://ci.newstarts.cn

[S26] C：内存清零
来源：http://yy.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://of.szsharing.cn

[S27] C：定义常量
来源：http://hw.panjiajie.cn

const double PI = 3.14159;
来源：http://xe.yuntaijiaju.cn

[S28] C：静态变量
来源：http://es.bjjhwx.cn

static int counter = 0;
来源：http://ly.huixiangedu.cn

[S29] C：变参函数
来源：http://sr.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ed.shtwfgs.cn

[S30] C：头文件保护
来源：http://bi.shtwfgs.cn

#ifndef X_H
来源：http://xl.shxzukj.cn

#define X_H
来源：http://rv.yuexingan06.cn

#endif
来源：http://vu.shtwfgs.cn

[S31] C++：Hello World
来源：http://mf.colortex.cn

#include <iostream>
来源：http://xl.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://hc.nicolike.cn

[S32] C++：字符串
来源：http://sh.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://yk.nicolike.cn

[S33] C++：vector 增删
来源：http://kw.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hh.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://do.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://td.9csxet.cn

[S35] C++：map
来源：http://vu.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://za.nszjky.cn

[S36] C++：unordered_map
来源：http://fu.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gk.panjiajie.cn

[S37] C++：set
来源：http://rr.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fm.asd995.cn

[S38] C++：排序
来源：http://ci.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://dp.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://on.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ei.nicolike.cn

[S40] C++：查找元素
来源：http://jx.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uy.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://qc.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hh.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://dr.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://ow.huanxung.cn

[S43] C++：智能指针
来源：http://rh.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://gx.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://xz.hahajie.cn

void inc(int &x) { ++x; }
来源：http://vr.muxihuayi.cn

[S45] C++：lambda
来源：http://wk.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zt.bookmarksfly.cn

[S46] C++：函数模板
来源：http://fj.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hm.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://su.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ft.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://if.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dp.nicolike.cn

while (std::getline(in, line)) { }
来源：http://qr.bjjhwx.cn

[S49] C++：写文件
来源：http://iw.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ma.huixiangedu.cn

[S50] C++：格式化数字
来源：http://yb.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uu.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://lm.huixiangedu.cn

static_cast<double>(a) / b
来源：http://ym.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://bt.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://vw.panjiajie.cn

[S53] C++：移动语义
来源：http://nh.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://jt.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://gq.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ni.huanxung.cn

[S55] C++：结构化绑定
来源：http://ob.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gf.hahajie.cn

[S56] C++：optional
来源：http://sh.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pf.asd995.cn

[S57] C++：编译期常量
来源：http://xv.huanxung.cn

constexpr int N = 10;
来源：http://ky.shtwfgs.cn

[S58] C++：命名空间
来源：http://xb.521024.cn

namespace ns { int f() { return 1; } }
来源：http://jc.hnjuh.cn

[S59] C++：静态断言
来源：http://hm.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ai.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://kw.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jf.nszjky.cn

================================================================================
来源：http://pg.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fb.jctech888.com.cn

================================================================================
来源：http://yh.nszjky.cn

[T01] Kotlin：Hello World
来源：http://uq.shxzukj.cn

println("Hello")
来源：http://vj.9csxet.cn

[T02] Kotlin：变量
来源：http://yw.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://me.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://ex.chemitech.net.cn

"值: $b"
来源：http://fj.szsharing.cn

[T04] Kotlin：空安全
来源：http://yt.hnjuh.cn

val n: String? = null;  n?.length
来源：http://gn.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://oz.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://er.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://mu.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vz.huixinmuqiang.cn

[T07] Kotlin：集合过滤
来源：http://og.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ou.9csxet.cn

[T08] Kotlin：数据类
来源：http://xl.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://sn.shxzskj.cn


<!-- 参考信息 -->