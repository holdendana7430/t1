代发 wailian999

set -euo pipefail
来源：http://nj.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://oe.9csxet.cn

name="Tom"; echo "$name"
来源：http://kl.lnxyls.cn

[R03] 只读变量
来源：http://tq.gzmigu.cn

readonly PI=3.14
来源：http://vw.shxzukj.cn

[R04] 位置参数
来源：http://pj.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zz.nicolike.cn

[R05] 参数默认值
来源：http://nd.szxytkj.cn

name="${1:-default}"
来源：http://ud.szxytkj.cn

[R06] 判断命令是否存在
来源：http://yh.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lb.muxihuayi.cn

[R07] if 判断文件
来源：http://pt.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sl.shxzskj.cn

[R08] 数值比较
来源：http://sk.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nv.jctech888.com.cn

[R09] 字符串比较
来源：http://zs.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://or.jianghongdianzi.cn

[R10] 正则匹配
来源：http://rt.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lk.shxzskj.cn

[R11] case 多分支
来源：http://ba.yuexingan06.cn

case "$1" in
来源：http://lz.wgjwhj.cn

start) echo "启动" ;;
来源：http://rm.colortex.cn

stop)  echo "停止" ;;
来源：http://eb.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://zk.huixiangedu.cn

esac
来源：http://ph.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://ah.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://bg.bookmarksfly.cn

[R13] for 计数循环
来源：http://fw.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://tt.shxzukj.cn

[R14] C 风格 for
来源：http://re.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fz.hahajie.cn

[R15] while 逐行读文件
来源：http://qw.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ff.muxihuayi.cn

[R16] until 等待条件
来源：http://yw.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ly.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://ik.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kh.bjjhwx.cn

[R18] 遍历数组
来源：http://tj.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fv.asd995.cn

[R19] 数组长度
来源：http://hx.muxihuayi.cn

echo "${#arr[@]}"
来源：http://qe.nszjky.cn

[R20] 关联数组（字典）
来源：http://xv.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pr.haigaiapp.cn

[R21] 字符串长度
来源：http://dd.yuntaijiaju.cn

echo "${#s}"
来源：http://wt.gzmigu.cn

[R22] 截取子串
来源：http://lz.shxzskj.cn

echo "${s:0:5}"
来源：http://nq.yuexingan06.cn

[R23] 字符串替换
来源：http://bi.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jx.yuexingan06.cn

[R24] 大小写转换
来源：http://mq.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ew.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://lf.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jh.jctech888.com.cn

[R26] 命令替换
来源：http://jb.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://if.wgjwhj.cn

[R27] 算术展开
来源：http://ih.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://ai.newstarts.cn

[R28] 浮点运算
来源：http://rs.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://bb.nszjky.cn

[R29] 定义函数
来源：http://zv.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vh.haigaiapp.cn

[R30] 函数返回状态码
来源：http://vi.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://nl.bookmarksfly.cn

[R31] 局部变量
来源：http://yw.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://ui.szsharing.cn

[R32] 参数个数校验
来源：http://rz.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://om.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://uh.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dm.hnjuh.cn

[R34] 退出时清理
来源：http://gq.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pu.muxihuayi.cn

[R35] 后台执行并等待
来源：http://ga.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jt.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://qy.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ea.9csxet.cn

[R37] 把输出赋给变量
来源：http://tx.szxytkj.cn

files=$(ls -1)
来源：http://et.huanxung.cn

[R38] 管道串联
来源：http://or.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://eu.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://kv.chemitech.net.cn

cmd > out.log 2>&1
来源：http://lz.panjiajie.cn

[R40] 追加写日志
来源：http://rp.shxzukj.cn

echo "log" >> out.log
来源：http://nk.bookmarksfly.cn

[R41] 丢弃输出
来源：http://gg.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://te.colortex.cn

[R42] 输入重定向
来源：http://yx.shxzukj.cn

wc -l < a.txt
来源：http://ap.szxytkj.cn

[R43] 按名字查找文件
来源：http://nz.szxytkj.cn

find . -name "*.log" -type f
来源：http://hx.9csxet.cn

[R44] 按修改时间查找
来源：http://se.newstarts.cn

find . -mtime -7 -type f
来源：http://nu.bjjhwx.cn

[R45] 批量删除
来源：http://br.newstarts.cn

find . -name "*.tmp" -delete
来源：http://oj.panjiajie.cn

[R46] 递归替换文件内容
来源：http://ly.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cv.colortex.cn

[R47] sed 单行替换
来源：http://ib.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cj.haigaiapp.cn

