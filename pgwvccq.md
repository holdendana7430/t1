代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zb.nszjky.cn

[R08] 数值比较
来源：http://id.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://od.shxzskj.cn

[R09] 字符串比较
来源：http://gu.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lv.huixinmuqiang.cn

[R10] 正则匹配
来源：http://hl.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xy.521024.cn

[R11] case 多分支
来源：http://na.jctech888.com.cn

case "$1" in
来源：http://jz.shxzskj.cn

start) echo "启动" ;;
来源：http://xe.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://hk.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://rj.hnjuh.cn

esac
来源：http://ux.nicolike.cn

[R12] for 遍历文件
来源：http://gy.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://vn.bjjhwx.cn

[R13] for 计数循环
来源：http://fq.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://vp.huixiangedu.cn

[R14] C 风格 for
来源：http://yx.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ga.hahajie.cn

[R15] while 逐行读文件
来源：http://oa.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fw.newstarts.cn

[R16] until 等待条件
来源：http://vb.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zs.panjiajie.cn

[R17] 数组定义与取值
来源：http://vu.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oo.huanxung.cn

[R18] 遍历数组
来源：http://co.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jr.haigaiapp.cn

[R19] 数组长度
来源：http://yw.asd995.cn

echo "${#arr[@]}"
来源：http://ii.hnjuh.cn

[R20] 关联数组（字典）
来源：http://pj.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wp.jianghongdianzi.cn

[R21] 字符串长度
来源：http://tx.shxzukj.cn

echo "${#s}"
来源：http://dk.yuntaijiaju.cn

[R22] 截取子串
来源：http://wy.szsharing.cn

echo "${s:0:5}"
来源：http://dv.panjiajie.cn

[R23] 字符串替换
来源：http://an.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://el.szxytkj.cn

[R24] 大小写转换
来源：http://hk.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ve.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://ws.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iy.bookmarksfly.cn

[R26] 命令替换
来源：http://qp.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://dp.hahajie.cn

[R27] 算术展开
来源：http://xi.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://wr.jctech888.com.cn

[R28] 浮点运算
来源：http://we.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://rf.bjjhwx.cn

[R29] 定义函数
来源：http://wg.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kh.9csxet.cn

[R30] 函数返回状态码
来源：http://hm.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://qn.yuexingan06.cn

[R31] 局部变量
来源：http://cx.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://gr.newstarts.cn

[R32] 参数个数校验
来源：http://mx.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qi.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://wp.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yf.bookmarksfly.cn

[R34] 退出时清理
来源：http://sq.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lv.panjiajie.cn

[R35] 后台执行并等待
来源：http://qt.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://if.521024.cn

[R36] 并发执行多个任务
来源：http://pb.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mg.hahajie.cn

[R37] 把输出赋给变量
来源：http://kk.jctech888.com.cn

files=$(ls -1)
来源：http://jm.asd995.cn

[R38] 管道串联
来源：http://fv.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://cu.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://is.hahajie.cn

cmd > out.log 2>&1
来源：http://ms.shxzukj.cn

[R40] 追加写日志
来源：http://sx.jianghongdianzi.cn

echo "log" >> out.log
来源：http://gl.9csxet.cn

[R41] 丢弃输出
来源：http://my.9csxet.cn

cmd >/dev/null 2>&1
来源：http://zf.colortex.cn

[R42] 输入重定向
来源：http://hn.muxihuayi.cn

wc -l < a.txt
来源：http://fn.newstarts.cn

[R43] 按名字查找文件
来源：http://kf.huixiangedu.cn

find . -name "*.log" -type f
来源：http://gt.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://kq.shxzukj.cn

find . -mtime -7 -type f
来源：http://tv.jianghongdianzi.cn

[R45] 批量删除
来源：http://jk.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://xl.colortex.cn

[R46] 递归替换文件内容
来源：http://ge.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tx.nicolike.cn

[R47] sed 单行替换
来源：http://fa.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ld.9csxet.cn

[R48] awk 取指定列
来源：http://os.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://kh.huanxung.cn

[R49] awk 带条件
来源：http://gj.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vn.shxzukj.cn

[R50] awk 求和
来源：http://qd.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ym.szxytkj.cn

[R51] 排序去重取前几
来源：http://jl.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pz.jctech888.com.cn

[R52] 统计行数
来源：http://aj.yuntaijiaju.cn

