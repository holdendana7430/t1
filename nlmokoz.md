代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fl.bjjhwx.cn

[Q90] 生成序号列
来源：http://ra.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ih.shtwfgs.cn

================================================================================
来源：http://di.huanxung.cn

R. Bash 专题
来源：http://qh.huanxung.cn

================================================================================
来源：http://uz.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://gi.bjjhwx.cn

#!/usr/bin/env bash
来源：http://aa.huixinmuqiang.cn

set -euo pipefail
来源：http://kb.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://nc.hahajie.cn

name="Tom"; echo "$name"
来源：http://cu.nszjky.cn

[R03] 只读变量
来源：http://er.huixinmuqiang.cn

readonly PI=3.14
来源：http://vy.yuexingan06.cn

[R04] 位置参数
来源：http://zm.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cn.gzmigu.cn

[R05] 参数默认值
来源：http://db.panjiajie.cn

name="${1:-default}"
来源：http://fq.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://bl.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vr.huixiangedu.cn

[R07] if 判断文件
来源：http://lz.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ak.shtwfgs.cn

[R08] 数值比较
来源：http://og.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ri.huixiangedu.cn

[R09] 字符串比较
来源：http://cr.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pq.colortex.cn

[R10] 正则匹配
来源：http://sx.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yy.nicolike.cn

[R11] case 多分支
来源：http://px.bjjhwx.cn

case "$1" in
来源：http://ix.yuexingan06.cn

start) echo "启动" ;;
来源：http://jq.nicolike.cn

stop)  echo "停止" ;;
来源：http://ic.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://yx.asd995.cn

esac
来源：http://ed.gzmigu.cn

[R12] for 遍历文件
来源：http://gb.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://ey.nszjky.cn

[R13] for 计数循环
来源：http://pv.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://dh.panjiajie.cn

[R14] C 风格 for
来源：http://eu.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ol.shtwfgs.cn

[R15] while 逐行读文件
来源：http://ub.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kw.yuntaijiaju.cn

[R16] until 等待条件
来源：http://hx.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zt.szxytkj.cn

[R17] 数组定义与取值
来源：http://fi.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fh.yuexingan06.cn

[R18] 遍历数组
来源：http://ma.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yj.521024.cn

[R19] 数组长度
来源：http://mj.wgjwhj.cn

echo "${#arr[@]}"
来源：http://vd.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://fg.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rk.szsharing.cn

[R21] 字符串长度
来源：http://gk.nszjky.cn

echo "${#s}"
来源：http://oe.szxytkj.cn

[R22] 截取子串
来源：http://vv.521024.cn

echo "${s:0:5}"
来源：http://zg.jianghongdianzi.cn

[R23] 字符串替换
来源：http://dc.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pl.yuntaijiaju.cn

[R24] 大小写转换
来源：http://ju.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sw.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://hq.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://as.jianghongdianzi.cn

[R26] 命令替换
来源：http://hf.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://rg.asd995.cn

[R27] 算术展开
来源：http://wx.nszjky.cn

echo $((1 + 2 * 3))
来源：http://od.gzmigu.cn

[R28] 浮点运算
来源：http://xe.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://cl.shxzukj.cn

[R29] 定义函数
来源：http://yp.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ke.haigaiapp.cn

[R30] 函数返回状态码
来源：http://rk.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://hq.yuntaijiaju.cn

[R31] 局部变量
来源：http://xh.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://hy.hnjuh.cn

[R32] 参数个数校验
来源：http://ks.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mc.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://wk.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fn.lnxyls.cn

[R34] 退出时清理
来源：http://ym.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rj.szxytkj.cn

[R35] 后台执行并等待
来源：http://sb.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xd.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://ay.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ll.newstarts.cn

[R37] 把输出赋给变量
来源：http://rv.colortex.cn

files=$(ls -1)
来源：http://nx.bjjhwx.cn

[R38] 管道串联
来源：http://er.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://ab.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://ek.panjiajie.cn

cmd > out.log 2>&1
来源：http://cn.nszjky.cn

[R40] 追加写日志
来源：http://ch.chemitech.net.cn

echo "log" >> out.log
来源：http://ty.9csxet.cn

[R41] 丢弃输出
来源：http://wg.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://vt.9csxet.cn

[R42] 输入重定向
来源：http://vh.shtwfgs.cn

wc -l < a.txt
来源：http://sl.gzmigu.cn

[R43] 按名字查找文件
来源：http://tq.nszjky.cn

find . -name "*.log" -type f
来源：http://yp.521024.cn

