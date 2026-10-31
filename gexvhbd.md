代发 wailian999

R. Bash 专题
来源：http://jn.9csxet.cn

================================================================================
来源：http://vr.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://gi.lnxyls.cn

#!/usr/bin/env bash
来源：http://es.shxzskj.cn

set -euo pipefail
来源：http://jg.gzmigu.cn

[R02] 变量赋值与使用
来源：http://qw.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://vn.jianghongdianzi.cn

[R03] 只读变量
来源：http://xn.panjiajie.cn

readonly PI=3.14
来源：http://vs.newstarts.cn

[R04] 位置参数
来源：http://nt.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jo.jianghongdianzi.cn

[R05] 参数默认值
来源：http://bs.huanxung.cn

name="${1:-default}"
来源：http://tb.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://em.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bk.hahajie.cn

[R07] if 判断文件
来源：http://ha.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bq.asd995.cn

[R08] 数值比较
来源：http://df.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ue.lnxyls.cn

[R09] 字符串比较
来源：http://pd.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tn.nszjky.cn

[R10] 正则匹配
来源：http://zt.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rw.newstarts.cn

[R11] case 多分支
来源：http://wm.shtwfgs.cn

case "$1" in
来源：http://cf.wgjwhj.cn

start) echo "启动" ;;
来源：http://po.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://vr.hahajie.cn

*)     echo "未知命令" ;;
来源：http://xx.nicolike.cn

esac
来源：http://ji.nicolike.cn

[R12] for 遍历文件
来源：http://un.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://tj.hahajie.cn

[R13] for 计数循环
来源：http://qj.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://hy.haigaiapp.cn

[R14] C 风格 for
来源：http://wl.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lo.muxihuayi.cn

[R15] while 逐行读文件
来源：http://og.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mh.chemitech.net.cn

[R16] until 等待条件
来源：http://mz.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gb.panjiajie.cn

[R17] 数组定义与取值
来源：http://pm.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gs.huixinmuqiang.cn

[R18] 遍历数组
来源：http://ux.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yb.szxytkj.cn

[R19] 数组长度
来源：http://at.szxytkj.cn

echo "${#arr[@]}"
来源：http://af.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://qv.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qt.panjiajie.cn

[R21] 字符串长度
来源：http://kd.colortex.cn

echo "${#s}"
来源：http://jb.newstarts.cn

[R22] 截取子串
来源：http://cb.bookmarksfly.cn

echo "${s:0:5}"
来源：http://jb.bookmarksfly.cn

[R23] 字符串替换
来源：http://jg.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gq.bookmarksfly.cn

[R24] 大小写转换
来源：http://ne.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pb.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://ds.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rg.shxzskj.cn

[R26] 命令替换
来源：http://zc.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://dn.shxzskj.cn

[R27] 算术展开
来源：http://ka.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://oz.szsharing.cn

[R28] 浮点运算
来源：http://ad.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://bw.bjjhwx.cn

[R29] 定义函数
来源：http://er.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pa.wgjwhj.cn

[R30] 函数返回状态码
来源：http://ul.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://fi.hahajie.cn

[R31] 局部变量
来源：http://pb.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://wv.521024.cn

[R32] 参数个数校验
来源：http://by.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mc.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://mr.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cd.wgjwhj.cn

[R34] 退出时清理
来源：http://az.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://is.shtwfgs.cn

[R35] 后台执行并等待
来源：http://wd.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ee.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://om.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vf.gzmigu.cn

[R37] 把输出赋给变量
来源：http://pc.jctech888.com.cn

files=$(ls -1)
来源：http://el.bookmarksfly.cn

[R38] 管道串联
来源：http://qp.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://tg.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://ax.wgjwhj.cn

cmd > out.log 2>&1
来源：http://ty.gzmigu.cn

[R40] 追加写日志
来源：http://oo.haigaiapp.cn

echo "log" >> out.log
来源：http://ud.szxytkj.cn

[R41] 丢弃输出
来源：http://ng.asd995.cn

cmd >/dev/null 2>&1
来源：http://ef.colortex.cn

[R42] 输入重定向
来源：http://lg.lnxyls.cn

wc -l < a.txt
来源：http://mi.bjjhwx.cn

[R43] 按名字查找文件
来源：http://rb.lnxyls.cn

find . -name "*.log" -type f
来源：http://zb.muxihuayi.cn

[R44] 按修改时间查找
来源：http://yy.huanxung.cn

