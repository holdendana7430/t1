代发 wailian999

[Q86] 读取 JSON 字段
来源：http://wy.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kk.nszjky.cn

[Q87] JSON 字段做条件
来源：http://nh.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kl.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://hf.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://om.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ex.asd995.cn

[Q89] 判断表是否存在
来源：http://br.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cn.nszjky.cn

[Q90] 生成序号列
来源：http://vt.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xm.yuntaijiaju.cn

================================================================================
来源：http://pd.panjiajie.cn

R. Bash 专题
来源：http://sf.haigaiapp.cn

================================================================================
来源：http://jg.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://zo.jctech888.com.cn

#!/usr/bin/env bash
来源：http://bk.wgjwhj.cn

set -euo pipefail
来源：http://go.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://ri.asd995.cn

name="Tom"; echo "$name"
来源：http://qr.hahajie.cn

[R03] 只读变量
来源：http://xf.colortex.cn

readonly PI=3.14
来源：http://ft.wgjwhj.cn

[R04] 位置参数
来源：http://sw.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uy.huixiangedu.cn

[R05] 参数默认值
来源：http://ba.521024.cn

name="${1:-default}"
来源：http://ev.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://rr.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eo.gzmigu.cn

[R07] if 判断文件
来源：http://yz.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tm.newstarts.cn

[R08] 数值比较
来源：http://ol.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ew.chemitech.net.cn

[R09] 字符串比较
来源：http://ww.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xz.jctech888.com.cn

[R10] 正则匹配
来源：http://vj.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pf.wgjwhj.cn

[R11] case 多分支
来源：http://nk.szxytkj.cn

case "$1" in
来源：http://cn.hnjuh.cn

start) echo "启动" ;;
来源：http://li.gzmigu.cn

stop)  echo "停止" ;;
来源：http://vs.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://jf.bookmarksfly.cn

esac
来源：http://qj.asd995.cn

[R12] for 遍历文件
来源：http://kk.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://yq.huixinmuqiang.cn

[R13] for 计数循环
来源：http://mg.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://de.shtwfgs.cn

[R14] C 风格 for
来源：http://za.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ug.hahajie.cn

[R15] while 逐行读文件
来源：http://pp.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kl.521024.cn

[R16] until 等待条件
来源：http://zy.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sh.asd995.cn

[R17] 数组定义与取值
来源：http://kb.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ry.gzmigu.cn

[R18] 遍历数组
来源：http://lg.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gs.haigaiapp.cn

[R19] 数组长度
来源：http://av.muxihuayi.cn

echo "${#arr[@]}"
来源：http://mv.9csxet.cn

[R20] 关联数组（字典）
来源：http://il.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sq.wgjwhj.cn

[R21] 字符串长度
来源：http://un.szxytkj.cn

echo "${#s}"
来源：http://tj.colortex.cn

[R22] 截取子串
来源：http://mb.9csxet.cn

echo "${s:0:5}"
来源：http://dz.nszjky.cn

[R23] 字符串替换
来源：http://sx.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cj.nszjky.cn

[R24] 大小写转换
来源：http://oo.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kw.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://oe.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ru.gzmigu.cn

[R26] 命令替换
来源：http://yp.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://jk.colortex.cn

[R27] 算术展开
来源：http://cu.huanxung.cn

echo $((1 + 2 * 3))
来源：http://ic.panjiajie.cn

[R28] 浮点运算
来源：http://ot.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://jv.jctech888.com.cn

[R29] 定义函数
来源：http://dm.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ws.hahajie.cn

[R30] 函数返回状态码
来源：http://cj.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://nq.chemitech.net.cn

[R31] 局部变量
来源：http://if.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://mm.panjiajie.cn

[R32] 参数个数校验
来源：http://el.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ao.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://dy.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fx.bookmarksfly.cn

[R34] 退出时清理
来源：http://dg.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wa.huanxung.cn

[R35] 后台执行并等待
来源：http://ap.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dt.shxzukj.cn

[R36] 并发执行多个任务
来源：http://rc.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sv.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://sj.newstarts.cn

files=$(ls -1)
来源：http://fi.yuexingan06.cn

[R38] 管道串联
来源：http://mo.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://hs.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://ku.chemitech.net.cn

cmd > out.log 2>&1
来源：http://jj.huanxung.cn

[R40] 追加写日志
来源：http://bj.wgjwhj.cn

echo "log" >> out.log
来源：http://jx.9csxet.cn

[R41] 丢弃输出
来源：http://zf.nicolike.cn

