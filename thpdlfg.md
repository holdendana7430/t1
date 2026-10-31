代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://tl.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ir.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://is.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://tb.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wk.panjiajie.cn

[Q90] 生成序号列
来源：http://wy.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fi.jianghongdianzi.cn

================================================================================
来源：http://nm.9csxet.cn

R. Bash 专题
来源：http://bh.jianghongdianzi.cn

================================================================================
来源：http://fi.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://hs.yuexingan06.cn

#!/usr/bin/env bash
来源：http://pl.shxzskj.cn

set -euo pipefail
来源：http://fg.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://lv.hahajie.cn

name="Tom"; echo "$name"
来源：http://iq.yuexingan06.cn

[R03] 只读变量
来源：http://nz.haigaiapp.cn

readonly PI=3.14
来源：http://ci.gzmigu.cn

[R04] 位置参数
来源：http://qm.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://by.jctech888.com.cn

[R05] 参数默认值
来源：http://pb.szsharing.cn

name="${1:-default}"
来源：http://nu.gzmigu.cn

[R06] 判断命令是否存在
来源：http://hm.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xn.asd995.cn

[R07] if 判断文件
来源：http://tv.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ou.chemitech.net.cn

[R08] 数值比较
来源：http://fh.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gw.shxzskj.cn

[R09] 字符串比较
来源：http://pn.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ev.panjiajie.cn

[R10] 正则匹配
来源：http://pg.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kw.colortex.cn

[R11] case 多分支
来源：http://rw.shtwfgs.cn

case "$1" in
来源：http://yn.hahajie.cn

start) echo "启动" ;;
来源：http://lt.newstarts.cn

stop)  echo "停止" ;;
来源：http://nn.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://yn.shtwfgs.cn

esac
来源：http://iy.asd995.cn

[R12] for 遍历文件
来源：http://tk.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://rm.shxzskj.cn

[R13] for 计数循环
来源：http://zb.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://rx.colortex.cn

[R14] C 风格 for
来源：http://ro.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qf.newstarts.cn

[R15] while 逐行读文件
来源：http://oe.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dy.newstarts.cn

[R16] until 等待条件
来源：http://bk.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vw.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://fo.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rx.lnxyls.cn

[R18] 遍历数组
来源：http://dn.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cz.haigaiapp.cn

[R19] 数组长度
来源：http://jk.chemitech.net.cn

echo "${#arr[@]}"
来源：http://bg.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://vj.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ky.shxzukj.cn

[R21] 字符串长度
来源：http://xx.bookmarksfly.cn

echo "${#s}"
来源：http://tl.yuexingan06.cn

[R22] 截取子串
来源：http://xy.panjiajie.cn

echo "${s:0:5}"
来源：http://nw.huixiangedu.cn

[R23] 字符串替换
来源：http://ig.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gl.colortex.cn

[R24] 大小写转换
来源：http://ts.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://st.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://hk.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oa.shxzskj.cn

[R26] 命令替换
来源：http://kv.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://ca.gzmigu.cn

[R27] 算术展开
来源：http://ii.9csxet.cn

echo $((1 + 2 * 3))
来源：http://zn.gzmigu.cn

[R28] 浮点运算
来源：http://md.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://cr.huixiangedu.cn

[R29] 定义函数
来源：http://mb.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://do.shxzukj.cn

[R30] 函数返回状态码
来源：http://qm.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://tt.muxihuayi.cn

[R31] 局部变量
来源：http://ae.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://an.shtwfgs.cn

[R32] 参数个数校验
来源：http://vl.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ud.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://bl.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ik.shxzukj.cn

[R34] 退出时清理
来源：http://cd.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qt.yuexingan06.cn

[R35] 后台执行并等待
来源：http://yu.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zd.hahajie.cn

[R36] 并发执行多个任务
来源：http://yk.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ox.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://vm.haigaiapp.cn

files=$(ls -1)
来源：http://yu.shxzukj.cn

[R38] 管道串联
来源：http://bk.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://td.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://bw.colortex.cn

cmd > out.log 2>&1
来源：http://gb.wgjwhj.cn

[R40] 追加写日志
来源：http://uj.chemitech.net.cn

echo "log" >> out.log
来源：http://sh.nicolike.cn

[R41] 丢弃输出
来源：http://ec.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://ac.muxihuayi.cn

[R42] 输入重定向
来源：http://mu.shxzskj.cn

