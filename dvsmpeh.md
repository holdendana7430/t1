代发 wailian999

name="${1:-default}"
来源：http://ny.9csxet.cn

[R06] 判断命令是否存在
来源：http://kn.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fm.muxihuayi.cn

[R07] if 判断文件
来源：http://dj.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://if.yuntaijiaju.cn

[R08] 数值比较
来源：http://je.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xk.muxihuayi.cn

[R09] 字符串比较
来源：http://dp.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sx.huixiangedu.cn

[R10] 正则匹配
来源：http://ck.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jn.shxzskj.cn

[R11] case 多分支
来源：http://jv.szxytkj.cn

case "$1" in
来源：http://kz.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://we.lnxyls.cn

stop)  echo "停止" ;;
来源：http://on.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://hm.521024.cn

esac
来源：http://wn.panjiajie.cn

[R12] for 遍历文件
来源：http://kn.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://yo.jianghongdianzi.cn

[R13] for 计数循环
来源：http://ol.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://zo.huixinmuqiang.cn

[R14] C 风格 for
来源：http://yx.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uy.colortex.cn

[R15] while 逐行读文件
来源：http://wy.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dw.hahajie.cn

[R16] until 等待条件
来源：http://kh.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nj.szxytkj.cn

[R17] 数组定义与取值
来源：http://nz.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tc.huixiangedu.cn

[R18] 遍历数组
来源：http://tq.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lg.gzmigu.cn

[R19] 数组长度
来源：http://bk.colortex.cn

echo "${#arr[@]}"
来源：http://fs.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://yi.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tk.huixinmuqiang.cn

[R21] 字符串长度
来源：http://ae.jianghongdianzi.cn

echo "${#s}"
来源：http://bf.hahajie.cn

[R22] 截取子串
来源：http://tf.szxytkj.cn

echo "${s:0:5}"
来源：http://cg.hahajie.cn

[R23] 字符串替换
来源：http://zx.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yp.chemitech.net.cn

[R24] 大小写转换
来源：http://xq.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wq.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://fj.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ng.panjiajie.cn

[R26] 命令替换
来源：http://ku.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://tn.hahajie.cn

[R27] 算术展开
来源：http://ib.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://jf.lnxyls.cn

[R28] 浮点运算
来源：http://ho.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://pp.shxzukj.cn

[R29] 定义函数
来源：http://tl.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dx.szsharing.cn

[R30] 函数返回状态码
来源：http://im.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://ij.bookmarksfly.cn

[R31] 局部变量
来源：http://fi.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://av.bookmarksfly.cn

[R32] 参数个数校验
来源：http://hk.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://va.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://eo.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mb.bookmarksfly.cn

[R34] 退出时清理
来源：http://es.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kv.521024.cn

[R35] 后台执行并等待
来源：http://ze.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wn.9csxet.cn

[R36] 并发执行多个任务
来源：http://nh.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uy.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://wb.colortex.cn

files=$(ls -1)
来源：http://jh.wgjwhj.cn

[R38] 管道串联
来源：http://bg.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://th.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://gl.shtwfgs.cn

cmd > out.log 2>&1
来源：http://ys.lnxyls.cn

[R40] 追加写日志
来源：http://vt.shxzskj.cn

echo "log" >> out.log
来源：http://ij.hahajie.cn

[R41] 丢弃输出
来源：http://no.521024.cn

cmd >/dev/null 2>&1
来源：http://sv.9csxet.cn

[R42] 输入重定向
来源：http://zo.szxytkj.cn

wc -l < a.txt
来源：http://bw.hahajie.cn

[R43] 按名字查找文件
来源：http://bs.nicolike.cn

find . -name "*.log" -type f
来源：http://gc.newstarts.cn

[R44] 按修改时间查找
来源：http://xo.nicolike.cn

find . -mtime -7 -type f
来源：http://mo.muxihuayi.cn

[R45] 批量删除
来源：http://xu.szsharing.cn

find . -name "*.tmp" -delete
来源：http://tj.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://ku.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fp.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://db.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kp.wgjwhj.cn

[R48] awk 取指定列
来源：http://hg.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://re.huanxung.cn

[R49] awk 带条件
来源：http://sx.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xb.lnxyls.cn

[R50] awk 求和
来源：http://fb.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yb.newstarts.cn

[R51] 排序去重取前几
来源：http://de.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://od.shxzukj.cn

