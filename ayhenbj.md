代发 wailian999

name="${1:-default}"
来源：http://ij.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://hx.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yp.hahajie.cn

[R07] if 判断文件
来源：http://xq.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dt.wgjwhj.cn

[R08] 数值比较
来源：http://vy.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lv.panjiajie.cn

[R09] 字符串比较
来源：http://ur.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vu.hahajie.cn

[R10] 正则匹配
来源：http://vw.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eo.nicolike.cn

[R11] case 多分支
来源：http://ig.hahajie.cn

case "$1" in
来源：http://pl.hnjuh.cn

start) echo "启动" ;;
来源：http://yj.gzmigu.cn

stop)  echo "停止" ;;
来源：http://ej.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://mo.gzmigu.cn

esac
来源：http://ji.yuexingan06.cn

[R12] for 遍历文件
来源：http://io.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://lu.bjjhwx.cn

[R13] for 计数循环
来源：http://cr.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://za.szxytkj.cn

[R14] C 风格 for
来源：http://fy.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mc.hnjuh.cn

[R15] while 逐行读文件
来源：http://zv.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://os.huixiangedu.cn

[R16] until 等待条件
来源：http://cc.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jg.haigaiapp.cn

[R17] 数组定义与取值
来源：http://jl.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qn.bjjhwx.cn

[R18] 遍历数组
来源：http://lk.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sp.huanxung.cn

[R19] 数组长度
来源：http://ya.muxihuayi.cn

echo "${#arr[@]}"
来源：http://jq.shxzskj.cn

[R20] 关联数组（字典）
来源：http://jp.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://de.panjiajie.cn

[R21] 字符串长度
来源：http://us.yuntaijiaju.cn

echo "${#s}"
来源：http://ms.shtwfgs.cn

[R22] 截取子串
来源：http://du.hahajie.cn

echo "${s:0:5}"
来源：http://ad.521024.cn

[R23] 字符串替换
来源：http://de.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ox.wgjwhj.cn

[R24] 大小写转换
来源：http://qe.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jr.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://zz.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://id.muxihuayi.cn

[R26] 命令替换
来源：http://rc.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://tn.jianghongdianzi.cn

[R27] 算术展开
来源：http://bh.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://gk.wgjwhj.cn

[R28] 浮点运算
来源：http://ok.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://rs.gzmigu.cn

[R29] 定义函数
来源：http://ys.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uv.muxihuayi.cn

[R30] 函数返回状态码
来源：http://de.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://lh.szsharing.cn

[R31] 局部变量
来源：http://bg.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://rq.jctech888.com.cn

[R32] 参数个数校验
来源：http://qo.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://li.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://nm.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://id.huanxung.cn

[R34] 退出时清理
来源：http://dk.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dk.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://im.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vf.shxzskj.cn

[R36] 并发执行多个任务
来源：http://qb.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xc.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://ma.9csxet.cn

files=$(ls -1)
来源：http://jd.muxihuayi.cn

[R38] 管道串联
来源：http://xz.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://tz.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://yp.huanxung.cn

cmd > out.log 2>&1
来源：http://ho.huixinmuqiang.cn

[R40] 追加写日志
来源：http://pd.yuntaijiaju.cn

echo "log" >> out.log
来源：http://rg.chemitech.net.cn

[R41] 丢弃输出
来源：http://ty.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://ac.bjjhwx.cn

[R42] 输入重定向
来源：http://np.yuntaijiaju.cn

wc -l < a.txt
来源：http://gc.panjiajie.cn

[R43] 按名字查找文件
来源：http://td.nicolike.cn

find . -name "*.log" -type f
来源：http://xv.jctech888.com.cn

[R44] 按修改时间查找
来源：http://ic.9csxet.cn

find . -mtime -7 -type f
来源：http://jw.huanxung.cn

[R45] 批量删除
来源：http://az.9csxet.cn

find . -name "*.tmp" -delete
来源：http://an.nszjky.cn

[R46] 递归替换文件内容
来源：http://fx.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xi.muxihuayi.cn

[R47] sed 单行替换
来源：http://th.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nb.yuexingan06.cn

[R48] awk 取指定列
来源：http://sh.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://sn.yuexingan06.cn

[R49] awk 带条件
来源：http://qi.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xm.chemitech.net.cn

[R50] awk 求和
来源：http://zy.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gk.panjiajie.cn

[R51] 排序去重取前几
来源：http://hp.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://va.huanxung.cn

