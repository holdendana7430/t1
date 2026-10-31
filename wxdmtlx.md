代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://zt.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://po.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jv.asd995.cn

[Q89] 判断表是否存在
来源：http://ge.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vq.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://as.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qs.panjiajie.cn

================================================================================
来源：http://av.haigaiapp.cn

R. Bash 专题
来源：http://rb.wgjwhj.cn

================================================================================
来源：http://zw.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://hp.shtwfgs.cn

#!/usr/bin/env bash
来源：http://kn.yuntaijiaju.cn

set -euo pipefail
来源：http://sn.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://ys.shxzskj.cn

name="Tom"; echo "$name"
来源：http://kt.jctech888.com.cn

[R03] 只读变量
来源：http://nm.huixinmuqiang.cn

readonly PI=3.14
来源：http://uu.yuntaijiaju.cn

[R04] 位置参数
来源：http://uh.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fl.yuexingan06.cn

[R05] 参数默认值
来源：http://rc.shxzukj.cn

name="${1:-default}"
来源：http://qx.nszjky.cn

[R06] 判断命令是否存在
来源：http://ps.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cc.huanxung.cn

[R07] if 判断文件
来源：http://mu.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jv.hnjuh.cn

[R08] 数值比较
来源：http://am.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sw.gzmigu.cn

[R09] 字符串比较
来源：http://uz.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jb.jctech888.com.cn

[R10] 正则匹配
来源：http://jc.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sz.colortex.cn

[R11] case 多分支
来源：http://at.521024.cn

case "$1" in
来源：http://lg.asd995.cn

start) echo "启动" ;;
来源：http://qa.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://es.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://kt.newstarts.cn

esac
来源：http://ci.yuexingan06.cn

[R12] for 遍历文件
来源：http://cw.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://ug.shxzukj.cn

[R13] for 计数循环
来源：http://kv.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ea.shxzukj.cn

[R14] C 风格 for
来源：http://ud.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ao.szsharing.cn

[R15] while 逐行读文件
来源：http://om.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ln.bookmarksfly.cn

[R16] until 等待条件
来源：http://uv.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xb.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://bo.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fx.wgjwhj.cn

[R18] 遍历数组
来源：http://ji.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ak.nicolike.cn

[R19] 数组长度
来源：http://vu.nszjky.cn

echo "${#arr[@]}"
来源：http://gy.huanxung.cn

[R20] 关联数组（字典）
来源：http://pw.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sq.huanxung.cn

[R21] 字符串长度
来源：http://qb.shtwfgs.cn

echo "${#s}"
来源：http://fz.gzmigu.cn

[R22] 截取子串
来源：http://lx.nszjky.cn

echo "${s:0:5}"
来源：http://cc.shxzskj.cn

[R23] 字符串替换
来源：http://ju.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://np.panjiajie.cn

[R24] 大小写转换
来源：http://uj.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kx.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://pr.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vt.jianghongdianzi.cn

[R26] 命令替换
来源：http://gr.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://fs.hnjuh.cn

[R27] 算术展开
来源：http://hg.asd995.cn

echo $((1 + 2 * 3))
来源：http://qt.huixinmuqiang.cn

[R28] 浮点运算
来源：http://rv.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://ml.haigaiapp.cn

[R29] 定义函数
来源：http://ex.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ro.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://au.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ef.bookmarksfly.cn

[R31] 局部变量
来源：http://xf.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://jl.shtwfgs.cn

[R32] 参数个数校验
来源：http://mc.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mu.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://po.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ch.huixiangedu.cn

[R34] 退出时清理
来源：http://ve.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xe.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://uw.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ud.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://ii.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nf.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://me.shxzskj.cn

files=$(ls -1)
来源：http://sz.hahajie.cn

[R38] 管道串联
来源：http://nf.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://dg.521024.cn

[R39] 重定向标准输出与错误
来源：http://cj.wgjwhj.cn

cmd > out.log 2>&1
来源：http://ef.szsharing.cn

[R40] 追加写日志
来源：http://jq.gzmigu.cn

echo "log" >> out.log
来源：http://qu.bjjhwx.cn

[R41] 丢弃输出
来源：http://hh.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://uf.bookmarksfly.cn

[R42] 输入重定向
来源：http://xd.panjiajie.cn

wc -l < a.txt
来源：http://uk.huanxung.cn