wc -l a.txt
来源：http://gc.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://we.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fb.521024.cn

[R54] 比较两个文件
来源：http://ki.521024.cn

diff a.txt b.txt
来源：http://kr.wgjwhj.cn

[R55] 压缩与解压
来源：http://jt.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vc.asd995.cn

[R56] 远程拷贝
来源：http://lx.wgjwhj.cn

scp file user@host:/path/
来源：http://dn.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://kg.shtwfgs.cn

ssh user@host 'uptime'
来源：http://er.bookmarksfly.cn

[R58] 下载文件
来源：http://ig.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://we.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ni.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xv.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ck.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://no.yuexingan06.cn

[R61] 磁盘占用
来源：http://ub.yuntaijiaju.cn

df -h;  du -sh *
来源：http://xx.hahajie.cn

[R62] 找最占空间的文件
来源：http://ye.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://ow.yuntaijiaju.cn

[R63] 内存与进程
来源：http://vo.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://di.shtwfgs.cn

[R64] 结束进程
来源：http://ch.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://xb.newstarts.cn

[R65] 查看端口占用
来源：http://kh.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yx.chemitech.net.cn

[R66] 定时任务
来源：http://vt.asd995.cn

crontab -e;  crontab -l
来源：http://ea.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://uv.huanxung.cn

openssl rand -hex 16
来源：http://vl.hahajie.cn

[R68] 计算文件校验值
来源：http://os.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uz.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://jc.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://oq.lnxyls.cn

[R70] 时间戳与互转
来源：http://jn.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://rp.hahajie.cn

[R71] 日期格式化
来源：http://xg.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jj.szxytkj.cn

[R72] 等待端口就绪
来源：http://dy.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ip.wgjwhj.cn

[R73] 分割大日志
来源：http://zo.bjjhwx.cn

split -l 1000 big.log part_
来源：http://uy.huixinmuqiang.cn

[R74] 批量重命名
来源：http://bi.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zb.yuexingan06.cn

[R75] 导出环境变量
来源：http://jm.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://qa.panjiajie.cn

[R76] 使用临时文件
来源：http://yq.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dp.bjjhwx.cn

[R77] 读取用户输入
来源：http://oz.hnjuh.cn

read -rp "请输入: " ans
来源：http://gr.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://xy.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tz.jctech888.com.cn

[R79] 解析命令行选项
来源：http://sz.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dq.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://ra.shxzskj.cn

time ./run.sh
来源：http://qj.huixiangedu.cn

================================================================================
来源：http://li.muxihuayi.cn

S. C / C++ 专题
来源：http://eh.hnjuh.cn

================================================================================
来源：http://jm.panjiajie.cn

[S01] C：Hello World
来源：http://hr.yuntaijiaju.cn

#include <stdio.h>
来源：http://df.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sa.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://fr.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://qr.jianghongdianzi.cn

[S03] C：读入整数
来源：http://le.newstarts.cn

int x; scanf("%d", &x);
来源：http://aj.bookmarksfly.cn

[S04] C：字符串复制
来源：http://ra.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oj.newstarts.cn

[S05] C：字符串长度
来源：http://jt.nszjky.cn

strlen(s)
来源：http://hq.shxzskj.cn

[S06] C：字符串比较
来源：http://sl.shxzskj.cn

strcmp(a, b) == 0
来源：http://kh.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://zf.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://es.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://zb.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aw.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://nh.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ac.lnxyls.cn

[S10] C：指针与解引用
来源：http://om.521024.cn

int *p = &a;  *p = 5;
来源：http://lg.wgjwhj.cn

[S11] C：逐行读文件
来源：http://ol.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://ms.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bi.szxytkj.cn

fclose(f);
来源：http://ki.gzmigu.cn

[S12] C：写文件
来源：http://ab.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ln.wgjwhj.cn

[S13] C：宏定义
来源：http://gh.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hm.nicolike.cn

[S14] C：枚举
来源：http://cc.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ip.shtwfgs.cn

[S15] C：类型转换
来源：http://go.lnxyls.cn

(double) a / b
来源：http://fv.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://ji.huixinmuqiang.cn

x |= (1 << 3);
来源：http://av.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://kt.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://on.asd995.cn

[S18] C：命令行参数
来源：http://ck.muxihuayi.cn

