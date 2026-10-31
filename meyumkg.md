代发 wailian999

readonly PI=3.14
来源：http://fe.huixiangedu.cn

[R04] 位置参数
来源：http://vo.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ky.asd995.cn

[R05] 参数默认值
来源：http://rz.yuntaijiaju.cn

name="${1:-default}"
来源：http://gi.szsharing.cn

[R06] 判断命令是否存在
来源：http://lv.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wi.huixinmuqiang.cn

[R07] if 判断文件
来源：http://cm.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cy.jctech888.com.cn

[R08] 数值比较
来源：http://ej.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rt.jctech888.com.cn

[R09] 字符串比较
来源：http://fp.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ew.shxzukj.cn

[R10] 正则匹配
来源：http://av.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nc.521024.cn

[R11] case 多分支
来源：http://jt.newstarts.cn

case "$1" in
来源：http://ig.newstarts.cn

start) echo "启动" ;;
来源：http://qv.lnxyls.cn

stop)  echo "停止" ;;
来源：http://iq.nicolike.cn

*)     echo "未知命令" ;;
来源：http://fg.haigaiapp.cn

esac
来源：http://jv.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://vt.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://am.lnxyls.cn

[R13] for 计数循环
来源：http://wu.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://va.hnjuh.cn

[R14] C 风格 for
来源：http://yr.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xx.shxzukj.cn

[R15] while 逐行读文件
来源：http://kv.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ky.szxytkj.cn

[R16] until 等待条件
来源：http://tn.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yh.yuexingan06.cn

[R17] 数组定义与取值
来源：http://wy.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hz.bookmarksfly.cn

[R18] 遍历数组
来源：http://wu.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wn.nicolike.cn

[R19] 数组长度
来源：http://ts.bjjhwx.cn

echo "${#arr[@]}"
来源：http://vm.nicolike.cn

[R20] 关联数组（字典）
来源：http://fr.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fb.521024.cn

[R21] 字符串长度
来源：http://tt.bjjhwx.cn

echo "${#s}"
来源：http://jt.hnjuh.cn

[R22] 截取子串
来源：http://hp.haigaiapp.cn

echo "${s:0:5}"
来源：http://jc.huixiangedu.cn

[R23] 字符串替换
来源：http://va.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pw.shxzukj.cn

[R24] 大小写转换
来源：http://zi.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pj.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://ay.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bq.asd995.cn

[R26] 命令替换
来源：http://et.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://no.colortex.cn

[R27] 算术展开
来源：http://hp.asd995.cn

echo $((1 + 2 * 3))
来源：http://oq.hnjuh.cn

[R28] 浮点运算
来源：http://pz.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://sc.wgjwhj.cn

[R29] 定义函数
来源：http://df.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iv.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://tp.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://io.shxzskj.cn

[R31] 局部变量
来源：http://un.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://rw.szsharing.cn

[R32] 参数个数校验
来源：http://hh.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ec.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://jk.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ma.szsharing.cn

[R34] 退出时清理
来源：http://xx.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rr.shtwfgs.cn

[R35] 后台执行并等待
来源：http://na.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mx.hnjuh.cn

[R36] 并发执行多个任务
来源：http://nk.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vu.hahajie.cn

[R37] 把输出赋给变量
来源：http://ej.bookmarksfly.cn

files=$(ls -1)
来源：http://gw.colortex.cn

[R38] 管道串联
来源：http://ji.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://rs.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://wj.bjjhwx.cn

cmd > out.log 2>&1
来源：http://eu.gzmigu.cn

[R40] 追加写日志
来源：http://mb.newstarts.cn

echo "log" >> out.log
来源：http://vc.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://ps.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://ng.haigaiapp.cn

[R42] 输入重定向
来源：http://bp.muxihuayi.cn

wc -l < a.txt
来源：http://qk.521024.cn

[R43] 按名字查找文件
来源：http://bu.huanxung.cn

find . -name "*.log" -type f
来源：http://tq.huanxung.cn

[R44] 按修改时间查找
来源：http://xc.huixiangedu.cn

find . -mtime -7 -type f
来源：http://ha.gzmigu.cn

[R45] 批量删除
来源：http://va.nszjky.cn

find . -name "*.tmp" -delete
来源：http://pv.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://tw.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uc.hnjuh.cn

[R47] sed 单行替换
来源：http://go.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hg.panjiajie.cn

[R48] awk 取指定列
来源：http://dp.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://qv.shxzukj.cn