[R43] 按名字查找文件
来源：http://ca.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://fa.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://dn.panjiajie.cn

find . -mtime -7 -type f
来源：http://nk.huixiangedu.cn

[R45] 批量删除
来源：http://or.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://qh.szsharing.cn

[R46] 递归替换文件内容
来源：http://fe.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sw.bjjhwx.cn

[R47] sed 单行替换
来源：http://jp.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xm.nicolike.cn

[R48] awk 取指定列
来源：http://la.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://zn.9csxet.cn

[R49] awk 带条件
来源：http://fz.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cq.jianghongdianzi.cn

[R50] awk 求和
来源：http://py.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rg.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://hr.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://br.lnxyls.cn

[R52] 统计行数
来源：http://hs.asd995.cn

wc -l a.txt
来源：http://gy.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://fb.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ic.hahajie.cn

[R54] 比较两个文件
来源：http://ra.huanxung.cn

diff a.txt b.txt
来源：http://cf.hnjuh.cn

[R55] 压缩与解压
来源：http://ox.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://td.yuexingan06.cn

[R56] 远程拷贝
来源：http://sk.hahajie.cn

scp file user@host:/path/
来源：http://qq.hnjuh.cn

[R57] 远程执行命令
来源：http://hd.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://fk.shxzskj.cn

[R58] 下载文件
来源：http://hs.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mj.huixiangedu.cn

[R59] 发 POST JSON
来源：http://xm.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xm.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://rx.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uz.chemitech.net.cn

[R61] 磁盘占用
来源：http://bh.hahajie.cn

df -h;  du -sh *
来源：http://du.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://vb.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://wv.huixinmuqiang.cn

[R63] 内存与进程
来源：http://vv.521024.cn

free -h;  ps aux | grep nginx
来源：http://gr.szxytkj.cn

[R64] 结束进程
来源：http://fn.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://ez.shxzskj.cn

[R65] 查看端口占用
来源：http://pc.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ft.jianghongdianzi.cn

[R66] 定时任务
来源：http://fx.szsharing.cn

crontab -e;  crontab -l
来源：http://do.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://qv.lnxyls.cn

openssl rand -hex 16
来源：http://wb.newstarts.cn

[R68] 计算文件校验值
来源：http://ah.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dc.9csxet.cn

[R69] 生成随机密码
来源：http://wu.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://kz.wgjwhj.cn

[R70] 时间戳与互转
来源：http://yn.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://uc.nicolike.cn

[R71] 日期格式化
来源：http://it.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ol.shxzskj.cn

[R72] 等待端口就绪
来源：http://lp.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zm.huixinmuqiang.cn

[R73] 分割大日志
来源：http://zl.szxytkj.cn

split -l 1000 big.log part_
来源：http://yo.521024.cn

[R74] 批量重命名
来源：http://ff.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nj.jctech888.com.cn

[R75] 导出环境变量
来源：http://qt.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://gk.hnjuh.cn

[R76] 使用临时文件
来源：http://ll.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vt.huixiangedu.cn

[R77] 读取用户输入
来源：http://mm.newstarts.cn

read -rp "请输入: " ans
来源：http://xx.muxihuayi.cn

[R78] 交互式菜单
来源：http://sw.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ew.colortex.cn

[R79] 解析命令行选项
来源：http://ef.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ul.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://tv.chemitech.net.cn

time ./run.sh
来源：http://yi.chemitech.net.cn

================================================================================
来源：http://hm.newstarts.cn

S. C / C++ 专题
来源：http://vw.chemitech.net.cn

================================================================================
来源：http://mg.lnxyls.cn

[S01] C：Hello World
来源：http://iy.gzmigu.cn

#include <stdio.h>
来源：http://ez.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pc.asd995.cn

[S02] C：变量与格式化输出
来源：http://kf.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://vn.521024.cn

[S03] C：读入整数
来源：http://hf.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://ha.muxihuayi.cn

[S04] C：字符串复制
来源：http://aq.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nb.panjiajie.cn

[S05] C：字符串长度
来源：http://gf.jianghongdianzi.cn

strlen(s)
来源：http://fr.chemitech.net.cn

[S06] C：字符串比较
来源：http://pt.gzmigu.cn

strcmp(a, b) == 0
来源：http://tp.9csxet.cn

[S07] C：数组遍历求和
来源：http://id.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mj.asd995.cn

[S08] C：动态内存分配与释放
来源：http://jv.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hn.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://qc.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nt.gzmigu.cn