[R52] 统计行数
来源：http://ag.huixiangedu.cn

wc -l a.txt
来源：http://so.521024.cn

[R53] 查看文件头与实时尾
来源：http://ir.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bx.hahajie.cn

[R54] 比较两个文件
来源：http://lx.haigaiapp.cn

diff a.txt b.txt
来源：http://ox.gzmigu.cn

[R55] 压缩与解压
来源：http://jf.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mu.szxytkj.cn

[R56] 远程拷贝
来源：http://lr.chemitech.net.cn

scp file user@host:/path/
来源：http://me.jctech888.com.cn

[R57] 远程执行命令
来源：http://ez.szxytkj.cn

ssh user@host 'uptime'
来源：http://si.huanxung.cn

[R58] 下载文件
来源：http://pc.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jb.jctech888.com.cn

[R59] 发 POST JSON
来源：http://eu.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yo.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://wg.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lf.jctech888.com.cn

[R61] 磁盘占用
来源：http://dd.newstarts.cn

df -h;  du -sh *
来源：http://rg.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://bi.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://sc.colortex.cn

[R63] 内存与进程
来源：http://id.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://lp.yuntaijiaju.cn

[R64] 结束进程
来源：http://nu.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://zh.haigaiapp.cn

[R65] 查看端口占用
来源：http://wj.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://om.colortex.cn

[R66] 定时任务
来源：http://ia.shxzukj.cn

crontab -e;  crontab -l
来源：http://sa.huanxung.cn

[R67] 生成随机十六进制串
来源：http://kc.huanxung.cn

openssl rand -hex 16
来源：http://fy.panjiajie.cn

[R68] 计算文件校验值
来源：http://us.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ud.asd995.cn

[R69] 生成随机密码
来源：http://mg.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://ut.newstarts.cn

[R70] 时间戳与互转
来源：http://cm.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://iq.asd995.cn

[R71] 日期格式化
来源：http://rc.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ca.nicolike.cn

[R72] 等待端口就绪
来源：http://ea.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gp.nicolike.cn

[R73] 分割大日志
来源：http://kd.shtwfgs.cn

split -l 1000 big.log part_
来源：http://ag.hahajie.cn

[R74] 批量重命名
来源：http://pb.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dw.jctech888.com.cn

[R75] 导出环境变量
来源：http://vl.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://gb.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://ro.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ut.yuexingan06.cn

[R77] 读取用户输入
来源：http://tk.521024.cn

read -rp "请输入: " ans
来源：http://vx.lnxyls.cn

[R78] 交互式菜单
来源：http://lx.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ie.wgjwhj.cn

[R79] 解析命令行选项
来源：http://fz.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://or.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://gu.asd995.cn

time ./run.sh
来源：http://yv.bjjhwx.cn

================================================================================
来源：http://wf.wgjwhj.cn

S. C / C++ 专题
来源：http://yr.huixiangedu.cn

================================================================================
来源：http://es.gzmigu.cn

[S01] C：Hello World
来源：http://cg.colortex.cn

#include <stdio.h>
来源：http://ak.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ot.huanxung.cn

[S02] C：变量与格式化输出
来源：http://tj.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://oy.huanxung.cn

[S03] C：读入整数
来源：http://mt.panjiajie.cn

int x; scanf("%d", &x);
来源：http://dz.gzmigu.cn

[S04] C：字符串复制
来源：http://cc.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ab.hnjuh.cn

[S05] C：字符串长度
来源：http://jx.yuntaijiaju.cn

strlen(s)
来源：http://go.asd995.cn

[S06] C：字符串比较
来源：http://qy.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://oi.shxzukj.cn

[S07] C：数组遍历求和
来源：http://tg.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pm.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://dy.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cw.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://zk.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vk.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://ml.newstarts.cn

int *p = &a;  *p = 5;
来源：http://gj.gzmigu.cn

[S11] C：逐行读文件
来源：http://zp.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://di.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pk.muxihuayi.cn

fclose(f);
来源：http://uh.yuexingan06.cn

[S12] C：写文件
来源：http://me.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pc.9csxet.cn

[S13] C：宏定义
来源：http://jm.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pa.szxytkj.cn

[S14] C：枚举
来源：http://uo.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://ll.nicolike.cn

[S15] C：类型转换
来源：http://ez.yuexingan06.cn

(double) a / b
来源：http://pr.lnxyls.cn

