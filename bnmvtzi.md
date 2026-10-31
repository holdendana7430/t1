代发 wailian999

set -euo pipefail
来源：http://ik.shxzskj.cn

[R02] 变量赋值与使用
来源：http://om.huanxung.cn

name="Tom"; echo "$name"
来源：http://bf.bookmarksfly.cn

[R03] 只读变量
来源：http://hk.huanxung.cn

readonly PI=3.14
来源：http://ke.521024.cn

[R04] 位置参数
来源：http://cm.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ow.szxytkj.cn

[R05] 参数默认值
来源：http://zp.521024.cn

name="${1:-default}"
来源：http://zd.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://np.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fw.gzmigu.cn

[R07] if 判断文件
来源：http://my.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://us.shxzukj.cn

[R08] 数值比较
来源：http://cs.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dr.szxytkj.cn

[R09] 字符串比较
来源：http://bv.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ji.newstarts.cn

[R10] 正则匹配
来源：http://ab.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ob.huixiangedu.cn

[R11] case 多分支
来源：http://nm.haigaiapp.cn

case "$1" in
来源：http://wc.asd995.cn

start) echo "启动" ;;
来源：http://fs.lnxyls.cn

stop)  echo "停止" ;;
来源：http://yn.colortex.cn

*)     echo "未知命令" ;;
来源：http://zp.shxzukj.cn

esac
来源：http://qy.nszjky.cn

[R12] for 遍历文件
来源：http://hu.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://jk.yuntaijiaju.cn

[R13] for 计数循环
来源：http://ra.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://id.gzmigu.cn

[R14] C 风格 for
来源：http://ay.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mx.shxzskj.cn

[R15] while 逐行读文件
来源：http://ol.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yu.newstarts.cn

[R16] until 等待条件
来源：http://tk.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ev.szsharing.cn

[R17] 数组定义与取值
来源：http://nq.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vg.chemitech.net.cn

[R18] 遍历数组
来源：http://zc.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wl.huanxung.cn

[R19] 数组长度
来源：http://cu.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://ws.asd995.cn

[R20] 关联数组（字典）
来源：http://fs.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eh.chemitech.net.cn

[R21] 字符串长度
来源：http://vy.panjiajie.cn

echo "${#s}"
来源：http://yo.huixinmuqiang.cn

[R22] 截取子串
来源：http://ca.bjjhwx.cn

echo "${s:0:5}"
来源：http://rz.huanxung.cn

[R23] 字符串替换
来源：http://fn.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tn.bjjhwx.cn

[R24] 大小写转换
来源：http://bq.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rw.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://wp.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pp.hahajie.cn

[R26] 命令替换
来源：http://mo.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://rk.haigaiapp.cn

[R27] 算术展开
来源：http://sl.asd995.cn

echo $((1 + 2 * 3))
来源：http://cq.bjjhwx.cn

[R28] 浮点运算
来源：http://zg.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://uk.newstarts.cn

[R29] 定义函数
来源：http://mh.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bi.521024.cn

[R30] 函数返回状态码
来源：http://wa.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://fb.shxzukj.cn

[R31] 局部变量
来源：http://ai.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://we.gzmigu.cn

[R32] 参数个数校验
来源：http://qy.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ci.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://qs.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dg.521024.cn

[R34] 退出时清理
来源：http://jm.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cx.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://fq.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tp.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://dg.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bi.lnxyls.cn

[R37] 把输出赋给变量
来源：http://ql.szsharing.cn

files=$(ls -1)
来源：http://lq.wgjwhj.cn

[R38] 管道串联
来源：http://hm.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://qf.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://no.hahajie.cn

cmd > out.log 2>&1
来源：http://ai.yuntaijiaju.cn

[R40] 追加写日志
来源：http://aw.chemitech.net.cn

echo "log" >> out.log
来源：http://xy.asd995.cn

[R41] 丢弃输出
来源：http://lp.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://my.szxytkj.cn

[R42] 输入重定向
来源：http://su.huanxung.cn

wc -l < a.txt
来源：http://uk.bjjhwx.cn

[R43] 按名字查找文件
来源：http://ek.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://gz.panjiajie.cn

[R44] 按修改时间查找
来源：http://sf.colortex.cn

find . -mtime -7 -type f
来源：http://wt.muxihuayi.cn

[R45] 批量删除
来源：http://ng.nszjky.cn

find . -name "*.tmp" -delete
来源：http://hv.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://mv.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wd.nszjky.cn