[R52] 统计行数
来源：http://nm.yuntaijiaju.cn

wc -l a.txt
来源：http://kz.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://id.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ad.gzmigu.cn

[R54] 比较两个文件
来源：http://dd.yuexingan06.cn

diff a.txt b.txt
来源：http://cy.muxihuayi.cn

[R55] 压缩与解压
来源：http://mh.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://js.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ri.shxzskj.cn

scp file user@host:/path/
来源：http://ur.jctech888.com.cn

[R57] 远程执行命令
来源：http://mv.hahajie.cn

ssh user@host 'uptime'
来源：http://ar.shtwfgs.cn

[R58] 下载文件
来源：http://sh.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bp.shxzukj.cn

[R59] 发 POST JSON
来源：http://cf.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yu.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://me.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wo.shtwfgs.cn

[R61] 磁盘占用
来源：http://ad.gzmigu.cn

df -h;  du -sh *
来源：http://hz.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://oi.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://vr.shxzukj.cn

[R63] 内存与进程
来源：http://vp.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://xe.jctech888.com.cn

[R64] 结束进程
来源：http://ts.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://sm.asd995.cn

[R65] 查看端口占用
来源：http://ft.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nk.nicolike.cn

[R66] 定时任务
来源：http://nt.asd995.cn

crontab -e;  crontab -l
来源：http://cm.9csxet.cn

[R67] 生成随机十六进制串
来源：http://sx.yuntaijiaju.cn

openssl rand -hex 16
来源：http://zo.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://td.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ze.chemitech.net.cn

[R69] 生成随机密码
来源：http://na.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://cq.shtwfgs.cn

[R70] 时间戳与互转
来源：http://yo.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://ky.yuexingan06.cn

[R71] 日期格式化
来源：http://zz.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jt.szxytkj.cn

[R72] 等待端口就绪
来源：http://hr.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://el.hahajie.cn

[R73] 分割大日志
来源：http://ha.shxzskj.cn

split -l 1000 big.log part_
来源：http://xa.colortex.cn

[R74] 批量重命名
来源：http://mo.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cf.haigaiapp.cn

[R75] 导出环境变量
来源：http://lj.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://ol.szxytkj.cn

[R76] 使用临时文件
来源：http://pv.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://nv.colortex.cn

read -rp "请输入: " ans
来源：http://rj.jctech888.com.cn

[R78] 交互式菜单
来源：http://ur.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://au.newstarts.cn

[R79] 解析命令行选项
来源：http://bx.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yp.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://gc.shxzskj.cn

time ./run.sh
来源：http://gm.hnjuh.cn

================================================================================
来源：http://dg.szxytkj.cn

S. C / C++ 专题
来源：http://cp.nicolike.cn

================================================================================
来源：http://cq.521024.cn

[S01] C：Hello World
来源：http://fz.huanxung.cn

#include <stdio.h>
来源：http://ec.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jo.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://je.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://ts.huanxung.cn

[S03] C：读入整数
来源：http://pf.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://mg.wgjwhj.cn

[S04] C：字符串复制
来源：http://cl.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lz.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://gw.shxzukj.cn

strlen(s)
来源：http://in.haigaiapp.cn

[S06] C：字符串比较
来源：http://pr.panjiajie.cn

strcmp(a, b) == 0
来源：http://na.9csxet.cn

[S07] C：数组遍历求和
来源：http://ac.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ww.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://gx.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fb.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://af.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uo.newstarts.cn

[S10] C：指针与解引用
来源：http://ty.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://un.hnjuh.cn

[S11] C：逐行读文件
来源：http://jz.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://lo.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kn.shtwfgs.cn

fclose(f);
来源：http://ad.hahajie.cn

[S12] C：写文件
来源：http://na.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ld.nicolike.cn

[S13] C：宏定义
来源：http://gt.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uz.jctech888.com.cn

[S14] C：枚举
来源：http://qz.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://jq.asd995.cn

[S15] C：类型转换
来源：http://yd.shtwfgs.cn

(double) a / b
来源：http://hq.bookmarksfly.cn

[S16] C：位操作置位
来源：http://xh.panjiajie.cn

x |= (1 << 3);
来源：http://tw.asd995.cn

[S17] C：安全拼接字符串
来源：http://tk.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oz.chemitech.net.cn

[S18] C：命令行参数
来源：http://np.wgjwhj.cn

int main(int argc, char **argv)
来源：http://as.szsharing.cn

