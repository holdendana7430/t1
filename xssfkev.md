代发 wailian999

name="${1:-default}"
来源：http://gk.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://gt.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fs.huanxung.cn

[R07] if 判断文件
来源：http://mc.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yy.hahajie.cn

[R08] 数值比较
来源：http://gh.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nj.asd995.cn

[R09] 字符串比较
来源：http://ht.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rz.asd995.cn

[R10] 正则匹配
来源：http://qw.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ty.yuntaijiaju.cn

[R11] case 多分支
来源：http://co.shtwfgs.cn

case "$1" in
来源：http://wn.huixiangedu.cn

start) echo "启动" ;;
来源：http://eq.lnxyls.cn

stop)  echo "停止" ;;
来源：http://xj.nszjky.cn

*)     echo "未知命令" ;;
来源：http://fy.muxihuayi.cn

esac
来源：http://gm.521024.cn

[R12] for 遍历文件
来源：http://ps.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://wd.shtwfgs.cn

[R13] for 计数循环
来源：http://qa.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://ty.shxzskj.cn

[R14] C 风格 for
来源：http://oe.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ym.hahajie.cn

[R15] while 逐行读文件
来源：http://pi.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qf.asd995.cn

[R16] until 等待条件
来源：http://xr.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ec.lnxyls.cn

[R17] 数组定义与取值
来源：http://dx.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gs.521024.cn

[R18] 遍历数组
来源：http://oo.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tl.huixiangedu.cn

[R19] 数组长度
来源：http://vz.wgjwhj.cn

echo "${#arr[@]}"
来源：http://et.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://xf.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rm.jianghongdianzi.cn

[R21] 字符串长度
来源：http://ln.hnjuh.cn

echo "${#s}"
来源：http://yk.szxytkj.cn

[R22] 截取子串
来源：http://yy.bjjhwx.cn

echo "${s:0:5}"
来源：http://wq.gzmigu.cn

[R23] 字符串替换
来源：http://bp.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://la.szxytkj.cn

[R24] 大小写转换
来源：http://yq.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://st.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://ef.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xh.newstarts.cn

[R26] 命令替换
来源：http://jm.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://vy.shtwfgs.cn

[R27] 算术展开
来源：http://iu.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://ip.yuexingan06.cn

[R28] 浮点运算
来源：http://jy.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://ow.9csxet.cn

[R29] 定义函数
来源：http://zf.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vg.shtwfgs.cn

[R30] 函数返回状态码
来源：http://sr.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://fu.9csxet.cn

[R31] 局部变量
来源：http://ap.521024.cn

f() { local x=1; echo "$x"; }
来源：http://kz.9csxet.cn

[R32] 参数个数校验
来源：http://yq.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zo.asd995.cn

[R33] 捕获错误并提示行号
来源：http://lg.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fo.gzmigu.cn

[R34] 退出时清理
来源：http://py.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://re.muxihuayi.cn

[R35] 后台执行并等待
来源：http://yj.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qw.gzmigu.cn

[R36] 并发执行多个任务
来源：http://kz.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://af.hahajie.cn

[R37] 把输出赋给变量
来源：http://hs.haigaiapp.cn

files=$(ls -1)
来源：http://uj.huixinmuqiang.cn

[R38] 管道串联
来源：http://nu.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://dl.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://nt.muxihuayi.cn

cmd > out.log 2>&1
来源：http://xd.shxzukj.cn

[R40] 追加写日志
来源：http://nu.panjiajie.cn

echo "log" >> out.log
来源：http://md.newstarts.cn

[R41] 丢弃输出
来源：http://fm.newstarts.cn

cmd >/dev/null 2>&1
来源：http://mo.shxzukj.cn

[R42] 输入重定向
来源：http://bm.bjjhwx.cn

wc -l < a.txt
来源：http://gw.asd995.cn

[R43] 按名字查找文件
来源：http://gm.hnjuh.cn

find . -name "*.log" -type f
来源：http://ff.shtwfgs.cn

[R44] 按修改时间查找
来源：http://mb.chemitech.net.cn

find . -mtime -7 -type f
来源：http://uo.hahajie.cn

[R45] 批量删除
来源：http://wp.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://el.szsharing.cn

[R46] 递归替换文件内容
来源：http://ox.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uh.szsharing.cn

[R47] sed 单行替换
来源：http://xh.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yx.newstarts.cn

[R48] awk 取指定列
来源：http://pk.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://vu.newstarts.cn

[R49] awk 带条件
来源：http://yz.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qi.wgjwhj.cn