[R48] awk 取指定列
来源：http://yc.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://ih.nszjky.cn

[R49] awk 带条件
来源：http://ec.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xm.shxzskj.cn

[R50] awk 求和
来源：http://xm.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fx.shtwfgs.cn

[R51] 排序去重取前几
来源：http://sd.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ff.wgjwhj.cn

[R52] 统计行数
来源：http://ot.szsharing.cn

wc -l a.txt
来源：http://pu.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://mk.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://na.huanxung.cn

[R54] 比较两个文件
来源：http://lw.hnjuh.cn

diff a.txt b.txt
来源：http://jn.szsharing.cn

[R55] 压缩与解压
来源：http://yz.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ft.nszjky.cn

[R56] 远程拷贝
来源：http://bx.chemitech.net.cn

scp file user@host:/path/
来源：http://sk.shtwfgs.cn

[R57] 远程执行命令
来源：http://hb.hnjuh.cn

ssh user@host 'uptime'
来源：http://bm.jctech888.com.cn

[R58] 下载文件
来源：http://wm.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ub.hnjuh.cn

[R59] 发 POST JSON
来源：http://qg.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ow.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://yl.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dy.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://of.huixinmuqiang.cn

df -h;  du -sh *
来源：http://xg.panjiajie.cn

[R62] 找最占空间的文件
来源：http://ob.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://vd.9csxet.cn

[R63] 内存与进程
来源：http://lf.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://nu.muxihuayi.cn

[R64] 结束进程
来源：http://vx.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://ja.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://wo.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wy.shtwfgs.cn

[R66] 定时任务
来源：http://ag.shxzskj.cn

crontab -e;  crontab -l
来源：http://zy.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://un.yuntaijiaju.cn

openssl rand -hex 16
来源：http://ip.nicolike.cn

[R68] 计算文件校验值
来源：http://ei.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ob.521024.cn

[R69] 生成随机密码
来源：http://jd.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://ke.nszjky.cn

[R70] 时间戳与互转
来源：http://va.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://an.nszjky.cn

[R71] 日期格式化
来源：http://wh.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oc.gzmigu.cn

[R72] 等待端口就绪
来源：http://zb.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ek.jctech888.com.cn

[R73] 分割大日志
来源：http://zv.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://mh.asd995.cn

[R74] 批量重命名
来源：http://su.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bh.muxihuayi.cn

[R75] 导出环境变量
来源：http://rs.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://kf.shxzskj.cn

[R76] 使用临时文件
来源：http://hi.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fw.chemitech.net.cn

[R77] 读取用户输入
来源：http://cl.lnxyls.cn

read -rp "请输入: " ans
来源：http://hz.gzmigu.cn

[R78] 交互式菜单
来源：http://xc.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://er.chemitech.net.cn

[R79] 解析命令行选项
来源：http://ie.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ep.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://id.bookmarksfly.cn

time ./run.sh
来源：http://rd.huixiangedu.cn

================================================================================
来源：http://zb.jctech888.com.cn

S. C / C++ 专题
来源：http://wl.521024.cn

================================================================================
来源：http://wj.9csxet.cn

[S01] C：Hello World
来源：http://ml.szxytkj.cn

#include <stdio.h>
来源：http://fp.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vw.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://mb.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://tt.gzmigu.cn

[S03] C：读入整数
来源：http://nm.colortex.cn

int x; scanf("%d", &x);
来源：http://ps.hahajie.cn

[S04] C：字符串复制
来源：http://oj.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pp.hnjuh.cn

[S05] C：字符串长度
来源：http://pu.chemitech.net.cn

strlen(s)
来源：http://oe.szsharing.cn

[S06] C：字符串比较
来源：http://qg.haigaiapp.cn

strcmp(a, b) == 0
来源：http://tj.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://yl.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ni.521024.cn

[S08] C：动态内存分配与释放
来源：http://oa.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xh.521024.cn

[S09] C：结构体定义与初始化
来源：http://hw.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nk.gzmigu.cn

[S10] C：指针与解引用
来源：http://yv.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://yk.shxzskj.cn

[S11] C：逐行读文件
来源：http://qy.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://tc.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sn.bjjhwx.cn

fclose(f);
来源：http://yk.newstarts.cn

[S12] C：写文件
来源：http://sy.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uo.shtwfgs.cn

[S13] C：宏定义
来源：http://nc.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ie.haigaiapp.cn

[S14] C：枚举
来源：http://wj.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ni.asd995.cn

[S15] C：类型转换
来源：http://nb.bookmarksfly.cn

