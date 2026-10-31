代发 wailian999

R. Bash 专题
来源：http://eg.bjjhwx.cn

================================================================================
来源：http://ze.hahajie.cn

[R01] shebang 与严格模式
来源：http://bj.nszjky.cn

#!/usr/bin/env bash
来源：http://ng.nicolike.cn

set -euo pipefail
来源：http://at.hnjuh.cn

[R02] 变量赋值与使用
来源：http://kk.szxytkj.cn

name="Tom"; echo "$name"
来源：http://ev.shtwfgs.cn

[R03] 只读变量
来源：http://qc.chemitech.net.cn

readonly PI=3.14
来源：http://fd.gzmigu.cn

[R04] 位置参数
来源：http://id.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://by.szxytkj.cn

[R05] 参数默认值
来源：http://mu.521024.cn

name="${1:-default}"
来源：http://lx.shxzskj.cn

[R06] 判断命令是否存在
来源：http://wj.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://os.bjjhwx.cn

[R07] if 判断文件
来源：http://hf.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wp.nszjky.cn

[R08] 数值比较
来源：http://xu.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wp.huixiangedu.cn

[R09] 字符串比较
来源：http://qg.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dg.hahajie.cn

[R10] 正则匹配
来源：http://tx.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://su.chemitech.net.cn

[R11] case 多分支
来源：http://ut.huixinmuqiang.cn

case "$1" in
来源：http://an.huixiangedu.cn

start) echo "启动" ;;
来源：http://uf.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://zg.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://lu.szsharing.cn

esac
来源：http://rs.hahajie.cn

[R12] for 遍历文件
来源：http://sc.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://sv.chemitech.net.cn

[R13] for 计数循环
来源：http://ec.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://tx.hnjuh.cn

[R14] C 风格 for
来源：http://mr.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jh.shxzskj.cn

[R15] while 逐行读文件
来源：http://uy.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oo.jianghongdianzi.cn

[R16] until 等待条件
来源：http://kq.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xe.huixiangedu.cn

[R17] 数组定义与取值
来源：http://qj.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://so.wgjwhj.cn

[R18] 遍历数组
来源：http://jq.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vd.muxihuayi.cn

[R19] 数组长度
来源：http://uc.chemitech.net.cn

echo "${#arr[@]}"
来源：http://ex.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://pb.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://df.lnxyls.cn

[R21] 字符串长度
来源：http://iw.shxzukj.cn

echo "${#s}"
来源：http://ml.colortex.cn

[R22] 截取子串
来源：http://jc.yuexingan06.cn

echo "${s:0:5}"
来源：http://db.panjiajie.cn

[R23] 字符串替换
来源：http://xj.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cn.yuexingan06.cn

[R24] 大小写转换
来源：http://hz.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mp.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://jl.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rp.lnxyls.cn

[R26] 命令替换
来源：http://th.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://xg.huixinmuqiang.cn

[R27] 算术展开
来源：http://ks.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://lu.521024.cn

[R28] 浮点运算
来源：http://gi.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://df.shxzskj.cn

[R29] 定义函数
来源：http://bk.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yh.wgjwhj.cn

[R30] 函数返回状态码
来源：http://to.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://jj.huanxung.cn

[R31] 局部变量
来源：http://kk.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://np.521024.cn

[R32] 参数个数校验
来源：http://ed.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ir.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://qx.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pt.gzmigu.cn

[R34] 退出时清理
来源：http://xr.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sm.yuexingan06.cn

[R35] 后台执行并等待
来源：http://nx.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ar.newstarts.cn

[R36] 并发执行多个任务
来源：http://cd.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ua.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://bd.huanxung.cn

files=$(ls -1)
来源：http://dl.szsharing.cn

[R38] 管道串联
来源：http://im.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://cr.colortex.cn

[R39] 重定向标准输出与错误
来源：http://kf.panjiajie.cn

cmd > out.log 2>&1
来源：http://my.jctech888.com.cn

[R40] 追加写日志
来源：http://vw.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ki.huixiangedu.cn

[R41] 丢弃输出
来源：http://jb.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://wq.haigaiapp.cn

[R42] 输入重定向
来源：http://od.gzmigu.cn

wc -l < a.txt
来源：http://nj.9csxet.cn

[R43] 按名字查找文件
来源：http://my.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://fc.lnxyls.cn

[R44] 按修改时间查找
来源：http://ea.szsharing.cn