[R49] awk 带条件
来源：http://sj.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sy.huanxung.cn

[R50] awk 求和
来源：http://hs.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dx.lnxyls.cn

[R51] 排序去重取前几
来源：http://ft.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kr.bjjhwx.cn

[R52] 统计行数
来源：http://pq.jianghongdianzi.cn

wc -l a.txt
来源：http://lc.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://la.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dy.chemitech.net.cn

[R54] 比较两个文件
来源：http://gl.newstarts.cn

diff a.txt b.txt
来源：http://fn.hnjuh.cn

[R55] 压缩与解压
来源：http://le.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gj.hahajie.cn

[R56] 远程拷贝
来源：http://qz.shxzskj.cn

scp file user@host:/path/
来源：http://me.haigaiapp.cn

[R57] 远程执行命令
来源：http://rs.gzmigu.cn

ssh user@host 'uptime'
来源：http://gi.haigaiapp.cn

[R58] 下载文件
来源：http://nb.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sy.shxzukj.cn

[R59] 发 POST JSON
来源：http://lt.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cy.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://dm.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://it.huanxung.cn

[R61] 磁盘占用
来源：http://vv.hnjuh.cn

df -h;  du -sh *
来源：http://ma.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://xi.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://pk.bookmarksfly.cn

[R63] 内存与进程
来源：http://qm.521024.cn

free -h;  ps aux | grep nginx
来源：http://ut.newstarts.cn

[R64] 结束进程
来源：http://jk.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://ei.huixiangedu.cn

[R65] 查看端口占用
来源：http://pk.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tt.haigaiapp.cn

[R66] 定时任务
来源：http://ph.jctech888.com.cn

crontab -e;  crontab -l
来源：http://ki.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://wa.hnjuh.cn

openssl rand -hex 16
来源：http://no.nicolike.cn

[R68] 计算文件校验值
来源：http://yq.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hs.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://hv.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://ad.haigaiapp.cn

[R70] 时间戳与互转
来源：http://qe.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://ff.newstarts.cn

[R71] 日期格式化
来源：http://ay.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tj.jctech888.com.cn

[R72] 等待端口就绪
来源：http://cd.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cx.asd995.cn

[R73] 分割大日志
来源：http://lh.jctech888.com.cn

split -l 1000 big.log part_
来源：http://ux.9csxet.cn

[R74] 批量重命名
来源：http://lj.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uk.shxzukj.cn

[R75] 导出环境变量
来源：http://rb.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://yq.521024.cn

[R76] 使用临时文件
来源：http://fn.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ry.bookmarksfly.cn

[R77] 读取用户输入
来源：http://jk.haigaiapp.cn

read -rp "请输入: " ans
来源：http://ej.huanxung.cn

[R78] 交互式菜单
来源：http://vr.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ho.nicolike.cn

[R79] 解析命令行选项
来源：http://gx.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oh.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://gj.521024.cn

time ./run.sh
来源：http://sh.yuexingan06.cn

================================================================================
来源：http://zh.panjiajie.cn

S. C / C++ 专题
来源：http://be.hahajie.cn

================================================================================
来源：http://ec.chemitech.net.cn

[S01] C：Hello World
来源：http://cq.szxytkj.cn

#include <stdio.h>
来源：http://nw.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fs.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://jp.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://ek.yuntaijiaju.cn

[S03] C：读入整数
来源：http://zp.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://iv.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://uz.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fq.huanxung.cn

[S05] C：字符串长度
来源：http://mz.jctech888.com.cn

strlen(s)
来源：http://ai.asd995.cn

[S06] C：字符串比较
来源：http://au.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://fe.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://sx.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zx.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://hu.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oo.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://qg.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tv.521024.cn

[S10] C：指针与解引用
来源：http://nf.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://xi.asd995.cn

[S11] C：逐行读文件
来源：http://jq.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://xb.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jc.shxzskj.cn

fclose(f);
来源：http://sy.szsharing.cn

[S12] C：写文件
来源：http://ix.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kj.hnjuh.cn

[S13] C：宏定义
来源：http://yg.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yh.jianghongdianzi.cn

[S14] C：枚举
来源：http://bs.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://nh.huixiangedu.cn

[S15] C：类型转换
来源：http://ot.lnxyls.cn

(double) a / b
来源：http://mj.nszjky.cn

[S16] C：位操作置位
来源：http://it.hahajie.cn