[R47] sed 单行替换
来源：http://ng.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wu.chemitech.net.cn

[R48] awk 取指定列
来源：http://eb.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://ar.lnxyls.cn

[R49] awk 带条件
来源：http://tw.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://op.huixinmuqiang.cn

[R50] awk 求和
来源：http://ue.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pf.shtwfgs.cn

[R51] 排序去重取前几
来源：http://ki.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qz.panjiajie.cn

[R52] 统计行数
来源：http://xm.wgjwhj.cn

wc -l a.txt
来源：http://hm.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://ho.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vb.chemitech.net.cn

[R54] 比较两个文件
来源：http://yj.lnxyls.cn

diff a.txt b.txt
来源：http://rt.hnjuh.cn

[R55] 压缩与解压
来源：http://hb.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xn.9csxet.cn

[R56] 远程拷贝
来源：http://hr.panjiajie.cn

scp file user@host:/path/
来源：http://ow.huixiangedu.cn

[R57] 远程执行命令
来源：http://uz.hnjuh.cn

ssh user@host 'uptime'
来源：http://ql.huixinmuqiang.cn

[R58] 下载文件
来源：http://xl.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://se.colortex.cn

[R59] 发 POST JSON
来源：http://po.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hi.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://sr.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xx.lnxyls.cn

[R61] 磁盘占用
来源：http://oc.shtwfgs.cn

df -h;  du -sh *
来源：http://bw.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://yw.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://sv.jianghongdianzi.cn

[R63] 内存与进程
来源：http://mu.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://os.huixinmuqiang.cn

[R64] 结束进程
来源：http://yt.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://al.haigaiapp.cn

[R65] 查看端口占用
来源：http://cc.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ho.panjiajie.cn

[R66] 定时任务
来源：http://rc.szsharing.cn

crontab -e;  crontab -l
来源：http://zg.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://oh.bookmarksfly.cn

openssl rand -hex 16
来源：http://ab.hnjuh.cn

[R68] 计算文件校验值
来源：http://vm.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rc.colortex.cn

[R69] 生成随机密码
来源：http://jj.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://tq.chemitech.net.cn

[R70] 时间戳与互转
来源：http://rs.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://yl.huanxung.cn

[R71] 日期格式化
来源：http://mo.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gx.hnjuh.cn

[R72] 等待端口就绪
来源：http://mk.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://co.szsharing.cn

[R73] 分割大日志
来源：http://lk.bjjhwx.cn

split -l 1000 big.log part_
来源：http://jm.newstarts.cn

[R74] 批量重命名
来源：http://qz.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eb.hahajie.cn

[R75] 导出环境变量
来源：http://zr.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://xh.bookmarksfly.cn

[R76] 使用临时文件
来源：http://jr.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jo.panjiajie.cn

[R77] 读取用户输入
来源：http://sm.haigaiapp.cn

read -rp "请输入: " ans
来源：http://kv.gzmigu.cn

[R78] 交互式菜单
来源：http://es.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jb.gzmigu.cn

[R79] 解析命令行选项
来源：http://sz.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gz.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://cp.jianghongdianzi.cn

time ./run.sh
来源：http://kz.jctech888.com.cn

================================================================================
来源：http://vw.chemitech.net.cn

S. C / C++ 专题
来源：http://gt.9csxet.cn

================================================================================
来源：http://oy.szxytkj.cn

[S01] C：Hello World
来源：http://ca.panjiajie.cn

#include <stdio.h>
来源：http://zo.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ko.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://iy.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://lq.nicolike.cn

[S03] C：读入整数
来源：http://gi.szxytkj.cn

int x; scanf("%d", &x);
来源：http://yx.nicolike.cn

[S04] C：字符串复制
来源：http://og.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yd.huixiangedu.cn

[S05] C：字符串长度
来源：http://jj.hahajie.cn

strlen(s)
来源：http://nv.hahajie.cn

[S06] C：字符串比较
来源：http://vu.lnxyls.cn

strcmp(a, b) == 0
来源：http://np.huanxung.cn

[S07] C：数组遍历求和
来源：http://qm.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ab.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://in.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ys.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://nh.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cs.asd995.cn

[S10] C：指针与解引用
来源：http://el.asd995.cn

int *p = &a;  *p = 5;
来源：http://nc.huixiangedu.cn

[S11] C：逐行读文件
来源：http://zt.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://ax.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tu.gzmigu.cn