[R50] awk 求和
来源：http://mg.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hx.colortex.cn

[R51] 排序去重取前几
来源：http://xe.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xs.huixiangedu.cn

[R52] 统计行数
来源：http://gk.nicolike.cn

wc -l a.txt
来源：http://yl.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://wg.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zc.bookmarksfly.cn

[R54] 比较两个文件
来源：http://hn.wgjwhj.cn

diff a.txt b.txt
来源：http://so.hahajie.cn

[R55] 压缩与解压
来源：http://oc.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lp.shxzskj.cn

[R56] 远程拷贝
来源：http://to.huixinmuqiang.cn

scp file user@host:/path/
来源：http://dn.haigaiapp.cn

[R57] 远程执行命令
来源：http://pd.haigaiapp.cn

ssh user@host 'uptime'
来源：http://rm.huixinmuqiang.cn

[R58] 下载文件
来源：http://ca.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ia.521024.cn

[R59] 发 POST JSON
来源：http://qk.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xz.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://ya.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://js.shtwfgs.cn

[R61] 磁盘占用
来源：http://iq.hnjuh.cn

df -h;  du -sh *
来源：http://jw.gzmigu.cn

[R62] 找最占空间的文件
来源：http://wa.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://go.gzmigu.cn

[R63] 内存与进程
来源：http://cj.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://ba.bookmarksfly.cn

[R64] 结束进程
来源：http://qc.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://nz.gzmigu.cn

[R65] 查看端口占用
来源：http://hs.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pu.szsharing.cn

[R66] 定时任务
来源：http://hm.gzmigu.cn

crontab -e;  crontab -l
来源：http://rv.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://by.szxytkj.cn

openssl rand -hex 16
来源：http://av.shxzskj.cn

[R68] 计算文件校验值
来源：http://ce.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vw.chemitech.net.cn

[R69] 生成随机密码
来源：http://pm.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://az.shxzukj.cn

[R70] 时间戳与互转
来源：http://fb.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://gf.asd995.cn

[R71] 日期格式化
来源：http://jw.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kc.gzmigu.cn

[R72] 等待端口就绪
来源：http://gf.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ag.colortex.cn

[R73] 分割大日志
来源：http://nh.shxzskj.cn

split -l 1000 big.log part_
来源：http://zf.huanxung.cn

[R74] 批量重命名
来源：http://uu.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qu.jctech888.com.cn

[R75] 导出环境变量
来源：http://ik.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://tj.bookmarksfly.cn

[R76] 使用临时文件
来源：http://ov.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tv.521024.cn

[R77] 读取用户输入
来源：http://dt.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://kn.shxzukj.cn

[R78] 交互式菜单
来源：http://np.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ge.521024.cn

[R79] 解析命令行选项
来源：http://me.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oj.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://du.521024.cn

time ./run.sh
来源：http://ts.yuexingan06.cn

================================================================================
来源：http://oa.newstarts.cn

S. C / C++ 专题
来源：http://mn.bjjhwx.cn

================================================================================
来源：http://ld.wgjwhj.cn

[S01] C：Hello World
来源：http://nk.huixiangedu.cn

#include <stdio.h>
来源：http://gz.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wm.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://yl.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://qy.szsharing.cn

[S03] C：读入整数
来源：http://gi.asd995.cn

int x; scanf("%d", &x);
来源：http://jo.huanxung.cn

[S04] C：字符串复制
来源：http://fq.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oy.gzmigu.cn

[S05] C：字符串长度
来源：http://eb.haigaiapp.cn

strlen(s)
来源：http://ix.bjjhwx.cn

[S06] C：字符串比较
来源：http://ii.szxytkj.cn

strcmp(a, b) == 0
来源：http://al.lnxyls.cn

[S07] C：数组遍历求和
来源：http://mp.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ah.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://re.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lm.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://vl.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gy.lnxyls.cn

[S10] C：指针与解引用
来源：http://mx.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://bm.szxytkj.cn

[S11] C：逐行读文件
来源：http://kh.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://in.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dh.szxytkj.cn

fclose(f);
来源：http://zt.chemitech.net.cn

[S12] C：写文件
来源：http://mx.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ls.shxzukj.cn

[S13] C：宏定义
来源：http://sm.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kd.nicolike.cn

[S14] C：枚举
来源：http://lg.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://ll.wgjwhj.cn

[S15] C：类型转换
来源：http://jr.newstarts.cn

(double) a / b
来源：http://na.521024.cn

[S16] C：位操作置位
来源：http://ke.bookmarksfly.cn