[S10] C：指针与解引用
来源：http://dd.colortex.cn

int *p = &a;  *p = 5;
来源：http://fa.asd995.cn

[S11] C：逐行读文件
来源：http://rn.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://zr.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rr.yuntaijiaju.cn

fclose(f);
来源：http://ph.lnxyls.cn

[S12] C：写文件
来源：http://vz.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lm.asd995.cn

[S13] C：宏定义
来源：http://lz.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sr.9csxet.cn

[S14] C：枚举
来源：http://zj.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://ex.nszjky.cn

[S15] C：类型转换
来源：http://ub.bjjhwx.cn

(double) a / b
来源：http://vr.huixiangedu.cn

[S16] C：位操作置位
来源：http://dm.hahajie.cn

x |= (1 << 3);
来源：http://dq.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://ee.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yn.muxihuayi.cn

[S18] C：命令行参数
来源：http://im.bjjhwx.cn

int main(int argc, char **argv)
来源：http://xy.bjjhwx.cn

[S19] C：快速排序
来源：http://br.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://im.huixinmuqiang.cn

[S20] C：二分查找
来源：http://ai.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://su.szxytkj.cn

[S21] C：字符类别判断
来源：http://gu.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ry.hnjuh.cn

[S22] C：字符串转数字
来源：http://mq.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ez.shtwfgs.cn

[S23] C：随机数
来源：http://vi.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zm.asd995.cn

[S24] C：获取本地时间
来源：http://ds.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ic.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://mf.nszjky.cn

memcpy(dst, src, n);
来源：http://om.newstarts.cn

[S26] C：内存清零
来源：http://ah.szsharing.cn

memset(a, 0, sizeof a);
来源：http://ls.szsharing.cn

[S27] C：定义常量
来源：http://zz.colortex.cn

const double PI = 3.14159;
来源：http://es.nszjky.cn

[S28] C：静态变量
来源：http://nf.szxytkj.cn

static int counter = 0;
来源：http://zo.huixinmuqiang.cn

[S29] C：变参函数
来源：http://ua.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zu.nszjky.cn

[S30] C：头文件保护
来源：http://rr.hnjuh.cn

#ifndef X_H
来源：http://fs.shxzskj.cn

#define X_H
来源：http://bc.yuexingan06.cn

#endif
来源：http://oi.szsharing.cn

[S31] C++：Hello World
来源：http://go.yuexingan06.cn

#include <iostream>
来源：http://ts.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://bb.nicolike.cn

[S32] C++：字符串
来源：http://hx.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://pu.szxytkj.cn

[S33] C++：vector 增删
来源：http://kq.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tv.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://nu.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ul.nicolike.cn

[S35] C++：map
来源：http://ou.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mp.lnxyls.cn

[S36] C++：unordered_map
来源：http://gc.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nk.bookmarksfly.cn

[S37] C++：set
来源：http://ls.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yi.yuexingan06.cn

[S38] C++：排序
来源：http://sm.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://cn.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://mq.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ut.newstarts.cn

[S40] C++：查找元素
来源：http://kf.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zl.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://ff.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kl.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://wy.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://fs.szsharing.cn

[S43] C++：智能指针
来源：http://pu.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://uh.shxzskj.cn

[S44] C++：引用传参
来源：http://ab.nszjky.cn

void inc(int &x) { ++x; }
来源：http://qp.newstarts.cn

[S45] C++：lambda
来源：http://ks.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xp.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://pn.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mp.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://vr.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tm.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://ja.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fa.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://zl.huixiangedu.cn

[S49] C++：写文件
来源：http://si.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rr.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://zd.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://og.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://op.newstarts.cn

static_cast<double>(a) / b
来源：http://di.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://mp.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://ef.hnjuh.cn

[S53] C++：移动语义
来源：http://fo.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://nn.bookmarksfly.cn

[S54] C++：异常处理
来源：http://hn.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kr.panjiajie.cn

[S55] C++：结构化绑定
来源：http://nm.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ly.yuntaijiaju.cn

[S56] C++：optional
来源：http://tg.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qt.huixiangedu.cn

[S57] C++：编译期常量
来源：http://pg.jctech888.com.cn

constexpr int N = 10;
来源：http://hl.nicolike.cn

[S58] C++：命名空间
来源：http://xm.huixinmuqiang.cn


<!-- 参考信息 -->