代发 wailian999

name="${1:-default}"
来源：http://zi.szxytkj.cn

[R06] 判断命令是否存在
来源：http://up.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vd.shtwfgs.cn

[R07] if 判断文件
来源：http://by.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zn.shxzskj.cn

[R08] 数值比较
来源：http://mm.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ud.521024.cn

[R09] 字符串比较
来源：http://kp.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ga.szsharing.cn

[R10] 正则匹配
来源：http://xq.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uk.bjjhwx.cn

[R11] case 多分支
来源：http://sv.nszjky.cn

case "$1" in
来源：http://nf.wgjwhj.cn

start) echo "启动" ;;
来源：http://qp.nszjky.cn

stop)  echo "停止" ;;
来源：http://wa.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://ft.nszjky.cn

esac
来源：http://qa.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://zm.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://sx.lnxyls.cn

[R13] for 计数循环
来源：http://oo.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://yw.yuexingan06.cn

[R14] C 风格 for
来源：http://kv.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sr.huanxung.cn

[R15] while 逐行读文件
来源：http://yg.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fa.lnxyls.cn

[R16] until 等待条件
来源：http://hd.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vk.asd995.cn

[R17] 数组定义与取值
来源：http://la.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rx.szsharing.cn

[R18] 遍历数组
来源：http://ac.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cw.lnxyls.cn

[R19] 数组长度
来源：http://dn.hahajie.cn

echo "${#arr[@]}"
来源：http://ey.huanxung.cn

[R20] 关联数组（字典）
来源：http://rk.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uv.shxzskj.cn

[R21] 字符串长度
来源：http://xp.jianghongdianzi.cn

echo "${#s}"
来源：http://oq.newstarts.cn

[R22] 截取子串
来源：http://qf.shxzskj.cn

echo "${s:0:5}"
来源：http://rq.huanxung.cn

[R23] 字符串替换
来源：http://yo.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ps.chemitech.net.cn

[R24] 大小写转换
来源：http://qm.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mi.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://xq.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ul.wgjwhj.cn

[R26] 命令替换
来源：http://kp.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://ka.szxytkj.cn

[R27] 算术展开
来源：http://fg.newstarts.cn

echo $((1 + 2 * 3))
来源：http://ey.colortex.cn

[R28] 浮点运算
来源：http://hn.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://in.shxzukj.cn

[R29] 定义函数
来源：http://ln.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nh.szxytkj.cn

[R30] 函数返回状态码
来源：http://mk.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://kc.jianghongdianzi.cn

[R31] 局部变量
来源：http://sm.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://dw.bjjhwx.cn

[R32] 参数个数校验
来源：http://gy.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yj.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://tc.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jn.shtwfgs.cn

[R34] 退出时清理
来源：http://ov.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://py.chemitech.net.cn

[R35] 后台执行并等待
来源：http://fu.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lg.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://yt.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ht.asd995.cn

[R37] 把输出赋给变量
来源：http://jb.9csxet.cn

files=$(ls -1)
来源：http://sx.yuexingan06.cn

[R38] 管道串联
来源：http://oh.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://bo.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://en.huanxung.cn

cmd > out.log 2>&1
来源：http://qf.huanxung.cn

[R40] 追加写日志
来源：http://je.panjiajie.cn

echo "log" >> out.log
来源：http://jf.panjiajie.cn

[R41] 丢弃输出
来源：http://uw.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://gp.szxytkj.cn

[R42] 输入重定向
来源：http://gr.nicolike.cn

wc -l < a.txt
来源：http://mx.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://uq.yuexingan06.cn

find . -name "*.log" -type f
来源：http://db.9csxet.cn

[R44] 按修改时间查找
来源：http://ob.colortex.cn

find . -mtime -7 -type f
来源：http://hs.szsharing.cn

[R45] 批量删除
来源：http://tb.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://zj.asd995.cn

[R46] 递归替换文件内容
来源：http://wu.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xu.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://nv.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pb.szsharing.cn

[R48] awk 取指定列
来源：http://tu.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://qc.chemitech.net.cn

[R49] awk 带条件
来源：http://ql.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fn.nszjky.cn

[R50] awk 求和
来源：http://ni.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kr.9csxet.cn

[R51] 排序去重取前几
来源：http://oz.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fb.hnjuh.cn

[R52] 统计行数
来源：http://qd.haigaiapp.cn

wc -l a.txt
来源：http://zd.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://pa.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ob.9csxet.cn