find . -mtime -7 -type f
来源：http://jr.shxzukj.cn

[R45] 批量删除
来源：http://jz.nicolike.cn

find . -name "*.tmp" -delete
来源：http://nv.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://ux.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yv.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://al.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cy.hahajie.cn

[R48] awk 取指定列
来源：http://qg.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://hp.szxytkj.cn

[R49] awk 带条件
来源：http://rh.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vk.hnjuh.cn

[R50] awk 求和
来源：http://hq.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zk.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://yi.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cl.shxzukj.cn

[R52] 统计行数
来源：http://im.bjjhwx.cn

wc -l a.txt
来源：http://dj.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://hk.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bc.jctech888.com.cn

[R54] 比较两个文件
来源：http://kb.panjiajie.cn

diff a.txt b.txt
来源：http://nl.gzmigu.cn

[R55] 压缩与解压
来源：http://py.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ly.newstarts.cn

[R56] 远程拷贝
来源：http://dg.yuexingan06.cn

scp file user@host:/path/
来源：http://rk.nszjky.cn

[R57] 远程执行命令
来源：http://mj.jctech888.com.cn

ssh user@host 'uptime'
来源：http://qc.yuexingan06.cn

[R58] 下载文件
来源：http://yv.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ib.shxzskj.cn

[R59] 发 POST JSON
来源：http://kr.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lw.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://qh.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hv.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://qb.shtwfgs.cn

df -h;  du -sh *
来源：http://in.panjiajie.cn

[R62] 找最占空间的文件
来源：http://yd.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://iv.shxzskj.cn

[R63] 内存与进程
来源：http://tv.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://na.gzmigu.cn

[R64] 结束进程
来源：http://zc.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://lr.hnjuh.cn

[R65] 查看端口占用
来源：http://vf.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sh.nszjky.cn

[R66] 定时任务
来源：http://nb.huixiangedu.cn

crontab -e;  crontab -l
来源：http://od.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://nm.9csxet.cn

openssl rand -hex 16
来源：http://yo.bjjhwx.cn

[R68] 计算文件校验值
来源：http://vp.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tv.9csxet.cn

[R69] 生成随机密码
来源：http://xf.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://tm.gzmigu.cn

[R70] 时间戳与互转
来源：http://pp.521024.cn

date +%s;  date -d @1700000000
来源：http://us.gzmigu.cn

[R71] 日期格式化
来源：http://sh.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sq.panjiajie.cn

[R72] 等待端口就绪
来源：http://eo.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hv.shxzukj.cn

[R73] 分割大日志
来源：http://ft.nicolike.cn

split -l 1000 big.log part_
来源：http://oo.muxihuayi.cn

[R74] 批量重命名
来源：http://yf.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zn.lnxyls.cn

[R75] 导出环境变量
来源：http://km.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://na.szxytkj.cn

[R76] 使用临时文件
来源：http://cx.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jc.nszjky.cn

[R77] 读取用户输入
来源：http://kl.newstarts.cn

read -rp "请输入: " ans
来源：http://wy.huixiangedu.cn

[R78] 交互式菜单
来源：http://ja.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ue.gzmigu.cn

[R79] 解析命令行选项
来源：http://az.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zn.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://lf.lnxyls.cn

time ./run.sh
来源：http://mf.nszjky.cn

================================================================================
来源：http://az.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ph.huixinmuqiang.cn

================================================================================
来源：http://hk.hahajie.cn

[S01] C：Hello World
来源：http://fc.huixinmuqiang.cn

#include <stdio.h>
来源：http://tf.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xm.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://nl.521024.cn

int a = 10; printf("%d\n", a);
来源：http://tl.newstarts.cn

[S03] C：读入整数
来源：http://gg.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://lr.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://pm.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tx.shxzskj.cn

[S05] C：字符串长度
来源：http://lf.gzmigu.cn

strlen(s)
来源：http://ot.wgjwhj.cn

[S06] C：字符串比较
来源：http://jc.lnxyls.cn

strcmp(a, b) == 0
来源：http://uf.9csxet.cn

[S07] C：数组遍历求和
来源：http://rg.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zn.colortex.cn

[S08] C：动态内存分配与释放
来源：http://pc.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ch.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://gg.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://an.huanxung.cn

[S10] C：指针与解引用
来源：http://ih.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://li.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://vw.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://se.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fx.wgjwhj.cn

fclose(f);
来源：http://os.panjiajie.cn