[R44] 按修改时间查找
来源：http://zl.szsharing.cn

find . -mtime -7 -type f
来源：http://qf.shtwfgs.cn

[R45] 批量删除
来源：http://qu.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://na.colortex.cn

[R46] 递归替换文件内容
来源：http://cd.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hc.szsharing.cn

[R47] sed 单行替换
来源：http://bt.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dh.szxytkj.cn

[R48] awk 取指定列
来源：http://gg.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://rk.colortex.cn

[R49] awk 带条件
来源：http://mc.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qm.huixiangedu.cn

[R50] awk 求和
来源：http://vb.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qc.asd995.cn

[R51] 排序去重取前几
来源：http://op.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fn.newstarts.cn

[R52] 统计行数
来源：http://kf.wgjwhj.cn

wc -l a.txt
来源：http://qe.521024.cn

[R53] 查看文件头与实时尾
来源：http://ij.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jc.jctech888.com.cn

[R54] 比较两个文件
来源：http://lt.gzmigu.cn

diff a.txt b.txt
来源：http://qj.colortex.cn

[R55] 压缩与解压
来源：http://in.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jd.gzmigu.cn

[R56] 远程拷贝
来源：http://su.panjiajie.cn

scp file user@host:/path/
来源：http://qe.newstarts.cn

[R57] 远程执行命令
来源：http://gi.hnjuh.cn

ssh user@host 'uptime'
来源：http://sd.huixinmuqiang.cn

[R58] 下载文件
来源：http://qh.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ul.panjiajie.cn

[R59] 发 POST JSON
来源：http://ut.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sk.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://zj.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kq.shxzskj.cn

[R61] 磁盘占用
来源：http://fs.muxihuayi.cn

df -h;  du -sh *
来源：http://th.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://em.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://jv.haigaiapp.cn

[R63] 内存与进程
来源：http://ep.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://im.yuntaijiaju.cn

[R64] 结束进程
来源：http://qs.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://eg.yuexingan06.cn

[R65] 查看端口占用
来源：http://ot.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rw.shxzskj.cn

[R66] 定时任务
来源：http://gf.wgjwhj.cn

crontab -e;  crontab -l
来源：http://oc.newstarts.cn

[R67] 生成随机十六进制串
来源：http://pr.panjiajie.cn

openssl rand -hex 16
来源：http://pv.lnxyls.cn

[R68] 计算文件校验值
来源：http://ad.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://su.yuexingan06.cn

[R69] 生成随机密码
来源：http://rj.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://hx.shtwfgs.cn

[R70] 时间戳与互转
来源：http://pw.hahajie.cn

date +%s;  date -d @1700000000
来源：http://yt.panjiajie.cn

[R71] 日期格式化
来源：http://tv.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vz.gzmigu.cn

[R72] 等待端口就绪
来源：http://lv.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pb.panjiajie.cn

[R73] 分割大日志
来源：http://lh.szsharing.cn

split -l 1000 big.log part_
来源：http://eh.hnjuh.cn

[R74] 批量重命名
来源：http://ip.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ro.chemitech.net.cn

[R75] 导出环境变量
来源：http://ug.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://xl.9csxet.cn

[R76] 使用临时文件
来源：http://cy.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fy.huixiangedu.cn

[R77] 读取用户输入
来源：http://mo.gzmigu.cn

read -rp "请输入: " ans
来源：http://vu.gzmigu.cn

[R78] 交互式菜单
来源：http://wy.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xi.panjiajie.cn

[R79] 解析命令行选项
来源：http://ao.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://it.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://dz.hahajie.cn

time ./run.sh
来源：http://vm.chemitech.net.cn

================================================================================
来源：http://dr.szxytkj.cn

S. C / C++ 专题
来源：http://ii.jctech888.com.cn

================================================================================
来源：http://xf.jianghongdianzi.cn

[S01] C：Hello World
来源：http://sl.muxihuayi.cn

#include <stdio.h>
来源：http://ek.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ju.nicolike.cn

[S02] C：变量与格式化输出
来源：http://vb.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://mk.lnxyls.cn

[S03] C：读入整数
来源：http://io.lnxyls.cn

int x; scanf("%d", &x);
来源：http://he.chemitech.net.cn

[S04] C：字符串复制
来源：http://jx.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wz.shxzukj.cn

[S05] C：字符串长度
来源：http://go.panjiajie.cn

strlen(s)
来源：http://cw.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://ea.lnxyls.cn