x |= (1 << 3);
来源：http://in.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://gf.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ts.shxzukj.cn

[S18] C：命令行参数
来源：http://ij.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://xz.huanxung.cn

[S19] C：快速排序
来源：http://gl.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zu.panjiajie.cn

[S20] C：二分查找
来源：http://fr.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qd.huanxung.cn

[S21] C：字符类别判断
来源：http://vo.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ng.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://uv.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vs.521024.cn

[S23] C：随机数
来源：http://po.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ir.newstarts.cn

[S24] C：获取本地时间
来源：http://mz.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rd.hahajie.cn

[S25] C：内存拷贝
来源：http://ju.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://tk.wgjwhj.cn

[S26] C：内存清零
来源：http://zk.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://wg.nszjky.cn

[S27] C：定义常量
来源：http://hf.9csxet.cn

const double PI = 3.14159;
来源：http://mo.newstarts.cn

[S28] C：静态变量
来源：http://ea.yuexingan06.cn

static int counter = 0;
来源：http://qa.nszjky.cn

[S29] C：变参函数
来源：http://wx.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://et.chemitech.net.cn

[S30] C：头文件保护
来源：http://dm.szsharing.cn

#ifndef X_H
来源：http://ie.hnjuh.cn

#define X_H
来源：http://fj.521024.cn

#endif
来源：http://ml.shxzskj.cn

[S31] C++：Hello World
来源：http://hb.shxzskj.cn

#include <iostream>
来源：http://ow.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ba.szxytkj.cn

[S32] C++：字符串
来源：http://pf.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://ne.shtwfgs.cn

[S33] C++：vector 增删
来源：http://zr.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mv.9csxet.cn

[S34] C++：遍历 vector
来源：http://es.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://jp.szsharing.cn

[S35] C++：map
来源：http://zl.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jd.yuexingan06.cn

[S36] C++：unordered_map
来源：http://fh.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dy.huanxung.cn

[S37] C++：set
来源：http://si.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xk.gzmigu.cn

[S38] C++：排序
来源：http://ic.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://sm.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://fi.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qj.asd995.cn

[S40] C++：查找元素
来源：http://rq.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ha.521024.cn

[S41] C++：类与构造函数
来源：http://sa.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sn.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://mp.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://mh.szxytkj.cn

[S43] C++：智能指针
来源：http://sr.521024.cn

auto p = std::make_unique<int>(5);
来源：http://mu.gzmigu.cn

[S44] C++：引用传参
来源：http://ti.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://rv.nszjky.cn

[S45] C++：lambda
来源：http://vz.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yd.521024.cn

[S46] C++：函数模板
来源：http://le.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://na.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://wa.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ca.shxzskj.cn

[S48] C++：逐行读文件
来源：http://pj.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ae.colortex.cn

while (std::getline(in, line)) { }
来源：http://ow.shtwfgs.cn

[S49] C++：写文件
来源：http://gm.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pd.shxzskj.cn

[S50] C++：格式化数字
来源：http://xr.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aw.huanxung.cn

[S51] C++：显式类型转换
来源：http://lg.bjjhwx.cn

static_cast<double>(a) / b
来源：http://te.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://wz.nszjky.cn

int size() const noexcept { return n_; }
来源：http://vh.panjiajie.cn

[S53] C++：移动语义
来源：http://fd.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://vm.nicolike.cn

[S54] C++：异常处理
来源：http://bo.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qu.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://vm.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rm.jianghongdianzi.cn

[S56] C++：optional
来源：http://qh.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sd.wgjwhj.cn

[S57] C++：编译期常量
来源：http://ml.bookmarksfly.cn

constexpr int N = 10;
来源：http://hd.bookmarksfly.cn

[S58] C++：命名空间
来源：http://mg.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://zj.huixiangedu.cn

[S59] C++：静态断言
来源：http://me.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fj.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://he.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ej.shxzukj.cn

================================================================================
来源：http://tr.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jf.huixinmuqiang.cn

================================================================================
来源：http://hz.nicolike.cn

[T01] Kotlin：Hello World
来源：http://pn.wgjwhj.cn

println("Hello")
来源：http://kp.nicolike.cn

[T02] Kotlin：变量
来源：http://li.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yg.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://pr.shxzskj.cn

"值: $b"
来源：http://fr.hnjuh.cn

[T04] Kotlin：空安全
来源：http://rk.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://dj.huixinmuqiang.cn


<!-- 参考信息 -->