fclose(f);
来源：http://hz.lnxyls.cn

[S12] C：写文件
来源：http://py.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ja.nszjky.cn

[S13] C：宏定义
来源：http://wx.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xk.muxihuayi.cn

[S14] C：枚举
来源：http://gw.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://hf.shxzukj.cn

[S15] C：类型转换
来源：http://ta.gzmigu.cn

(double) a / b
来源：http://ks.gzmigu.cn

[S16] C：位操作置位
来源：http://nz.521024.cn

x |= (1 << 3);
来源：http://et.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://om.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zl.szxytkj.cn

[S18] C：命令行参数
来源：http://bz.panjiajie.cn

int main(int argc, char **argv)
来源：http://gm.shxzskj.cn

[S19] C：快速排序
来源：http://kj.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wm.huixiangedu.cn

[S20] C：二分查找
来源：http://gg.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wl.newstarts.cn

[S21] C：字符类别判断
来源：http://ii.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xz.huixiangedu.cn

[S22] C：字符串转数字
来源：http://ve.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ui.yuntaijiaju.cn

[S23] C：随机数
来源：http://ze.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mg.jctech888.com.cn

[S24] C：获取本地时间
来源：http://wf.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bg.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://bj.newstarts.cn

memcpy(dst, src, n);
来源：http://sx.shxzukj.cn

[S26] C：内存清零
来源：http://xx.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://ik.muxihuayi.cn

[S27] C：定义常量
来源：http://do.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://uj.huixiangedu.cn

[S28] C：静态变量
来源：http://fm.shxzskj.cn

static int counter = 0;
来源：http://dz.bjjhwx.cn

[S29] C：变参函数
来源：http://fs.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zs.asd995.cn

[S30] C：头文件保护
来源：http://qz.newstarts.cn

#ifndef X_H
来源：http://ht.huixiangedu.cn

#define X_H
来源：http://zm.huixinmuqiang.cn

#endif
来源：http://sf.hnjuh.cn

[S31] C++：Hello World
来源：http://ku.nicolike.cn

#include <iostream>
来源：http://lb.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://or.chemitech.net.cn

[S32] C++：字符串
来源：http://vg.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://ji.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://gh.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kr.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://pd.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://hz.muxihuayi.cn

[S35] C++：map
来源：http://yr.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ay.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://zm.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dk.nszjky.cn

[S37] C++：set
来源：http://qz.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fn.newstarts.cn

[S38] C++：排序
来源：http://fn.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://sy.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://ri.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ri.nicolike.cn

[S40] C++：查找元素
来源：http://wv.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://do.9csxet.cn

[S41] C++：类与构造函数
来源：http://oq.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yz.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://gy.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://to.bjjhwx.cn

[S43] C++：智能指针
来源：http://bs.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://fj.szxytkj.cn

[S44] C++：引用传参
来源：http://zh.9csxet.cn

void inc(int &x) { ++x; }
来源：http://cy.chemitech.net.cn

[S45] C++：lambda
来源：http://mr.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jg.shxzskj.cn

[S46] C++：函数模板
来源：http://up.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uf.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://mn.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gg.szsharing.cn

[S48] C++：逐行读文件
来源：http://nv.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://be.szsharing.cn

while (std::getline(in, line)) { }
来源：http://tc.muxihuayi.cn

[S49] C++：写文件
来源：http://ji.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qr.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://fh.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rb.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://ue.asd995.cn

static_cast<double>(a) / b
来源：http://kq.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://ks.9csxet.cn

int size() const noexcept { return n_; }
来源：http://sf.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://nt.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://hn.hahajie.cn

[S54] C++：异常处理
来源：http://ph.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://up.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://ye.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kk.wgjwhj.cn

[S56] C++：optional
来源：http://mz.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cu.nszjky.cn

[S57] C++：编译期常量
来源：http://yx.wgjwhj.cn

constexpr int N = 10;
来源：http://xk.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://rw.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://pq.shtwfgs.cn

[S59] C++：静态断言
来源：http://rw.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fg.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://je.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xd.bookmarksfly.cn

================================================================================
来源：http://fm.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kb.hnjuh.cn

================================================================================
来源：http://cq.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://tr.yuntaijiaju.cn

println("Hello")
来源：http://le.huanxung.cn

[T02] Kotlin：变量
来源：http://sw.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aw.haigaiapp.cn


<!-- 参考信息 -->