strcmp(a, b) == 0
来源：http://me.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://jr.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wl.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://xr.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cd.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://av.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nd.bjjhwx.cn

[S10] C：指针与解引用
来源：http://hh.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://lc.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://sh.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://co.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vy.colortex.cn

fclose(f);
来源：http://hf.panjiajie.cn

[S12] C：写文件
来源：http://ao.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://np.9csxet.cn

[S13] C：宏定义
来源：http://dt.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sx.haigaiapp.cn

[S14] C：枚举
来源：http://ef.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ln.huanxung.cn

[S15] C：类型转换
来源：http://ih.huixinmuqiang.cn

(double) a / b
来源：http://nl.panjiajie.cn

[S16] C：位操作置位
来源：http://ar.panjiajie.cn

x |= (1 << 3);
来源：http://nf.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://xu.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aw.chemitech.net.cn

[S18] C：命令行参数
来源：http://pf.wgjwhj.cn

int main(int argc, char **argv)
来源：http://dn.shxzukj.cn

[S19] C：快速排序
来源：http://mv.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ms.huixinmuqiang.cn

[S20] C：二分查找
来源：http://br.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sc.nicolike.cn

[S21] C：字符类别判断
来源：http://sp.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nm.huixiangedu.cn

[S22] C：字符串转数字
来源：http://wu.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qw.hahajie.cn

[S23] C：随机数
来源：http://ux.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rh.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://ke.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mr.muxihuayi.cn

[S25] C：内存拷贝
来源：http://es.szxytkj.cn

memcpy(dst, src, n);
来源：http://oo.huanxung.cn

[S26] C：内存清零
来源：http://kn.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://zd.shtwfgs.cn

[S27] C：定义常量
来源：http://ju.gzmigu.cn

const double PI = 3.14159;
来源：http://ja.newstarts.cn

[S28] C：静态变量
来源：http://xs.huixiangedu.cn

static int counter = 0;
来源：http://cd.9csxet.cn

[S29] C：变参函数
来源：http://on.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vl.jctech888.com.cn

[S30] C：头文件保护
来源：http://wa.huixiangedu.cn

#ifndef X_H
来源：http://pd.shxzskj.cn

#define X_H
来源：http://xt.asd995.cn

#endif
来源：http://lj.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://ui.yuexingan06.cn

#include <iostream>
来源：http://jv.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://uy.jianghongdianzi.cn

[S32] C++：字符串
来源：http://dd.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://up.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://bq.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jp.521024.cn

[S34] C++：遍历 vector
来源：http://jv.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://sj.huixinmuqiang.cn

[S35] C++：map
来源：http://pg.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ee.bjjhwx.cn

[S36] C++：unordered_map
来源：http://hf.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gm.huixinmuqiang.cn

[S37] C++：set
来源：http://bs.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qm.szsharing.cn

[S38] C++：排序
来源：http://yu.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://rd.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://lk.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vq.bookmarksfly.cn

[S40] C++：查找元素
来源：http://ws.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xw.szsharing.cn

[S41] C++：类与构造函数
来源：http://df.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nw.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://fw.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://af.panjiajie.cn

[S43] C++：智能指针
来源：http://wb.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://py.shtwfgs.cn

[S44] C++：引用传参
来源：http://jg.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://ik.gzmigu.cn

[S45] C++：lambda
来源：http://fd.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zn.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://kn.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://km.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://ou.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ur.shxzskj.cn

[S48] C++：逐行读文件
来源：http://ul.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://av.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://ph.shxzskj.cn

[S49] C++：写文件
来源：http://zt.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://em.szxytkj.cn

[S50] C++：格式化数字
来源：http://my.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gz.nicolike.cn

[S51] C++：显式类型转换
来源：http://xb.szsharing.cn

static_cast<double>(a) / b
来源：http://iv.asd995.cn

[S52] C++：const 与 noexcept
来源：http://tu.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://ft.bjjhwx.cn

[S53] C++：移动语义
来源：http://bt.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://hv.bjjhwx.cn

[S54] C++：异常处理
来源：http://fa.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wl.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://ds.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xc.szsharing.cn

[S56] C++：optional
来源：http://yv.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iu.shxzukj.cn

[S57] C++：编译期常量
来源：http://ef.bookmarksfly.cn

constexpr int N = 10;
来源：http://wd.hahajie.cn

[S58] C++：命名空间
来源：http://us.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://nz.nszjky.cn

[S59] C++：静态断言
来源：http://xd.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://on.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://ys.chemitech.net.cn


<!-- 参考信息 -->