[S19] C：快速排序
来源：http://mm.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vc.521024.cn

[S20] C：二分查找
来源：http://sq.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ox.colortex.cn

[S21] C：字符类别判断
来源：http://ob.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bg.hahajie.cn

[S22] C：字符串转数字
来源：http://rq.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://th.lnxyls.cn

[S23] C：随机数
来源：http://oj.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dc.shtwfgs.cn

[S24] C：获取本地时间
来源：http://px.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://px.asd995.cn

[S25] C：内存拷贝
来源：http://pq.huixiangedu.cn

memcpy(dst, src, n);
来源：http://yp.yuntaijiaju.cn

[S26] C：内存清零
来源：http://gd.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://ff.colortex.cn

[S27] C：定义常量
来源：http://bf.hnjuh.cn

const double PI = 3.14159;
来源：http://un.huixiangedu.cn

[S28] C：静态变量
来源：http://zt.yuexingan06.cn

static int counter = 0;
来源：http://fi.huanxung.cn

[S29] C：变参函数
来源：http://xd.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ke.chemitech.net.cn

[S30] C：头文件保护
来源：http://hr.yuntaijiaju.cn

#ifndef X_H
来源：http://pj.haigaiapp.cn

#define X_H
来源：http://qg.gzmigu.cn

#endif
来源：http://yv.szsharing.cn

[S31] C++：Hello World
来源：http://yj.shtwfgs.cn

#include <iostream>
来源：http://pt.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://sy.chemitech.net.cn

[S32] C++：字符串
来源：http://bw.colortex.cn

std::string s = "hi";  s += "!";
来源：http://gf.panjiajie.cn

[S33] C++：vector 增删
来源：http://op.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ee.nicolike.cn

[S34] C++：遍历 vector
来源：http://hp.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://aa.huanxung.cn

[S35] C++：map
来源：http://yr.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gv.haigaiapp.cn

[S36] C++：unordered_map
来源：http://mv.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bd.huixiangedu.cn

[S37] C++：set
来源：http://dr.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ww.9csxet.cn

[S38] C++：排序
来源：http://ng.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://gn.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://bo.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jj.panjiajie.cn

[S40] C++：查找元素
来源：http://ve.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eu.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://lt.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yf.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://eh.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://nl.nicolike.cn

[S43] C++：智能指针
来源：http://ij.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://me.colortex.cn

[S44] C++：引用传参
来源：http://gz.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://bq.colortex.cn

[S45] C++：lambda
来源：http://gi.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dr.9csxet.cn

[S46] C++：函数模板
来源：http://py.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rs.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://cj.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rg.newstarts.cn

[S48] C++：逐行读文件
来源：http://pr.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kk.asd995.cn

while (std::getline(in, line)) { }
来源：http://mo.szsharing.cn

[S49] C++：写文件
来源：http://fi.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://za.nszjky.cn

[S50] C++：格式化数字
来源：http://zp.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ah.szsharing.cn

[S51] C++：显式类型转换
来源：http://zv.shxzskj.cn

static_cast<double>(a) / b
来源：http://pc.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://bh.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://vm.colortex.cn

[S53] C++：移动语义
来源：http://if.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://pt.yuexingan06.cn

[S54] C++：异常处理
来源：http://nh.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ci.szxytkj.cn

[S55] C++：结构化绑定
来源：http://dz.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wp.jianghongdianzi.cn

[S56] C++：optional
来源：http://rc.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://an.hnjuh.cn

[S57] C++：编译期常量
来源：http://xg.newstarts.cn

constexpr int N = 10;
来源：http://yu.521024.cn

[S58] C++：命名空间
来源：http://to.521024.cn

namespace ns { int f() { return 1; } }
来源：http://cp.gzmigu.cn

[S59] C++：静态断言
来源：http://fl.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yg.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://lw.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tt.huanxung.cn

================================================================================
来源：http://ej.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ug.shtwfgs.cn

================================================================================
来源：http://ac.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://zo.shxzskj.cn

println("Hello")
来源：http://ig.huixiangedu.cn

[T02] Kotlin：变量
来源：http://wn.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gd.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://fo.hahajie.cn

"值: $b"
来源：http://ue.nszjky.cn

[T04] Kotlin：空安全
来源：http://qv.hahajie.cn

val n: String? = null;  n?.length
来源：http://rb.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://or.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ms.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://to.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://is.panjiajie.cn


<!-- 参考信息 -->