wc -l < a.txt
来源：http://xb.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://ow.yuexingan06.cn

find . -name "*.log" -type f
来源：http://he.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://nm.nszjky.cn

find . -mtime -7 -type f
来源：http://dp.gzmigu.cn

[R45] 批量删除
来源：http://mv.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://jk.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://bm.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hb.nszjky.cn

[R47] sed 单行替换
来源：http://cb.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://he.lnxyls.cn

[R48] awk 取指定列
来源：http://uj.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://mo.asd995.cn

[R49] awk 带条件
来源：http://qj.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://su.shxzskj.cn

[R50] awk 求和
来源：http://be.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ac.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://wv.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vs.9csxet.cn

[R52] 统计行数
来源：http://iz.newstarts.cn

wc -l a.txt
来源：http://dr.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://ie.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xh.asd995.cn

[R54] 比较两个文件
来源：http://zx.szsharing.cn

diff a.txt b.txt
来源：http://ly.huixiangedu.cn

[R55] 压缩与解压
来源：http://sy.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yh.chemitech.net.cn

[R56] 远程拷贝
来源：http://ed.wgjwhj.cn

scp file user@host:/path/
来源：http://zb.jctech888.com.cn

[R57] 远程执行命令
来源：http://kg.newstarts.cn

ssh user@host 'uptime'
来源：http://dl.colortex.cn

[R58] 下载文件
来源：http://kt.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zk.chemitech.net.cn

[R59] 发 POST JSON
来源：http://dz.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cl.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://jj.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nc.521024.cn

[R61] 磁盘占用
来源：http://pn.huixinmuqiang.cn

df -h;  du -sh *
来源：http://sx.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://qn.colortex.cn

du -ah . | sort -rh | head -10
来源：http://ws.lnxyls.cn

[R63] 内存与进程
来源：http://dt.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://tq.panjiajie.cn

[R64] 结束进程
来源：http://ae.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://ob.nicolike.cn

[R65] 查看端口占用
来源：http://aq.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gl.huixiangedu.cn

[R66] 定时任务
来源：http://uj.haigaiapp.cn

crontab -e;  crontab -l
来源：http://ds.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://id.haigaiapp.cn

openssl rand -hex 16
来源：http://wc.panjiajie.cn

[R68] 计算文件校验值
来源：http://hq.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://co.lnxyls.cn

[R69] 生成随机密码
来源：http://tc.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://uk.nicolike.cn

[R70] 时间戳与互转
来源：http://bz.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://ws.colortex.cn

[R71] 日期格式化
来源：http://bd.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ac.shxzskj.cn

[R72] 等待端口就绪
来源：http://zs.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ot.colortex.cn

[R73] 分割大日志
来源：http://zx.shtwfgs.cn

split -l 1000 big.log part_
来源：http://yx.gzmigu.cn

[R74] 批量重命名
来源：http://ia.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sh.newstarts.cn

[R75] 导出环境变量
来源：http://fe.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://kt.asd995.cn

[R76] 使用临时文件
来源：http://nu.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ge.huixiangedu.cn

[R77] 读取用户输入
来源：http://ig.colortex.cn

read -rp "请输入: " ans
来源：http://vr.panjiajie.cn

[R78] 交互式菜单
来源：http://jt.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://at.yuexingan06.cn

[R79] 解析命令行选项
来源：http://iq.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ln.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://mg.newstarts.cn

time ./run.sh
来源：http://ib.hahajie.cn

================================================================================
来源：http://pu.wgjwhj.cn

S. C / C++ 专题
来源：http://av.nicolike.cn

================================================================================
来源：http://el.asd995.cn

[S01] C：Hello World
来源：http://cw.szxytkj.cn

#include <stdio.h>
来源：http://ac.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tr.huanxung.cn

[S02] C：变量与格式化输出
来源：http://qx.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://zi.bjjhwx.cn

[S03] C：读入整数
来源：http://ty.521024.cn

int x; scanf("%d", &x);
来源：http://vg.chemitech.net.cn

[S04] C：字符串复制
来源：http://oh.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nk.chemitech.net.cn

[S05] C：字符串长度
来源：http://yf.szsharing.cn

strlen(s)
来源：http://dq.huanxung.cn

[S06] C：字符串比较
来源：http://gm.yuexingan06.cn

strcmp(a, b) == 0
来源：http://pg.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://eo.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://td.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://uo.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ty.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://qb.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ha.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://co.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://vi.newstarts.cn

