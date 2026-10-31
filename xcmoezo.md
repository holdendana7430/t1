代发 wailian999

readonly PI=3.14
来源：http://tg.hahajie.cn

[R04] 位置参数
来源：http://lc.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qz.jctech888.com.cn

[R05] 参数默认值
来源：http://kz.jctech888.com.cn

name="${1:-default}"
来源：http://jd.huanxung.cn

[R06] 判断命令是否存在
来源：http://pz.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dc.9csxet.cn

[R07] if 判断文件
来源：http://qq.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ay.newstarts.cn

[R08] 数值比较
来源：http://qm.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cb.huanxung.cn

[R09] 字符串比较
来源：http://ep.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qj.chemitech.net.cn

[R10] 正则匹配
来源：http://ul.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fr.gzmigu.cn

[R11] case 多分支
来源：http://yy.hnjuh.cn

case "$1" in
来源：http://vr.newstarts.cn

start) echo "启动" ;;
来源：http://ay.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://ty.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://yh.chemitech.net.cn

esac
来源：http://nr.panjiajie.cn

[R12] for 遍历文件
来源：http://il.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://od.huixinmuqiang.cn

[R13] for 计数循环
来源：http://vd.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://hv.chemitech.net.cn

[R14] C 风格 for
来源：http://rf.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://li.newstarts.cn

[R15] while 逐行读文件
来源：http://af.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mp.yuntaijiaju.cn

[R16] until 等待条件
来源：http://oj.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xj.shxzskj.cn

[R17] 数组定义与取值
来源：http://nu.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tb.yuntaijiaju.cn

[R18] 遍历数组
来源：http://lu.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xc.gzmigu.cn

[R19] 数组长度
来源：http://mn.jctech888.com.cn

echo "${#arr[@]}"
来源：http://jw.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://yn.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pe.hahajie.cn

[R21] 字符串长度
来源：http://kf.nszjky.cn

echo "${#s}"
来源：http://ux.hahajie.cn

[R22] 截取子串
来源：http://vv.haigaiapp.cn

echo "${s:0:5}"
来源：http://kn.newstarts.cn

[R23] 字符串替换
来源：http://ql.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hg.shxzskj.cn

[R24] 大小写转换
来源：http://eu.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sr.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://ut.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fv.nszjky.cn

[R26] 命令替换
来源：http://fh.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://bw.9csxet.cn

[R27] 算术展开
来源：http://gn.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://ny.szxytkj.cn

[R28] 浮点运算
来源：http://dv.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://og.9csxet.cn

[R29] 定义函数
来源：http://lh.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sk.szsharing.cn

[R30] 函数返回状态码
来源：http://na.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://jv.shxzukj.cn

[R31] 局部变量
来源：http://xt.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://sr.haigaiapp.cn

[R32] 参数个数校验
来源：http://zi.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yw.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://up.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sh.9csxet.cn

[R34] 退出时清理
来源：http://bj.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gx.chemitech.net.cn

[R35] 后台执行并等待
来源：http://ej.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zl.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://ar.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ie.asd995.cn

[R37] 把输出赋给变量
来源：http://fh.haigaiapp.cn

files=$(ls -1)
来源：http://su.wgjwhj.cn

[R38] 管道串联
来源：http://du.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://bu.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://ou.wgjwhj.cn

cmd > out.log 2>&1
来源：http://ke.newstarts.cn

[R40] 追加写日志
来源：http://yl.nszjky.cn

echo "log" >> out.log
来源：http://bo.hahajie.cn

[R41] 丢弃输出
来源：http://qq.asd995.cn

cmd >/dev/null 2>&1
来源：http://ji.nicolike.cn

[R42] 输入重定向
来源：http://ev.lnxyls.cn

wc -l < a.txt
来源：http://dl.yuexingan06.cn

[R43] 按名字查找文件
来源：http://rl.shxzukj.cn

find . -name "*.log" -type f
来源：http://ms.jctech888.com.cn

[R44] 按修改时间查找
来源：http://xc.nszjky.cn

find . -mtime -7 -type f
来源：http://hy.muxihuayi.cn

[R45] 批量删除
来源：http://ju.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://qa.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://io.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zi.wgjwhj.cn

[R47] sed 单行替换
来源：http://wl.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ks.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://eu.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://zs.colortex.cn

[R49] awk 带条件
来源：http://pa.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bw.9csxet.cn

[R50] awk 求和
来源：http://ba.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jl.521024.cn