(double) a / b
来源：http://gp.nicolike.cn

[S16] C：位操作置位
来源：http://ms.shxzskj.cn

x |= (1 << 3);
来源：http://pm.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://eu.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://el.wgjwhj.cn

[S18] C：命令行参数
来源：http://cn.newstarts.cn

int main(int argc, char **argv)
来源：http://gk.9csxet.cn

[S19] C：快速排序
来源：http://zf.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jd.yuexingan06.cn

[S20] C：二分查找
来源：http://yi.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ly.muxihuayi.cn

[S21] C：字符类别判断
来源：http://yw.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://do.szsharing.cn

[S22] C：字符串转数字
来源：http://uo.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cb.huixiangedu.cn

[S23] C：随机数
来源：http://kp.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fm.huanxung.cn

[S24] C：获取本地时间
来源：http://vm.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yi.bjjhwx.cn

[S25] C：内存拷贝
来源：http://sx.bjjhwx.cn

memcpy(dst, src, n);
来源：http://ds.hnjuh.cn

[S26] C：内存清零
来源：http://ew.huanxung.cn

memset(a, 0, sizeof a);
来源：http://qa.shtwfgs.cn

[S27] C：定义常量
来源：http://ff.shxzskj.cn

const double PI = 3.14159;
来源：http://af.huixinmuqiang.cn

[S28] C：静态变量
来源：http://bt.asd995.cn

static int counter = 0;
来源：http://le.hnjuh.cn

[S29] C：变参函数
来源：http://ri.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ny.521024.cn

[S30] C：头文件保护
来源：http://ho.huixinmuqiang.cn

#ifndef X_H
来源：http://jz.shtwfgs.cn

#define X_H
来源：http://ef.szxytkj.cn

#endif
来源：http://nv.9csxet.cn

[S31] C++：Hello World
来源：http://oz.huixinmuqiang.cn

#include <iostream>
来源：http://kc.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://fl.9csxet.cn

[S32] C++：字符串
来源：http://cm.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://da.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://hq.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ja.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://br.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://oh.szxytkj.cn

[S35] C++：map
来源：http://jb.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://le.colortex.cn

[S36] C++：unordered_map
来源：http://sc.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tw.muxihuayi.cn

[S37] C++：set
来源：http://ep.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qc.nszjky.cn

[S38] C++：排序
来源：http://vg.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://ta.521024.cn

[S39] C++：自定义比较器排序
来源：http://ke.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uk.yuexingan06.cn

[S40] C++：查找元素
来源：http://gf.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://og.szxytkj.cn

[S41] C++：类与构造函数
来源：http://lv.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ou.szsharing.cn

[S42] C++：继承与虚函数
来源：http://fg.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://nv.chemitech.net.cn

[S43] C++：智能指针
来源：http://fu.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://ed.shxzukj.cn

[S44] C++：引用传参
来源：http://ye.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://ko.bjjhwx.cn

[S45] C++：lambda
来源：http://ou.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ws.szxytkj.cn

[S46] C++：函数模板
来源：http://qs.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ey.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://lv.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ln.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://af.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ef.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://bd.bookmarksfly.cn

[S49] C++：写文件
来源：http://mb.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gu.colortex.cn

[S50] C++：格式化数字
来源：http://jn.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://is.nszjky.cn

[S51] C++：显式类型转换
来源：http://wn.szsharing.cn

static_cast<double>(a) / b
来源：http://kk.521024.cn

[S52] C++：const 与 noexcept
来源：http://fb.huanxung.cn

int size() const noexcept { return n_; }
来源：http://nu.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ib.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://vz.panjiajie.cn

[S54] C++：异常处理
来源：http://og.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zz.newstarts.cn

[S55] C++：结构化绑定
来源：http://mx.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rx.panjiajie.cn

[S56] C++：optional
来源：http://wo.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://it.nicolike.cn

[S57] C++：编译期常量
来源：http://vc.panjiajie.cn

constexpr int N = 10;
来源：http://lt.huixiangedu.cn

[S58] C++：命名空间
来源：http://is.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://uh.szxytkj.cn

[S59] C++：静态断言
来源：http://eq.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pf.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://am.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ho.shxzskj.cn

================================================================================
来源：http://cf.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fd.muxihuayi.cn

================================================================================
来源：http://gg.szsharing.cn

[T01] Kotlin：Hello World
来源：http://kp.lnxyls.cn

println("Hello")
来源：http://wr.huixiangedu.cn

[T02] Kotlin：变量
来源：http://vh.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tu.shxzukj.cn


<!-- 参考信息 -->