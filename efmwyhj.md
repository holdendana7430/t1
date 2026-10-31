代发 wailian999

readonly PI=3.14
来源：http://df.hahajie.cn

[R04] 位置参数
来源：http://bb.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bn.chemitech.net.cn

[R05] 参数默认值
来源：http://ju.nszjky.cn

name="${1:-default}"
来源：http://kl.szsharing.cn

[R06] 判断命令是否存在
来源：http://kk.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xk.bjjhwx.cn

[R07] if 判断文件
来源：http://sn.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kr.9csxet.cn

[R08] 数值比较
来源：http://vx.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://od.jianghongdianzi.cn

[R09] 字符串比较
来源：http://qd.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vu.huanxung.cn

[R10] 正则匹配
来源：http://bs.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rz.panjiajie.cn

[R11] case 多分支
来源：http://vy.521024.cn

case "$1" in
来源：http://ks.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://fs.panjiajie.cn

stop)  echo "停止" ;;
来源：http://bc.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://fc.hahajie.cn

esac
来源：http://az.panjiajie.cn

[R12] for 遍历文件
来源：http://cx.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://sn.jianghongdianzi.cn

[R13] for 计数循环
来源：http://lb.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://lj.shxzskj.cn

[R14] C 风格 for
来源：http://ph.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hi.szsharing.cn

[R15] while 逐行读文件
来源：http://zr.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tg.nszjky.cn

[R16] until 等待条件
来源：http://ol.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ml.huixiangedu.cn

[R17] 数组定义与取值
来源：http://rp.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fz.lnxyls.cn

[R18] 遍历数组
来源：http://rg.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mj.hahajie.cn

[R19] 数组长度
来源：http://ce.9csxet.cn

echo "${#arr[@]}"
来源：http://ws.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://ja.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ry.521024.cn

[R21] 字符串长度
来源：http://oh.521024.cn

echo "${#s}"
来源：http://br.shxzukj.cn

[R22] 截取子串
来源：http://rz.shxzskj.cn

echo "${s:0:5}"
来源：http://sk.haigaiapp.cn

[R23] 字符串替换
来源：http://pg.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yn.bjjhwx.cn

[R24] 大小写转换
来源：http://sb.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ob.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://ol.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qp.huanxung.cn

[R26] 命令替换
来源：http://ol.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://jo.huixiangedu.cn

[R27] 算术展开
来源：http://qz.szsharing.cn

echo $((1 + 2 * 3))
来源：http://tp.hahajie.cn

[R28] 浮点运算
来源：http://vt.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://pe.newstarts.cn

[R29] 定义函数
来源：http://vy.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rn.hnjuh.cn

[R30] 函数返回状态码
来源：http://fy.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://cl.9csxet.cn

[R31] 局部变量
来源：http://zr.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://mb.szsharing.cn

[R32] 参数个数校验
来源：http://xa.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zl.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://cz.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xk.asd995.cn

[R34] 退出时清理
来源：http://nh.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dw.szsharing.cn

[R35] 后台执行并等待
来源：http://zk.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zj.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://gw.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ct.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://ma.szxytkj.cn

files=$(ls -1)
来源：http://mc.szxytkj.cn

[R38] 管道串联
来源：http://ct.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://fx.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://vx.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://xv.panjiajie.cn

[R40] 追加写日志
来源：http://et.huanxung.cn

echo "log" >> out.log
来源：http://co.wgjwhj.cn

[R41] 丢弃输出
来源：http://dr.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://pm.nicolike.cn

[R42] 输入重定向
来源：http://lo.huixinmuqiang.cn

wc -l < a.txt
来源：http://gp.yuexingan06.cn

[R43] 按名字查找文件
来源：http://to.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://uo.hahajie.cn

[R44] 按修改时间查找
来源：http://iv.huanxung.cn

find . -mtime -7 -type f
来源：http://od.shxzukj.cn

[R45] 批量删除
来源：http://il.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://oi.lnxyls.cn

[R46] 递归替换文件内容
来源：http://kv.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qd.szsharing.cn

[R47] sed 单行替换
来源：http://rg.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yb.gzmigu.cn

[R48] awk 取指定列
来源：http://dd.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://iv.shxzskj.cn

[R49] awk 带条件
来源：http://le.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wd.nszjky.cn

[R50] awk 求和
来源：http://kv.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ug.panjiajie.cn

[R51] 排序去重取前几
来源：http://yc.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sr.hnjuh.cn