[R51] 排序去重取前几
来源：http://dx.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jv.yuntaijiaju.cn

[R52] 统计行数
来源：http://ek.muxihuayi.cn

wc -l a.txt
来源：http://ws.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://yr.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wj.szxytkj.cn

[R54] 比较两个文件
来源：http://ek.yuntaijiaju.cn

diff a.txt b.txt
来源：http://wl.jctech888.com.cn

[R55] 压缩与解压
来源：http://rv.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yt.muxihuayi.cn

[R56] 远程拷贝
来源：http://ed.newstarts.cn

scp file user@host:/path/
来源：http://ku.jctech888.com.cn

[R57] 远程执行命令
来源：http://mc.wgjwhj.cn

ssh user@host 'uptime'
来源：http://lf.nszjky.cn

[R58] 下载文件
来源：http://lz.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rq.lnxyls.cn

[R59] 发 POST JSON
来源：http://pn.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fi.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://xk.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rf.wgjwhj.cn

[R61] 磁盘占用
来源：http://tn.huixinmuqiang.cn

df -h;  du -sh *
来源：http://sb.colortex.cn

[R62] 找最占空间的文件
来源：http://qa.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://bn.newstarts.cn

[R63] 内存与进程
来源：http://wc.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://uo.panjiajie.cn

[R64] 结束进程
来源：http://hq.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://qu.bookmarksfly.cn

[R65] 查看端口占用
来源：http://hp.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jw.muxihuayi.cn

[R66] 定时任务
来源：http://cb.nszjky.cn

crontab -e;  crontab -l
来源：http://od.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://lm.9csxet.cn

openssl rand -hex 16
来源：http://ju.huanxung.cn

[R68] 计算文件校验值
来源：http://eu.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ir.521024.cn

[R69] 生成随机密码
来源：http://sg.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://hs.wgjwhj.cn

[R70] 时间戳与互转
来源：http://bi.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://zt.panjiajie.cn

[R71] 日期格式化
来源：http://pn.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mo.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://hz.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ea.colortex.cn

[R73] 分割大日志
来源：http://hr.huanxung.cn

split -l 1000 big.log part_
来源：http://ne.gzmigu.cn

[R74] 批量重命名
来源：http://sd.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rh.jctech888.com.cn

[R75] 导出环境变量
来源：http://hk.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://du.huixiangedu.cn

[R76] 使用临时文件
来源：http://wl.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gw.bookmarksfly.cn

[R77] 读取用户输入
来源：http://qh.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://he.newstarts.cn

[R78] 交互式菜单
来源：http://gv.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://io.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://qf.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zx.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://kf.9csxet.cn

time ./run.sh
来源：http://pr.yuexingan06.cn

================================================================================
来源：http://ol.nicolike.cn

S. C / C++ 专题
来源：http://vx.9csxet.cn

================================================================================
来源：http://mj.yuntaijiaju.cn

[S01] C：Hello World
来源：http://hr.yuntaijiaju.cn

#include <stdio.h>
来源：http://sq.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fw.nszjky.cn

[S02] C：变量与格式化输出
来源：http://pu.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://xl.huixiangedu.cn

[S03] C：读入整数
来源：http://as.asd995.cn

int x; scanf("%d", &x);
来源：http://rq.bookmarksfly.cn

[S04] C：字符串复制
来源：http://ut.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://td.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://dl.szsharing.cn

strlen(s)
来源：http://ts.bjjhwx.cn

[S06] C：字符串比较
来源：http://kv.chemitech.net.cn

strcmp(a, b) == 0
来源：http://ov.hahajie.cn

[S07] C：数组遍历求和
来源：http://zk.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ag.521024.cn

[S08] C：动态内存分配与释放
来源：http://yu.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pv.521024.cn

[S09] C：结构体定义与初始化
来源：http://ia.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fc.newstarts.cn

[S10] C：指针与解引用
来源：http://bs.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://wo.wgjwhj.cn

[S11] C：逐行读文件
来源：http://lj.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://em.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://px.yuntaijiaju.cn

fclose(f);
来源：http://th.yuntaijiaju.cn

[S12] C：写文件
来源：http://vv.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tb.shxzskj.cn

[S13] C：宏定义
来源：http://hu.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ue.hnjuh.cn

[S14] C：枚举
来源：http://cd.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://gi.hahajie.cn

[S15] C：类型转换
来源：http://hg.bookmarksfly.cn

(double) a / b
来源：http://oc.521024.cn

[S16] C：位操作置位
来源：http://bx.shxzukj.cn