find . -mtime -7 -type f
来源：http://xl.bjjhwx.cn

[R45] 批量删除
来源：http://jy.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://qj.szxytkj.cn

[R46] 递归替换文件内容
来源：http://ey.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ah.asd995.cn

[R47] sed 单行替换
来源：http://xw.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rw.panjiajie.cn

[R48] awk 取指定列
来源：http://xb.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://dj.yuexingan06.cn

[R49] awk 带条件
来源：http://bz.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sr.gzmigu.cn

[R50] awk 求和
来源：http://hu.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yo.shtwfgs.cn

[R51] 排序去重取前几
来源：http://hu.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pi.hahajie.cn

[R52] 统计行数
来源：http://gj.muxihuayi.cn

wc -l a.txt
来源：http://ci.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://me.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gx.nicolike.cn

[R54] 比较两个文件
来源：http://vx.shtwfgs.cn

diff a.txt b.txt
来源：http://vo.szxytkj.cn

[R55] 压缩与解压
来源：http://dv.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://es.haigaiapp.cn

[R56] 远程拷贝
来源：http://ae.hahajie.cn

scp file user@host:/path/
来源：http://fj.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://wt.shxzskj.cn

ssh user@host 'uptime'
来源：http://nc.jianghongdianzi.cn

[R58] 下载文件
来源：http://zl.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zf.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://si.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cg.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://lm.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iv.colortex.cn

[R61] 磁盘占用
来源：http://bm.shxzukj.cn

df -h;  du -sh *
来源：http://tm.shxzukj.cn

[R62] 找最占空间的文件
来源：http://bf.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://it.shtwfgs.cn

[R63] 内存与进程
来源：http://cd.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://ez.huixinmuqiang.cn

[R64] 结束进程
来源：http://pw.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://dn.huixiangedu.cn

[R65] 查看端口占用
来源：http://km.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rl.szxytkj.cn

[R66] 定时任务
来源：http://yi.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://oo.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://iq.9csxet.cn

openssl rand -hex 16
来源：http://fh.gzmigu.cn

[R68] 计算文件校验值
来源：http://fo.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kw.muxihuayi.cn

[R69] 生成随机密码
来源：http://vr.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://fp.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://mn.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://nv.huixiangedu.cn

[R71] 日期格式化
来源：http://ew.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://aq.nicolike.cn

[R72] 等待端口就绪
来源：http://ti.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ov.bjjhwx.cn

[R73] 分割大日志
来源：http://mo.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://ng.nicolike.cn

[R74] 批量重命名
来源：http://xp.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jt.hahajie.cn

[R75] 导出环境变量
来源：http://ek.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://qo.nszjky.cn

[R76] 使用临时文件
来源：http://in.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hw.shtwfgs.cn

[R77] 读取用户输入
来源：http://nb.shtwfgs.cn

read -rp "请输入: " ans
来源：http://hu.huanxung.cn

[R78] 交互式菜单
来源：http://ac.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tz.asd995.cn

[R79] 解析命令行选项
来源：http://lr.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bz.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://th.yuexingan06.cn

time ./run.sh
来源：http://ot.lnxyls.cn

================================================================================
来源：http://ox.yuntaijiaju.cn

S. C / C++ 专题
来源：http://mg.shxzukj.cn

================================================================================
来源：http://kf.muxihuayi.cn

[S01] C：Hello World
来源：http://ns.gzmigu.cn

#include <stdio.h>
来源：http://lv.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xv.521024.cn

[S02] C：变量与格式化输出
来源：http://zu.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://ny.nszjky.cn

[S03] C：读入整数
来源：http://nm.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://ld.muxihuayi.cn

[S04] C：字符串复制
来源：http://uq.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qt.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://qt.bjjhwx.cn

strlen(s)
来源：http://ih.yuexingan06.cn

[S06] C：字符串比较
来源：http://kx.chemitech.net.cn

strcmp(a, b) == 0
来源：http://gp.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://rk.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://od.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://bs.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rc.521024.cn

[S09] C：结构体定义与初始化
来源：http://th.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pg.haigaiapp.cn

[S10] C：指针与解引用
来源：http://uj.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://id.nszjky.cn

[S11] C：逐行读文件
来源：http://cp.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://ae.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://az.jctech888.com.cn

fclose(f);
来源：http://dh.yuntaijiaju.cn

[S12] C：写文件
来源：http://ky.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fq.chemitech.net.cn