[R52] 统计行数
来源：http://ku.nicolike.cn

wc -l a.txt
来源：http://ft.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://qq.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://id.hahajie.cn

[R54] 比较两个文件
来源：http://if.hnjuh.cn

diff a.txt b.txt
来源：http://fy.huixiangedu.cn

[R55] 压缩与解压
来源：http://yi.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fj.gzmigu.cn

[R56] 远程拷贝
来源：http://yo.nicolike.cn

scp file user@host:/path/
来源：http://ms.lnxyls.cn

[R57] 远程执行命令
来源：http://iu.szxytkj.cn

ssh user@host 'uptime'
来源：http://hz.9csxet.cn

[R58] 下载文件
来源：http://za.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xg.newstarts.cn

[R59] 发 POST JSON
来源：http://jo.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zg.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://va.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xi.9csxet.cn

[R61] 磁盘占用
来源：http://xt.chemitech.net.cn

df -h;  du -sh *
来源：http://wy.hnjuh.cn

[R62] 找最占空间的文件
来源：http://du.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://qw.bjjhwx.cn

[R63] 内存与进程
来源：http://zj.521024.cn

free -h;  ps aux | grep nginx
来源：http://ok.huixinmuqiang.cn

[R64] 结束进程
来源：http://ym.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://vk.hnjuh.cn

[R65] 查看端口占用
来源：http://nw.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ux.jianghongdianzi.cn

[R66] 定时任务
来源：http://ws.gzmigu.cn

crontab -e;  crontab -l
来源：http://ms.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://vt.huanxung.cn

openssl rand -hex 16
来源：http://wt.haigaiapp.cn

[R68] 计算文件校验值
来源：http://jh.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yv.jctech888.com.cn

[R69] 生成随机密码
来源：http://gf.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://yl.hnjuh.cn

[R70] 时间戳与互转
来源：http://uf.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://sn.szxytkj.cn

[R71] 日期格式化
来源：http://sv.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sj.gzmigu.cn

[R72] 等待端口就绪
来源：http://ki.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ew.yuexingan06.cn

[R73] 分割大日志
来源：http://zo.panjiajie.cn

split -l 1000 big.log part_
来源：http://dv.bookmarksfly.cn

[R74] 批量重命名
来源：http://py.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yp.lnxyls.cn

[R75] 导出环境变量
来源：http://le.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://eo.chemitech.net.cn

[R76] 使用临时文件
来源：http://uq.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://za.asd995.cn

[R77] 读取用户输入
来源：http://mu.lnxyls.cn

read -rp "请输入: " ans
来源：http://rt.hahajie.cn

[R78] 交互式菜单
来源：http://pd.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pp.lnxyls.cn

[R79] 解析命令行选项
来源：http://tv.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ld.asd995.cn

[R80] 查看脚本执行耗时
来源：http://cn.hahajie.cn

time ./run.sh
来源：http://fk.huixinmuqiang.cn

================================================================================
来源：http://gz.gzmigu.cn

S. C / C++ 专题
来源：http://rw.colortex.cn

================================================================================
来源：http://hl.gzmigu.cn

[S01] C：Hello World
来源：http://jl.bjjhwx.cn

#include <stdio.h>
来源：http://pj.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ht.szsharing.cn

[S02] C：变量与格式化输出
来源：http://ip.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://tm.jianghongdianzi.cn

[S03] C：读入整数
来源：http://rm.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://nm.panjiajie.cn

[S04] C：字符串复制
来源：http://vy.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tu.gzmigu.cn

[S05] C：字符串长度
来源：http://bd.gzmigu.cn

strlen(s)
来源：http://jh.bookmarksfly.cn

[S06] C：字符串比较
来源：http://kg.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://bx.asd995.cn

[S07] C：数组遍历求和
来源：http://rl.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vy.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://da.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lx.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://hh.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://im.lnxyls.cn

[S10] C：指针与解引用
来源：http://fd.szsharing.cn

int *p = &a;  *p = 5;
来源：http://eo.muxihuayi.cn

[S11] C：逐行读文件
来源：http://es.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://es.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ma.haigaiapp.cn

fclose(f);
来源：http://jn.shxzskj.cn

[S12] C：写文件
来源：http://ph.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sm.szsharing.cn

[S13] C：宏定义
来源：http://ls.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vb.hahajie.cn

[S14] C：枚举
来源：http://xj.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://iy.lnxyls.cn