[S12] C：写文件
来源：http://dd.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://re.shxzskj.cn

[S13] C：宏定义
来源：http://zu.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pl.asd995.cn

[S14] C：枚举
来源：http://tx.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://qr.hahajie.cn

[S15] C：类型转换
来源：http://dr.haigaiapp.cn

(double) a / b
来源：http://we.haigaiapp.cn

[S16] C：位操作置位
来源：http://ro.jianghongdianzi.cn

x |= (1 << 3);
来源：http://qi.hahajie.cn

[S17] C：安全拼接字符串
来源：http://mt.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ms.colortex.cn

[S18] C：命令行参数
来源：http://km.hnjuh.cn

int main(int argc, char **argv)
来源：http://sw.lnxyls.cn

[S19] C：快速排序
来源：http://ng.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://em.hahajie.cn

[S20] C：二分查找
来源：http://ox.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uf.huanxung.cn

[S21] C：字符类别判断
来源：http://pu.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://et.newstarts.cn

[S22] C：字符串转数字
来源：http://ec.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fq.9csxet.cn

[S23] C：随机数
来源：http://ht.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ee.chemitech.net.cn

[S24] C：获取本地时间
来源：http://xc.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jl.huixiangedu.cn

[S25] C：内存拷贝
来源：http://kp.hahajie.cn

memcpy(dst, src, n);
来源：http://hq.yuexingan06.cn

[S26] C：内存清零
来源：http://np.9csxet.cn

memset(a, 0, sizeof a);
来源：http://ey.hahajie.cn

[S27] C：定义常量
来源：http://vo.asd995.cn

const double PI = 3.14159;
来源：http://yo.panjiajie.cn

[S28] C：静态变量
来源：http://po.shxzukj.cn

static int counter = 0;
来源：http://kt.yuntaijiaju.cn

[S29] C：变参函数
来源：http://cz.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yv.muxihuayi.cn

[S30] C：头文件保护
来源：http://ot.shxzskj.cn

#ifndef X_H
来源：http://yy.szxytkj.cn

#define X_H
来源：http://dk.gzmigu.cn

#endif
来源：http://rs.nicolike.cn

[S31] C++：Hello World
来源：http://ei.chemitech.net.cn

#include <iostream>
来源：http://dr.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://sa.muxihuayi.cn

[S32] C++：字符串
来源：http://gi.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://py.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://nr.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mf.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://kd.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ir.yuntaijiaju.cn

[S35] C++：map
来源：http://hd.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fu.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://xt.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yp.nszjky.cn

[S37] C++：set
来源：http://vu.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oj.haigaiapp.cn

[S38] C++：排序
来源：http://dn.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://sz.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://cb.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vt.newstarts.cn

[S40] C++：查找元素
来源：http://ga.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wg.nszjky.cn

[S41] C++：类与构造函数
来源：http://ds.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wn.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://ms.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://em.haigaiapp.cn

[S43] C++：智能指针
来源：http://yh.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://hj.panjiajie.cn

[S44] C++：引用传参
来源：http://wj.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://pe.bjjhwx.cn

[S45] C++：lambda
来源：http://ku.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gm.bjjhwx.cn

[S46] C++：函数模板
来源：http://db.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xj.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://ck.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ju.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://sv.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ck.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://pp.haigaiapp.cn

[S49] C++：写文件
来源：http://un.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iv.panjiajie.cn

[S50] C++：格式化数字
来源：http://xf.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rk.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://jr.colortex.cn

static_cast<double>(a) / b
来源：http://ji.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://li.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://gd.chemitech.net.cn

[S53] C++：移动语义
来源：http://pa.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://eu.521024.cn

[S54] C++：异常处理
来源：http://al.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ir.asd995.cn

[S55] C++：结构化绑定
来源：http://vc.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lo.wgjwhj.cn

[S56] C++：optional
来源：http://bt.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qp.hahajie.cn

[S57] C++：编译期常量
来源：http://ml.jctech888.com.cn

constexpr int N = 10;
来源：http://ta.shtwfgs.cn

[S58] C++：命名空间
来源：http://st.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://xo.colortex.cn

[S59] C++：静态断言
来源：http://hz.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ke.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://zw.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zh.lnxyls.cn

================================================================================
来源：http://ga.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sm.huixiangedu.cn

================================================================================
来源：http://ix.nicolike.cn


<!-- 参考信息 -->