cmd >/dev/null 2>&1
来源：http://ji.shtwfgs.cn

[R42] 输入重定向
来源：http://qr.colortex.cn

wc -l < a.txt
来源：http://ar.hnjuh.cn

[R43] 按名字查找文件
来源：http://cj.szxytkj.cn

find . -name "*.log" -type f
来源：http://ss.huixiangedu.cn

[R44] 按修改时间查找
来源：http://ip.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://ox.huanxung.cn

[R45] 批量删除
来源：http://vx.nicolike.cn

find . -name "*.tmp" -delete
来源：http://cg.shxzskj.cn

[R46] 递归替换文件内容
来源：http://kt.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://je.newstarts.cn

[R47] sed 单行替换
来源：http://nq.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bk.shtwfgs.cn

[R48] awk 取指定列
来源：http://cb.521024.cn

awk '{print $1, $3}' a.txt
来源：http://po.colortex.cn

[R49] awk 带条件
来源：http://jy.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nl.shxzukj.cn

[R50] awk 求和
来源：http://ap.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ju.bjjhwx.cn

[R51] 排序去重取前几
来源：http://pu.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ye.shxzskj.cn

[R52] 统计行数
来源：http://sg.lnxyls.cn

wc -l a.txt
来源：http://qj.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://vx.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bs.521024.cn

[R54] 比较两个文件
来源：http://im.yuexingan06.cn

diff a.txt b.txt
来源：http://on.newstarts.cn

[R55] 压缩与解压
来源：http://dm.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fq.haigaiapp.cn

[R56] 远程拷贝
来源：http://nt.chemitech.net.cn

scp file user@host:/path/
来源：http://yk.shxzskj.cn

[R57] 远程执行命令
来源：http://qd.huixiangedu.cn

ssh user@host 'uptime'
来源：http://ab.shtwfgs.cn

[R58] 下载文件
来源：http://et.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sg.muxihuayi.cn

[R59] 发 POST JSON
来源：http://ad.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oj.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://eu.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://om.yuexingan06.cn

[R61] 磁盘占用
来源：http://xx.bjjhwx.cn

df -h;  du -sh *
来源：http://wm.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://ex.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://xb.gzmigu.cn

[R63] 内存与进程
来源：http://sx.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://ql.521024.cn

[R64] 结束进程
来源：http://zf.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://wf.shxzskj.cn

[R65] 查看端口占用
来源：http://kc.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lv.colortex.cn

[R66] 定时任务
来源：http://iz.panjiajie.cn

crontab -e;  crontab -l
来源：http://kb.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://bq.huanxung.cn

openssl rand -hex 16
来源：http://nz.yuexingan06.cn

[R68] 计算文件校验值
来源：http://yf.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mf.bjjhwx.cn

[R69] 生成随机密码
来源：http://jc.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://tc.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://du.szsharing.cn

date +%s;  date -d @1700000000
来源：http://uz.muxihuayi.cn

[R71] 日期格式化
来源：http://yp.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fl.yuexingan06.cn

[R72] 等待端口就绪
来源：http://um.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hg.521024.cn

[R73] 分割大日志
来源：http://oz.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://zw.huixiangedu.cn

[R74] 批量重命名
来源：http://zs.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iw.szxytkj.cn

[R75] 导出环境变量
来源：http://ql.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://cs.asd995.cn

[R76] 使用临时文件
来源：http://fl.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nt.jctech888.com.cn

[R77] 读取用户输入
来源：http://ty.bjjhwx.cn

read -rp "请输入: " ans
来源：http://yu.nszjky.cn

[R78] 交互式菜单
来源：http://aq.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ju.shtwfgs.cn

[R79] 解析命令行选项
来源：http://wg.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pr.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://mb.bjjhwx.cn

time ./run.sh
来源：http://ch.colortex.cn

================================================================================
来源：http://kp.lnxyls.cn

S. C / C++ 专题
来源：http://ke.jianghongdianzi.cn

================================================================================
来源：http://mh.lnxyls.cn

[S01] C：Hello World
来源：http://kl.jctech888.com.cn

#include <stdio.h>
来源：http://zp.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ac.nicolike.cn

[S02] C：变量与格式化输出
来源：http://ih.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://nb.hnjuh.cn

[S03] C：读入整数
来源：http://nh.hnjuh.cn

int x; scanf("%d", &x);
来源：http://up.haigaiapp.cn

[S04] C：字符串复制
来源：http://oh.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kc.bjjhwx.cn