int main(int argc, char **argv)
来源：http://wv.panjiajie.cn

[S19] C：快速排序
来源：http://sy.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://au.9csxet.cn

[S20] C：二分查找
来源：http://nq.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ba.szxytkj.cn

[S21] C：字符类别判断
来源：http://uq.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cf.gzmigu.cn

[S22] C：字符串转数字
来源：http://xn.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tk.gzmigu.cn

[S23] C：随机数
来源：http://ft.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nc.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://cd.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cf.colortex.cn

[S25] C：内存拷贝
来源：http://dn.szsharing.cn

memcpy(dst, src, n);
来源：http://pp.shxzskj.cn

[S26] C：内存清零
来源：http://lm.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://ip.huanxung.cn

[S27] C：定义常量
来源：http://iu.haigaiapp.cn

const double PI = 3.14159;
来源：http://cb.bjjhwx.cn

[S28] C：静态变量
来源：http://rq.shxzskj.cn

static int counter = 0;
来源：http://yo.huanxung.cn

[S29] C：变参函数
来源：http://yp.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oc.bookmarksfly.cn

[S30] C：头文件保护
来源：http://ox.gzmigu.cn

#ifndef X_H
来源：http://hb.panjiajie.cn

#define X_H
来源：http://cp.521024.cn

#endif
来源：http://rn.hnjuh.cn

[S31] C++：Hello World
来源：http://bu.shtwfgs.cn

#include <iostream>
来源：http://om.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://er.lnxyls.cn

[S32] C++：字符串
来源：http://uj.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://dm.asd995.cn

[S33] C++：vector 增删
来源：http://uj.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rl.lnxyls.cn

[S34] C++：遍历 vector
来源：http://gl.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://oi.chemitech.net.cn

[S35] C++：map
来源：http://wd.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hf.nicolike.cn

[S36] C++：unordered_map
来源：http://nr.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kc.lnxyls.cn

[S37] C++：set
来源：http://vy.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nz.szsharing.cn

[S38] C++：排序
来源：http://la.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://bq.521024.cn

[S39] C++：自定义比较器排序
来源：http://ef.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lh.jctech888.com.cn

[S40] C++：查找元素
来源：http://ty.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nk.nicolike.cn

[S41] C++：类与构造函数
来源：http://db.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hc.colortex.cn

[S42] C++：继承与虚函数
来源：http://ic.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://et.521024.cn

[S43] C++：智能指针
来源：http://ny.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://jn.huixiangedu.cn

[S44] C++：引用传参
来源：http://xt.9csxet.cn

void inc(int &x) { ++x; }
来源：http://xn.yuexingan06.cn

[S45] C++：lambda
来源：http://kq.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mp.nszjky.cn

[S46] C++：函数模板
来源：http://bm.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mi.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://wc.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://el.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://ye.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oi.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://wu.huixinmuqiang.cn

[S49] C++：写文件
来源：http://ia.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yp.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://mg.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hr.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://in.asd995.cn

static_cast<double>(a) / b
来源：http://fs.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://yh.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://wo.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://za.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://nh.szxytkj.cn

[S54] C++：异常处理
来源：http://jk.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gc.szsharing.cn

[S55] C++：结构化绑定
来源：http://nj.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uu.gzmigu.cn

[S56] C++：optional
来源：http://to.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ap.lnxyls.cn

[S57] C++：编译期常量
来源：http://iv.asd995.cn

constexpr int N = 10;
来源：http://af.hahajie.cn

[S58] C++：命名空间
来源：http://vr.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://hm.huixiangedu.cn

[S59] C++：静态断言
来源：http://jt.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rg.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://zv.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kj.hnjuh.cn

================================================================================
来源：http://dw.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yg.newstarts.cn

================================================================================
来源：http://qi.hahajie.cn

[T01] Kotlin：Hello World
来源：http://hx.bjjhwx.cn

println("Hello")
来源：http://vq.nicolike.cn

[T02] Kotlin：变量
来源：http://jj.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://st.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://wg.nszjky.cn

"值: $b"
来源：http://og.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://mk.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://tk.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://ov.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jr.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://yv.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ri.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://qq.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wi.gzmigu.cn

[T08] Kotlin：数据类
来源：http://ac.521024.cn

data class User(val name: String, val age: Int)
来源：http://fj.shxzskj.cn


<!-- 参考信息 -->