[R54] 比较两个文件
来源：http://ww.yuexingan06.cn

diff a.txt b.txt
来源：http://ud.gzmigu.cn

[R55] 压缩与解压
来源：http://cd.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tm.yuexingan06.cn

[R56] 远程拷贝
来源：http://hw.asd995.cn

scp file user@host:/path/
来源：http://kh.szsharing.cn

[R57] 远程执行命令
来源：http://br.nicolike.cn

ssh user@host 'uptime'
来源：http://ew.gzmigu.cn

[R58] 下载文件
来源：http://vr.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ay.lnxyls.cn

[R59] 发 POST JSON
来源：http://lc.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ff.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://gp.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ac.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://ot.lnxyls.cn

df -h;  du -sh *
来源：http://xk.hahajie.cn

[R62] 找最占空间的文件
来源：http://ma.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://dc.nicolike.cn

[R63] 内存与进程
来源：http://uu.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://hr.jctech888.com.cn

[R64] 结束进程
来源：http://eo.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://ez.hahajie.cn

[R65] 查看端口占用
来源：http://cy.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ar.shtwfgs.cn

[R66] 定时任务
来源：http://ad.9csxet.cn

crontab -e;  crontab -l
来源：http://ky.szsharing.cn

[R67] 生成随机十六进制串
来源：http://hc.yuntaijiaju.cn

openssl rand -hex 16
来源：http://as.hahajie.cn

[R68] 计算文件校验值
来源：http://ns.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://za.wgjwhj.cn

[R69] 生成随机密码
来源：http://ds.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://qf.521024.cn

[R70] 时间戳与互转
来源：http://bo.521024.cn

date +%s;  date -d @1700000000
来源：http://gv.shxzukj.cn

[R71] 日期格式化
来源：http://tc.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zx.9csxet.cn

[R72] 等待端口就绪
来源：http://dw.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wv.yuexingan06.cn

[R73] 分割大日志
来源：http://xu.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://wh.bookmarksfly.cn

[R74] 批量重命名
来源：http://gd.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yb.szsharing.cn

[R75] 导出环境变量
来源：http://vl.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://rk.shtwfgs.cn

[R76] 使用临时文件
来源：http://kf.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jl.bookmarksfly.cn

[R77] 读取用户输入
来源：http://qd.shxzukj.cn

read -rp "请输入: " ans
来源：http://bv.bookmarksfly.cn

[R78] 交互式菜单
来源：http://dh.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://in.nszjky.cn

[R79] 解析命令行选项
来源：http://ge.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zt.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://xb.newstarts.cn

time ./run.sh
来源：http://yg.jianghongdianzi.cn

================================================================================
来源：http://ni.colortex.cn

S. C / C++ 专题
来源：http://bj.yuntaijiaju.cn

================================================================================
来源：http://mo.shxzukj.cn

[S01] C：Hello World
来源：http://bc.panjiajie.cn

#include <stdio.h>
来源：http://we.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fc.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://fg.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://pa.hnjuh.cn

[S03] C：读入整数
来源：http://em.huanxung.cn

int x; scanf("%d", &x);
来源：http://rt.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://cd.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rj.newstarts.cn

[S05] C：字符串长度
来源：http://zj.hahajie.cn

strlen(s)
来源：http://fg.wgjwhj.cn

[S06] C：字符串比较
来源：http://sb.jctech888.com.cn

strcmp(a, b) == 0
来源：http://ho.521024.cn

[S07] C：数组遍历求和
来源：http://bu.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mr.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://wh.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cg.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://mj.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dl.gzmigu.cn

[S10] C：指针与解引用
来源：http://uf.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://wr.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://gw.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://io.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nw.asd995.cn

fclose(f);
来源：http://rd.9csxet.cn

[S12] C：写文件
来源：http://hw.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ds.asd995.cn

[S13] C：宏定义
来源：http://hj.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eq.szsharing.cn

[S14] C：枚举
来源：http://up.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://bg.lnxyls.cn

[S15] C：类型转换
来源：http://rr.jctech888.com.cn

(double) a / b
来源：http://xr.hahajie.cn

[S16] C：位操作置位
来源：http://fw.bookmarksfly.cn

x |= (1 << 3);
来源：http://er.521024.cn

[S17] C：安全拼接字符串
来源：http://ch.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hd.wgjwhj.cn

[S18] C：命令行参数
来源：http://od.szxytkj.cn

int main(int argc, char **argv)
来源：http://hl.yuexingan06.cn