[S13] C：宏定义
来源：http://bo.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://is.szxytkj.cn

[S14] C：枚举
来源：http://tu.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://tu.jctech888.com.cn

[S15] C：类型转换
来源：http://vp.haigaiapp.cn

(double) a / b
来源：http://ps.asd995.cn

[S16] C：位操作置位
来源：http://yl.hnjuh.cn

x |= (1 << 3);
来源：http://iq.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://ya.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jq.panjiajie.cn

[S18] C：命令行参数
来源：http://oo.hnjuh.cn

int main(int argc, char **argv)
来源：http://my.nszjky.cn

[S19] C：快速排序
来源：http://wm.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yu.hahajie.cn

[S20] C：二分查找
来源：http://cx.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qf.lnxyls.cn

[S21] C：字符类别判断
来源：http://lx.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mo.shxzskj.cn

[S22] C：字符串转数字
来源：http://ze.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yw.szxytkj.cn

[S23] C：随机数
来源：http://ls.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wm.yuexingan06.cn

[S24] C：获取本地时间
来源：http://pr.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kw.hahajie.cn

[S25] C：内存拷贝
来源：http://sf.szsharing.cn

memcpy(dst, src, n);
来源：http://yn.huanxung.cn

[S26] C：内存清零
来源：http://fl.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://fv.muxihuayi.cn

[S27] C：定义常量
来源：http://tf.jctech888.com.cn

const double PI = 3.14159;
来源：http://ek.huixiangedu.cn

[S28] C：静态变量
来源：http://iz.gzmigu.cn

static int counter = 0;
来源：http://gz.shxzskj.cn

[S29] C：变参函数
来源：http://ro.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kw.bookmarksfly.cn

[S30] C：头文件保护
来源：http://ah.asd995.cn

#ifndef X_H
来源：http://ji.muxihuayi.cn

#define X_H
来源：http://ks.huixiangedu.cn

#endif
来源：http://bc.bjjhwx.cn

[S31] C++：Hello World
来源：http://ty.shxzskj.cn

#include <iostream>
来源：http://ik.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://sz.9csxet.cn

[S32] C++：字符串
来源：http://ea.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://pu.muxihuayi.cn

[S33] C++：vector 增删
来源：http://rn.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ti.huanxung.cn

[S34] C++：遍历 vector
来源：http://bw.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://io.muxihuayi.cn

[S35] C++：map
来源：http://gh.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ug.9csxet.cn

[S36] C++：unordered_map
来源：http://sp.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rn.huixiangedu.cn

[S37] C++：set
来源：http://dt.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ge.chemitech.net.cn

[S38] C++：排序
来源：http://be.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://wy.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://hh.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qb.shxzukj.cn

[S40] C++：查找元素
来源：http://sh.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ht.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://yl.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kz.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://ov.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://uq.bookmarksfly.cn

[S43] C++：智能指针
来源：http://jw.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://xl.szxytkj.cn

[S44] C++：引用传参
来源：http://dy.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://ws.lnxyls.cn

[S45] C++：lambda
来源：http://fl.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tc.szxytkj.cn

[S46] C++：函数模板
来源：http://zx.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fr.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://sh.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kt.asd995.cn

[S48] C++：逐行读文件
来源：http://dn.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wr.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://jd.yuntaijiaju.cn

[S49] C++：写文件
来源：http://dn.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rn.haigaiapp.cn

[S50] C++：格式化数字
来源：http://de.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rq.shxzukj.cn

[S51] C++：显式类型转换
来源：http://te.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://ay.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://vy.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://xr.lnxyls.cn

[S53] C++：移动语义
来源：http://cw.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://nd.shtwfgs.cn

[S54] C++：异常处理
来源：http://ug.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nk.hnjuh.cn

[S55] C++：结构化绑定
来源：http://hj.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ru.shxzskj.cn

[S56] C++：optional
来源：http://ni.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cy.shxzskj.cn

[S57] C++：编译期常量
来源：http://aq.huixiangedu.cn

constexpr int N = 10;
来源：http://fc.newstarts.cn

[S58] C++：命名空间
来源：http://ew.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://rb.hahajie.cn

[S59] C++：静态断言
来源：http://vc.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kc.colortex.cn

[S60] C++：遍历并删除元素
来源：http://od.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sr.gzmigu.cn

================================================================================
来源：http://zv.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uy.bjjhwx.cn

================================================================================
来源：http://oc.huanxung.cn


<!-- 参考信息 -->