[S15] C：类型转换
来源：http://gn.shxzukj.cn

(double) a / b
来源：http://ca.newstarts.cn

[S16] C：位操作置位
来源：http://ei.huanxung.cn

x |= (1 << 3);
来源：http://oh.colortex.cn

[S17] C：安全拼接字符串
来源：http://nv.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://je.bjjhwx.cn

[S18] C：命令行参数
来源：http://pd.gzmigu.cn

int main(int argc, char **argv)
来源：http://si.muxihuayi.cn

[S19] C：快速排序
来源：http://xc.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mb.hnjuh.cn

[S20] C：二分查找
来源：http://st.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.asd995.cn

[S21] C：字符类别判断
来源：http://db.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sm.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://sg.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ar.szxytkj.cn

[S23] C：随机数
来源：http://kw.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pu.jctech888.com.cn

[S24] C：获取本地时间
来源：http://ug.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mz.521024.cn

[S25] C：内存拷贝
来源：http://rq.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://hh.gzmigu.cn

[S26] C：内存清零
来源：http://yo.9csxet.cn

memset(a, 0, sizeof a);
来源：http://uu.asd995.cn

[S27] C：定义常量
来源：http://hv.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://bq.wgjwhj.cn

[S28] C：静态变量
来源：http://cf.muxihuayi.cn

static int counter = 0;
来源：http://pk.shxzukj.cn

[S29] C：变参函数
来源：http://kp.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dy.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://hf.shxzskj.cn

#ifndef X_H
来源：http://wz.yuexingan06.cn

#define X_H
来源：http://yw.yuntaijiaju.cn

#endif
来源：http://wg.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://cg.bjjhwx.cn

#include <iostream>
来源：http://io.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://aw.panjiajie.cn

[S32] C++：字符串
来源：http://jw.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://nt.hahajie.cn

[S33] C++：vector 增删
来源：http://gw.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vu.hnjuh.cn

[S34] C++：遍历 vector
来源：http://sj.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://cx.huixinmuqiang.cn

[S35] C++：map
来源：http://bz.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ld.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://sg.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nn.yuntaijiaju.cn

[S37] C++：set
来源：http://dq.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ns.colortex.cn

[S38] C++：排序
来源：http://hd.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://xn.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://fp.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vn.hahajie.cn

[S40] C++：查找元素
来源：http://xo.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xm.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://oe.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://py.szsharing.cn

[S42] C++：继承与虚函数
来源：http://vt.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://lf.szsharing.cn

[S43] C++：智能指针
来源：http://fz.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://yh.521024.cn

[S44] C++：引用传参
来源：http://qj.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://ad.szxytkj.cn

[S45] C++：lambda
来源：http://hd.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://my.hnjuh.cn

[S46] C++：函数模板
来源：http://gz.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hj.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://xw.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ps.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://dq.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yi.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://jj.huanxung.cn

[S49] C++：写文件
来源：http://vu.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ij.haigaiapp.cn

[S50] C++：格式化数字
来源：http://ul.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ge.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://ev.asd995.cn

static_cast<double>(a) / b
来源：http://ed.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://qo.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://fr.szsharing.cn

[S53] C++：移动语义
来源：http://pp.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://cy.chemitech.net.cn

[S54] C++：异常处理
来源：http://ll.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://do.shxzukj.cn

[S55] C++：结构化绑定
来源：http://ty.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lj.hahajie.cn

[S56] C++：optional
来源：http://rg.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mj.shxzskj.cn

[S57] C++：编译期常量
来源：http://id.jctech888.com.cn

constexpr int N = 10;
来源：http://zf.bjjhwx.cn

[S58] C++：命名空间
来源：http://tb.521024.cn

namespace ns { int f() { return 1; } }
来源：http://sl.shtwfgs.cn

[S59] C++：静态断言
来源：http://ej.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ak.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://xg.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yl.chemitech.net.cn

================================================================================
来源：http://pg.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xp.hahajie.cn

================================================================================
来源：http://ha.colortex.cn

[T01] Kotlin：Hello World
来源：http://ji.521024.cn

println("Hello")
来源：http://rw.nszjky.cn

[T02] Kotlin：变量
来源：http://pa.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kx.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://zr.lnxyls.cn

"值: $b"
来源：http://xv.huanxung.cn

[T04] Kotlin：空安全
来源：http://xv.9csxet.cn

val n: String? = null;  n?.length
来源：http://qs.colortex.cn


<!-- 参考信息 -->