[S05] C：字符串长度
来源：http://cz.lnxyls.cn

strlen(s)
来源：http://at.yuexingan06.cn

[S06] C：字符串比较
来源：http://bm.nszjky.cn

strcmp(a, b) == 0
来源：http://br.szxytkj.cn

[S07] C：数组遍历求和
来源：http://qd.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nj.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ku.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mj.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://vo.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ll.nszjky.cn

[S10] C：指针与解引用
来源：http://fj.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://qz.shxzukj.cn

[S11] C：逐行读文件
来源：http://xh.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://sx.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bi.muxihuayi.cn

fclose(f);
来源：http://uj.haigaiapp.cn

[S12] C：写文件
来源：http://qp.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qw.szxytkj.cn

[S13] C：宏定义
来源：http://nz.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mn.wgjwhj.cn

[S14] C：枚举
来源：http://jl.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://nt.huixinmuqiang.cn

[S15] C：类型转换
来源：http://vg.jctech888.com.cn

(double) a / b
来源：http://ve.jctech888.com.cn

[S16] C：位操作置位
来源：http://xv.521024.cn

x |= (1 << 3);
来源：http://sp.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://lg.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zx.bookmarksfly.cn

[S18] C：命令行参数
来源：http://pl.haigaiapp.cn

int main(int argc, char **argv)
来源：http://ld.yuexingan06.cn

[S19] C：快速排序
来源：http://ei.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pc.hnjuh.cn

[S20] C：二分查找
来源：http://lq.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nu.gzmigu.cn

[S21] C：字符类别判断
来源：http://qk.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ss.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://dk.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://et.bookmarksfly.cn

[S23] C：随机数
来源：http://nr.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cq.wgjwhj.cn

[S24] C：获取本地时间
来源：http://zd.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kl.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://aa.gzmigu.cn

memcpy(dst, src, n);
来源：http://bv.muxihuayi.cn

[S26] C：内存清零
来源：http://vs.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://db.yuexingan06.cn

[S27] C：定义常量
来源：http://sn.huixiangedu.cn

const double PI = 3.14159;
来源：http://vc.lnxyls.cn

[S28] C：静态变量
来源：http://kw.szxytkj.cn

static int counter = 0;
来源：http://zm.9csxet.cn

[S29] C：变参函数
来源：http://dk.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oc.hnjuh.cn

[S30] C：头文件保护
来源：http://ld.shxzukj.cn

#ifndef X_H
来源：http://ju.bjjhwx.cn

#define X_H
来源：http://vt.nszjky.cn

#endif
来源：http://nw.nicolike.cn

[S31] C++：Hello World
来源：http://vj.shtwfgs.cn

#include <iostream>
来源：http://dg.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://yv.szsharing.cn

[S32] C++：字符串
来源：http://qh.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://sy.colortex.cn

[S33] C++：vector 增删
来源：http://rk.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pj.huanxung.cn

[S34] C++：遍历 vector
来源：http://qc.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://gj.colortex.cn

[S35] C++：map
来源：http://cc.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fz.nszjky.cn

[S36] C++：unordered_map
来源：http://eq.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wo.521024.cn

[S37] C++：set
来源：http://ve.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ig.huixiangedu.cn

[S38] C++：排序
来源：http://yl.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://wg.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://pg.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ts.asd995.cn

[S40] C++：查找元素
来源：http://qo.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ny.nszjky.cn

[S41] C++：类与构造函数
来源：http://fm.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://di.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://tv.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://ot.nicolike.cn

[S43] C++：智能指针
来源：http://ft.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://mc.bookmarksfly.cn

[S44] C++：引用传参
来源：http://rc.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://mm.nicolike.cn

[S45] C++：lambda
来源：http://nt.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fd.muxihuayi.cn

[S46] C++：函数模板
来源：http://ln.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qq.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://sp.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ph.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://zx.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bd.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://vz.nszjky.cn

[S49] C++：写文件
来源：http://vl.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gp.haigaiapp.cn

[S50] C++：格式化数字
来源：http://kx.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jz.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://fw.yuexingan06.cn

static_cast<double>(a) / b
来源：http://st.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://sj.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://zg.hnjuh.cn

[S53] C++：移动语义
来源：http://gf.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://dg.bookmarksfly.cn

[S54] C++：异常处理
来源：http://bb.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bt.szxytkj.cn

[S55] C++：结构化绑定
来源：http://iy.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://px.shxzukj.cn

[S56] C++：optional
来源：http://ab.bjjhwx.cn


<!-- 参考信息 -->