x |= (1 << 3);
来源：http://he.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://df.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://go.shtwfgs.cn

[S18] C：命令行参数
来源：http://mc.szsharing.cn

int main(int argc, char **argv)
来源：http://tj.shxzskj.cn

[S19] C：快速排序
来源：http://go.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mw.huanxung.cn

[S20] C：二分查找
来源：http://tk.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bq.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://bo.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fh.huixiangedu.cn

[S22] C：字符串转数字
来源：http://ea.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lg.jianghongdianzi.cn

[S23] C：随机数
来源：http://jq.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ew.nicolike.cn

[S24] C：获取本地时间
来源：http://yp.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cu.hahajie.cn

[S25] C：内存拷贝
来源：http://dq.huixiangedu.cn

memcpy(dst, src, n);
来源：http://ba.szxytkj.cn

[S26] C：内存清零
来源：http://yw.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://xw.szxytkj.cn

[S27] C：定义常量
来源：http://jq.shtwfgs.cn

const double PI = 3.14159;
来源：http://cw.haigaiapp.cn

[S28] C：静态变量
来源：http://hf.yuexingan06.cn

static int counter = 0;
来源：http://sy.yuntaijiaju.cn

[S29] C：变参函数
来源：http://xp.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xs.hahajie.cn

[S30] C：头文件保护
来源：http://di.haigaiapp.cn

#ifndef X_H
来源：http://fe.yuntaijiaju.cn

#define X_H
来源：http://qr.bjjhwx.cn

#endif
来源：http://lp.huixiangedu.cn

[S31] C++：Hello World
来源：http://lf.yuntaijiaju.cn

#include <iostream>
来源：http://dp.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://kz.9csxet.cn

[S32] C++：字符串
来源：http://xp.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://sp.lnxyls.cn

[S33] C++：vector 增删
来源：http://ys.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://su.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://hj.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://zv.yuntaijiaju.cn

[S35] C++：map
来源：http://ax.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cu.haigaiapp.cn

[S36] C++：unordered_map
来源：http://zh.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sj.newstarts.cn

[S37] C++：set
来源：http://vn.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pm.9csxet.cn

[S38] C++：排序
来源：http://ie.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://du.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://te.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sj.bjjhwx.cn

[S40] C++：查找元素
来源：http://td.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ar.shxzskj.cn

[S41] C++：类与构造函数
来源：http://lx.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ko.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://ww.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://ki.jctech888.com.cn

[S43] C++：智能指针
来源：http://ec.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://tw.asd995.cn

[S44] C++：引用传参
来源：http://xz.szsharing.cn

void inc(int &x) { ++x; }
来源：http://wj.yuexingan06.cn

[S45] C++：lambda
来源：http://fe.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ey.521024.cn

[S46] C++：函数模板
来源：http://ag.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xl.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://po.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oi.gzmigu.cn

[S48] C++：逐行读文件
来源：http://pm.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pg.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://vx.jianghongdianzi.cn

[S49] C++：写文件
来源：http://ry.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jx.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://bk.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://to.szsharing.cn

[S51] C++：显式类型转换
来源：http://rh.szxytkj.cn

static_cast<double>(a) / b
来源：http://zt.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://jo.colortex.cn

int size() const noexcept { return n_; }
来源：http://gv.shtwfgs.cn

[S53] C++：移动语义
来源：http://sf.521024.cn

std::vector<int> w = std::move(v);
来源：http://hf.521024.cn

[S54] C++：异常处理
来源：http://ri.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://af.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://ln.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ku.gzmigu.cn

[S56] C++：optional
来源：http://fw.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ld.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://eq.huixiangedu.cn

constexpr int N = 10;
来源：http://rg.bjjhwx.cn

[S58] C++：命名空间
来源：http://my.521024.cn

namespace ns { int f() { return 1; } }
来源：http://kn.shtwfgs.cn

[S59] C++：静态断言
来源：http://xw.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ac.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://ds.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xs.shtwfgs.cn

================================================================================
来源：http://ki.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pb.huixiangedu.cn

================================================================================
来源：http://xe.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://zd.huixinmuqiang.cn

println("Hello")
来源：http://lx.huixiangedu.cn

[T02] Kotlin：变量
来源：http://ke.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fz.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://bx.newstarts.cn

"值: $b"
来源：http://uv.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://qa.9csxet.cn

val n: String? = null;  n?.length
来源：http://jv.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://va.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ua.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://sd.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tf.szsharing.cn


<!-- 参考信息 -->