[S19] C：快速排序
来源：http://xe.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zb.yuntaijiaju.cn

[S20] C：二分查找
来源：http://jn.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://om.shtwfgs.cn

[S21] C：字符类别判断
来源：http://em.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tb.nicolike.cn

[S22] C：字符串转数字
来源：http://ga.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ez.haigaiapp.cn

[S23] C：随机数
来源：http://jc.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ke.wgjwhj.cn

[S24] C：获取本地时间
来源：http://dt.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ve.shxzskj.cn

[S25] C：内存拷贝
来源：http://nx.chemitech.net.cn

memcpy(dst, src, n);
来源：http://ew.gzmigu.cn

[S26] C：内存清零
来源：http://iv.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://xo.lnxyls.cn

[S27] C：定义常量
来源：http://ku.huanxung.cn

const double PI = 3.14159;
来源：http://cj.newstarts.cn

[S28] C：静态变量
来源：http://zm.haigaiapp.cn

static int counter = 0;
来源：http://xa.nszjky.cn

[S29] C：变参函数
来源：http://xj.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tb.yuexingan06.cn

[S30] C：头文件保护
来源：http://py.huanxung.cn

#ifndef X_H
来源：http://pj.asd995.cn

#define X_H
来源：http://nd.jianghongdianzi.cn

#endif
来源：http://hf.bookmarksfly.cn

[S31] C++：Hello World
来源：http://us.shxzskj.cn

#include <iostream>
来源：http://cj.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://kx.9csxet.cn

[S32] C++：字符串
来源：http://or.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://il.nszjky.cn

[S33] C++：vector 增删
来源：http://ug.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kn.newstarts.cn

[S34] C++：遍历 vector
来源：http://xa.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://eb.yuexingan06.cn

[S35] C++：map
来源：http://lc.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pf.szsharing.cn

[S36] C++：unordered_map
来源：http://gy.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gl.szxytkj.cn

[S37] C++：set
来源：http://hc.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eq.jianghongdianzi.cn

[S38] C++：排序
来源：http://wy.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://nf.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://cd.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sy.521024.cn

[S40] C++：查找元素
来源：http://dj.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://px.hnjuh.cn

[S41] C++：类与构造函数
来源：http://tp.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tn.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://sg.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://ud.muxihuayi.cn

[S43] C++：智能指针
来源：http://ni.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://rv.yuexingan06.cn

[S44] C++：引用传参
来源：http://ab.nszjky.cn

void inc(int &x) { ++x; }
来源：http://yj.bookmarksfly.cn

[S45] C++：lambda
来源：http://wi.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://he.jctech888.com.cn

[S46] C++：函数模板
来源：http://dq.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zo.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://py.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://al.szxytkj.cn

[S48] C++：逐行读文件
来源：http://wl.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dv.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://ti.haigaiapp.cn

[S49] C++：写文件
来源：http://ss.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://av.shxzukj.cn

[S50] C++：格式化数字
来源：http://fl.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cl.asd995.cn

[S51] C++：显式类型转换
来源：http://ib.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://vy.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://qh.newstarts.cn

int size() const noexcept { return n_; }
来源：http://qv.jctech888.com.cn

[S53] C++：移动语义
来源：http://gb.colortex.cn

std::vector<int> w = std::move(v);
来源：http://ho.hahajie.cn

[S54] C++：异常处理
来源：http://qk.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dy.gzmigu.cn

[S55] C++：结构化绑定
来源：http://ws.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zq.haigaiapp.cn

[S56] C++：optional
来源：http://tp.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tl.yuexingan06.cn

[S57] C++：编译期常量
来源：http://yj.szsharing.cn

constexpr int N = 10;
来源：http://uu.haigaiapp.cn

[S58] C++：命名空间
来源：http://po.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://qx.szxytkj.cn

[S59] C++：静态断言
来源：http://wy.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kt.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://wl.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://io.shtwfgs.cn

================================================================================
来源：http://qt.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://md.muxihuayi.cn

================================================================================
来源：http://xj.asd995.cn

[T01] Kotlin：Hello World
来源：http://fe.huanxung.cn

println("Hello")
来源：http://ho.huanxung.cn

[T02] Kotlin：变量
来源：http://sv.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gc.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://cq.haigaiapp.cn

"值: $b"
来源：http://lq.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://pz.lnxyls.cn

val n: String? = null;  n?.length
来源：http://xh.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://yk.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xo.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://ig.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ke.shxzukj.cn


<!-- 参考信息 -->