x |= (1 << 3);
来源：http://tq.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://bl.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eg.muxihuayi.cn

[S18] C：命令行参数
来源：http://ey.muxihuayi.cn

int main(int argc, char **argv)
来源：http://bw.hahajie.cn

[S19] C：快速排序
来源：http://bb.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jo.nszjky.cn

[S20] C：二分查找
来源：http://ix.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nm.gzmigu.cn

[S21] C：字符类别判断
来源：http://pm.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fz.yuexingan06.cn

[S22] C：字符串转数字
来源：http://zr.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ce.jianghongdianzi.cn

[S23] C：随机数
来源：http://uv.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yd.chemitech.net.cn

[S24] C：获取本地时间
来源：http://ad.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bm.szxytkj.cn

[S25] C：内存拷贝
来源：http://qo.szsharing.cn

memcpy(dst, src, n);
来源：http://dn.shtwfgs.cn

[S26] C：内存清零
来源：http://gt.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://xv.chemitech.net.cn

[S27] C：定义常量
来源：http://gv.nszjky.cn

const double PI = 3.14159;
来源：http://ut.huixiangedu.cn

[S28] C：静态变量
来源：http://uz.wgjwhj.cn

static int counter = 0;
来源：http://cy.huixiangedu.cn

[S29] C：变参函数
来源：http://qs.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gz.haigaiapp.cn

[S30] C：头文件保护
来源：http://lx.bjjhwx.cn

#ifndef X_H
来源：http://er.shxzukj.cn

#define X_H
来源：http://fb.shxzskj.cn

#endif
来源：http://nc.shxzskj.cn

[S31] C++：Hello World
来源：http://pw.gzmigu.cn

#include <iostream>
来源：http://gg.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://tr.jianghongdianzi.cn

[S32] C++：字符串
来源：http://nu.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://nx.yuexingan06.cn

[S33] C++：vector 增删
来源：http://dq.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://os.gzmigu.cn

[S34] C++：遍历 vector
来源：http://kj.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://ey.bjjhwx.cn

[S35] C++：map
来源：http://oy.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nh.panjiajie.cn

[S36] C++：unordered_map
来源：http://xc.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ou.jianghongdianzi.cn

[S37] C++：set
来源：http://he.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fp.bjjhwx.cn

[S38] C++：排序
来源：http://tp.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://ph.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://yo.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vk.jctech888.com.cn

[S40] C++：查找元素
来源：http://od.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mq.newstarts.cn

[S41] C++：类与构造函数
来源：http://bc.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vj.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://yx.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://bk.hahajie.cn

[S43] C++：智能指针
来源：http://qp.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://sb.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://zo.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://tr.jctech888.com.cn

[S45] C++：lambda
来源：http://ur.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lo.wgjwhj.cn

[S46] C++：函数模板
来源：http://cy.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://il.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://kf.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bv.asd995.cn

[S48] C++：逐行读文件
来源：http://cx.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ds.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://pf.yuexingan06.cn

[S49] C++：写文件
来源：http://mh.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wa.gzmigu.cn

[S50] C++：格式化数字
来源：http://az.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://op.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://wd.asd995.cn

static_cast<double>(a) / b
来源：http://bu.colortex.cn

[S52] C++：const 与 noexcept
来源：http://dv.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://xa.szsharing.cn

[S53] C++：移动语义
来源：http://mv.521024.cn

std::vector<int> w = std::move(v);
来源：http://zz.shxzskj.cn

[S54] C++：异常处理
来源：http://sl.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kb.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://gs.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wm.yuexingan06.cn

[S56] C++：optional
来源：http://bs.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zk.panjiajie.cn

[S57] C++：编译期常量
来源：http://pi.jianghongdianzi.cn

constexpr int N = 10;
来源：http://po.huixiangedu.cn

[S58] C++：命名空间
来源：http://yg.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://lh.muxihuayi.cn

[S59] C++：静态断言
来源：http://ez.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ef.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://iw.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lq.asd995.cn

================================================================================
来源：http://dj.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zz.muxihuayi.cn

================================================================================
来源：http://sy.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://dt.lnxyls.cn

println("Hello")
来源：http://av.lnxyls.cn

[T02] Kotlin：变量
来源：http://xg.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ld.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://wx.szsharing.cn

"值: $b"
来源：http://fc.asd995.cn

[T04] Kotlin：空安全
来源：http://ep.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://pq.gzmigu.cn


<!-- 参考信息 -->