[S16] C：位操作置位
来源：http://dv.hnjuh.cn

x |= (1 << 3);
来源：http://ss.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://qa.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://or.wgjwhj.cn

[S18] C：命令行参数
来源：http://hk.haigaiapp.cn

int main(int argc, char **argv)
来源：http://al.panjiajie.cn

[S19] C：快速排序
来源：http://pm.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fv.panjiajie.cn

[S20] C：二分查找
来源：http://sl.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bp.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://yg.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vc.newstarts.cn

[S22] C：字符串转数字
来源：http://kk.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tt.szxytkj.cn

[S23] C：随机数
来源：http://kw.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qv.asd995.cn

[S24] C：获取本地时间
来源：http://up.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dl.haigaiapp.cn

[S25] C：内存拷贝
来源：http://rf.jctech888.com.cn

memcpy(dst, src, n);
来源：http://qb.muxihuayi.cn

[S26] C：内存清零
来源：http://or.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://ux.9csxet.cn

[S27] C：定义常量
来源：http://ty.hnjuh.cn

const double PI = 3.14159;
来源：http://xr.hahajie.cn

[S28] C：静态变量
来源：http://vz.bjjhwx.cn

static int counter = 0;
来源：http://nd.lnxyls.cn

[S29] C：变参函数
来源：http://xk.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fg.9csxet.cn

[S30] C：头文件保护
来源：http://vv.shxzukj.cn

#ifndef X_H
来源：http://xm.colortex.cn

#define X_H
来源：http://ls.wgjwhj.cn

#endif
来源：http://wk.shtwfgs.cn

[S31] C++：Hello World
来源：http://dj.huanxung.cn

#include <iostream>
来源：http://tn.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://ij.shxzskj.cn

[S32] C++：字符串
来源：http://gk.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://ho.panjiajie.cn

[S33] C++：vector 增删
来源：http://ne.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ts.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://ur.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://ud.shxzukj.cn

[S35] C++：map
来源：http://oz.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fy.chemitech.net.cn

[S36] C++：unordered_map
来源：http://ln.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ss.yuexingan06.cn

[S37] C++：set
来源：http://au.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oi.wgjwhj.cn

[S38] C++：排序
来源：http://kj.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://ms.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://yc.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pt.nicolike.cn

[S40] C++：查找元素
来源：http://cr.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ei.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://au.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cs.newstarts.cn

[S42] C++：继承与虚函数
来源：http://od.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://tk.yuexingan06.cn

[S43] C++：智能指针
来源：http://af.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://gc.nszjky.cn

[S44] C++：引用传参
来源：http://ne.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://vy.huixiangedu.cn

[S45] C++：lambda
来源：http://ga.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wg.newstarts.cn

[S46] C++：函数模板
来源：http://nb.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wm.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://ag.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rd.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://jy.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nq.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://cv.nicolike.cn

[S49] C++：写文件
来源：http://ab.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fw.chemitech.net.cn

[S50] C++：格式化数字
来源：http://aq.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kc.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://pe.chemitech.net.cn

static_cast<double>(a) / b
来源：http://cc.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://il.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://bf.hahajie.cn

[S53] C++：移动语义
来源：http://ay.colortex.cn

std::vector<int> w = std::move(v);
来源：http://zn.gzmigu.cn

[S54] C++：异常处理
来源：http://cl.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mv.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://mh.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bx.jianghongdianzi.cn

[S56] C++：optional
来源：http://ls.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sk.newstarts.cn

[S57] C++：编译期常量
来源：http://ej.newstarts.cn

constexpr int N = 10;
来源：http://gu.nicolike.cn

[S58] C++：命名空间
来源：http://bm.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://en.hnjuh.cn

[S59] C++：静态断言
来源：http://vv.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sr.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://en.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pj.yuntaijiaju.cn

================================================================================
来源：http://ho.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iy.chemitech.net.cn

================================================================================
来源：http://hp.hahajie.cn

[T01] Kotlin：Hello World
来源：http://xk.jctech888.com.cn

println("Hello")
来源：http://ga.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://ow.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wy.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://gw.chemitech.net.cn

"值: $b"
来源：http://fy.9csxet.cn

[T04] Kotlin：空安全
来源：http://gt.nicolike.cn

val n: String? = null;  n?.length
来源：http://ix.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://ep.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lu.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://rp.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bc.shxzskj.cn


<!-- 参考信息 -->