[S11] C：逐行读文件
来源：http://wa.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://iy.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zi.szxytkj.cn

fclose(f);
来源：http://by.haigaiapp.cn

[S12] C：写文件
来源：http://pf.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ws.9csxet.cn

[S13] C：宏定义
来源：http://ds.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vd.nszjky.cn

[S14] C：枚举
来源：http://vn.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://eo.9csxet.cn

[S15] C：类型转换
来源：http://ut.szxytkj.cn

(double) a / b
来源：http://za.shtwfgs.cn

[S16] C：位操作置位
来源：http://rt.chemitech.net.cn

x |= (1 << 3);
来源：http://gb.colortex.cn

[S17] C：安全拼接字符串
来源：http://dk.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hi.shxzskj.cn

[S18] C：命令行参数
来源：http://we.muxihuayi.cn

int main(int argc, char **argv)
来源：http://ue.yuexingan06.cn

[S19] C：快速排序
来源：http://es.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vv.haigaiapp.cn

[S20] C：二分查找
来源：http://jw.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fe.chemitech.net.cn

[S21] C：字符类别判断
来源：http://zz.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gq.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://hn.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lt.newstarts.cn

[S23] C：随机数
来源：http://rg.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hd.chemitech.net.cn

[S24] C：获取本地时间
来源：http://mr.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bc.szsharing.cn

[S25] C：内存拷贝
来源：http://sk.nszjky.cn

memcpy(dst, src, n);
来源：http://lg.bjjhwx.cn

[S26] C：内存清零
来源：http://mg.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://fb.shxzukj.cn

[S27] C：定义常量
来源：http://vm.haigaiapp.cn

const double PI = 3.14159;
来源：http://kg.wgjwhj.cn

[S28] C：静态变量
来源：http://wx.9csxet.cn

static int counter = 0;
来源：http://qm.szxytkj.cn

[S29] C：变参函数
来源：http://fs.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ko.szsharing.cn

[S30] C：头文件保护
来源：http://gb.jctech888.com.cn

#ifndef X_H
来源：http://gj.yuexingan06.cn

#define X_H
来源：http://qu.chemitech.net.cn

#endif
来源：http://ni.asd995.cn

[S31] C++：Hello World
来源：http://gc.muxihuayi.cn

#include <iostream>
来源：http://vc.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://sm.shxzukj.cn

[S32] C++：字符串
来源：http://ze.asd995.cn

std::string s = "hi";  s += "!";
来源：http://ab.gzmigu.cn

[S33] C++：vector 增删
来源：http://lr.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yo.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://cm.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://ck.nszjky.cn

[S35] C++：map
来源：http://go.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zu.szsharing.cn

[S36] C++：unordered_map
来源：http://is.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bi.gzmigu.cn

[S37] C++：set
来源：http://aw.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://no.panjiajie.cn

[S38] C++：排序
来源：http://ic.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://na.521024.cn

[S39] C++：自定义比较器排序
来源：http://io.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bu.shxzskj.cn

[S40] C++：查找元素
来源：http://xl.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ml.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://gc.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wd.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://bb.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://dn.newstarts.cn

[S43] C++：智能指针
来源：http://en.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://ny.haigaiapp.cn

[S44] C++：引用传参
来源：http://rt.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://dr.jianghongdianzi.cn

[S45] C++：lambda
来源：http://os.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lc.szxytkj.cn

[S46] C++：函数模板
来源：http://oy.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yr.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://di.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ey.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://yy.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fi.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://al.shxzskj.cn

[S49] C++：写文件
来源：http://bk.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fa.huanxung.cn

[S50] C++：格式化数字
来源：http://jc.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jb.hahajie.cn

[S51] C++：显式类型转换
来源：http://kl.bjjhwx.cn

static_cast<double>(a) / b
来源：http://wq.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://qm.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://fz.jctech888.com.cn

[S53] C++：移动语义
来源：http://rw.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://lf.521024.cn

[S54] C++：异常处理
来源：http://mj.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tt.szxytkj.cn

[S55] C++：结构化绑定
来源：http://kx.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vk.newstarts.cn

[S56] C++：optional
来源：http://yl.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kh.nszjky.cn

[S57] C++：编译期常量
来源：http://kt.panjiajie.cn

constexpr int N = 10;
来源：http://ph.wgjwhj.cn

[S58] C++：命名空间
来源：http://fd.jianghongdianzi.cn


<!-- 参考信息 -->