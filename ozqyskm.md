代发 wailian999

[Q86] 读取 JSON 字段
来源：http://xr.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tx.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://ev.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hc.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://ms.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vr.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://re.asd995.cn

[Q89] 判断表是否存在
来源：http://sy.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yc.shxzukj.cn

[Q90] 生成序号列
来源：http://mo.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dw.lnxyls.cn

================================================================================
来源：http://wp.jianghongdianzi.cn

R. Bash 专题
来源：http://oz.huanxung.cn

================================================================================
来源：http://ws.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://ud.hahajie.cn

#!/usr/bin/env bash
来源：http://ov.muxihuayi.cn

set -euo pipefail
来源：http://kc.hnjuh.cn

[R02] 变量赋值与使用
来源：http://gx.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://xu.bookmarksfly.cn

[R03] 只读变量
来源：http://gs.yuexingan06.cn

readonly PI=3.14
来源：http://vm.wgjwhj.cn

[R04] 位置参数
来源：http://rj.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gl.jctech888.com.cn

[R05] 参数默认值
来源：http://by.shtwfgs.cn

name="${1:-default}"
来源：http://hg.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://px.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fi.huanxung.cn

[R07] if 判断文件
来源：http://zs.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ud.newstarts.cn

[R08] 数值比较
来源：http://hb.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wl.yuexingan06.cn

[R09] 字符串比较
来源：http://zy.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wa.shtwfgs.cn

[R10] 正则匹配
来源：http://uk.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rv.huixiangedu.cn

[R11] case 多分支
来源：http://cb.yuntaijiaju.cn

case "$1" in
来源：http://qm.521024.cn

start) echo "启动" ;;
来源：http://ap.gzmigu.cn

stop)  echo "停止" ;;
来源：http://qn.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://tv.huixiangedu.cn

esac
来源：http://ea.muxihuayi.cn

[R12] for 遍历文件
来源：http://rd.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://wl.asd995.cn

[R13] for 计数循环
来源：http://vd.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://rr.521024.cn

[R14] C 风格 for
来源：http://qw.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ba.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://ys.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lh.hnjuh.cn

[R16] until 等待条件
来源：http://vr.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ca.wgjwhj.cn

[R17] 数组定义与取值
来源：http://zk.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iv.huanxung.cn

[R18] 遍历数组
来源：http://nl.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ft.gzmigu.cn

[R19] 数组长度
来源：http://yp.nicolike.cn

echo "${#arr[@]}"
来源：http://us.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://li.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ar.wgjwhj.cn

[R21] 字符串长度
来源：http://qm.haigaiapp.cn

echo "${#s}"
来源：http://pf.bjjhwx.cn

[R22] 截取子串
来源：http://fl.chemitech.net.cn

echo "${s:0:5}"
来源：http://rs.lnxyls.cn

[R23] 字符串替换
来源：http://xy.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vn.haigaiapp.cn

[R24] 大小写转换
来源：http://zm.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mk.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://ui.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vl.muxihuayi.cn

[R26] 命令替换
来源：http://jf.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://yh.yuexingan06.cn

[R27] 算术展开
来源：http://yt.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://io.chemitech.net.cn

[R28] 浮点运算
来源：http://es.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://dg.huanxung.cn

[R29] 定义函数
来源：http://es.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uf.hahajie.cn

[R30] 函数返回状态码
来源：http://yl.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://ku.huixinmuqiang.cn

[R31] 局部变量
来源：http://mb.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://xg.shtwfgs.cn

[R32] 参数个数校验
来源：http://ok.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wl.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://ne.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zs.nszjky.cn

[R34] 退出时清理
来源：http://mt.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tp.nszjky.cn

[R35] 后台执行并等待
来源：http://sz.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ec.hahajie.cn

[R36] 并发执行多个任务
来源：http://um.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://so.nszjky.cn

[R37] 把输出赋给变量
来源：http://jn.chemitech.net.cn

files=$(ls -1)
来源：http://qs.huixinmuqiang.cn

[R38] 管道串联
来源：http://tp.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://bm.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://gq.9csxet.cn

cmd > out.log 2>&1
来源：http://tr.bjjhwx.cn

[R40] 追加写日志
来源：http://hf.yuexingan06.cn

echo "log" >> out.log
来源：http://tc.nszjky.cn

[R41] 丢弃输出
来源：http://ia.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://xu.bookmarksfly.cn

[R42] 输入重定向
来源：http://tj.shxzskj.cn

wc -l < a.txt
来源：http://tj.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://up.newstarts.cn

find . -name "*.log" -type f
来源：http://nc.haigaiapp.cn

[R44] 按修改时间查找
来源：http://np.shxzukj.cn

find . -mtime -7 -type f
来源：http://ai.shxzukj.cn

[R45] 批量删除
来源：http://os.colortex.cn

find . -name "*.tmp" -delete
来源：http://tx.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://xo.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ao.lnxyls.cn

[R47] sed 单行替换
来源：http://cu.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ga.hnjuh.cn

[R48] awk 取指定列
来源：http://qo.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://vu.bookmarksfly.cn

[R49] awk 带条件
来源：http://fs.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cl.shxzukj.cn

[R50] awk 求和
来源：http://ar.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rf.lnxyls.cn

[R51] 排序去重取前几
来源：http://ct.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kk.panjiajie.cn

[R52] 统计行数
来源：http://bv.9csxet.cn

wc -l a.txt
来源：http://ju.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://nt.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yo.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://rp.huixinmuqiang.cn

diff a.txt b.txt
来源：http://rq.newstarts.cn

[R55] 压缩与解压
来源：http://zq.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://er.huixiangedu.cn

[R56] 远程拷贝
来源：http://lq.jctech888.com.cn

scp file user@host:/path/
来源：http://zd.newstarts.cn

[R57] 远程执行命令
来源：http://br.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://wk.haigaiapp.cn

[R58] 下载文件
来源：http://bg.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eh.panjiajie.cn

[R59] 发 POST JSON
来源：http://tz.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ha.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://uw.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://px.bookmarksfly.cn

[R61] 磁盘占用
来源：http://gr.bjjhwx.cn

df -h;  du -sh *
来源：http://xn.521024.cn

[R62] 找最占空间的文件
来源：http://ic.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://tp.colortex.cn

[R63] 内存与进程
来源：http://ji.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://zp.yuntaijiaju.cn

[R64] 结束进程
来源：http://bq.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://fn.hnjuh.cn

[R65] 查看端口占用
来源：http://ij.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xz.hnjuh.cn

[R66] 定时任务
来源：http://he.shxzskj.cn

crontab -e;  crontab -l
来源：http://up.colortex.cn

[R67] 生成随机十六进制串
来源：http://lm.jianghongdianzi.cn

openssl rand -hex 16
来源：http://bu.gzmigu.cn

[R68] 计算文件校验值
来源：http://az.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xm.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://jt.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://vb.shxzukj.cn

[R70] 时间戳与互转
来源：http://wl.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://ks.chemitech.net.cn

[R71] 日期格式化
来源：http://dl.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tj.chemitech.net.cn

[R72] 等待端口就绪
来源：http://ob.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hh.jianghongdianzi.cn

[R73] 分割大日志
来源：http://nr.huanxung.cn

split -l 1000 big.log part_
来源：http://mj.shtwfgs.cn

[R74] 批量重命名
来源：http://qe.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xt.hahajie.cn

[R75] 导出环境变量
来源：http://ej.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://zg.asd995.cn

[R76] 使用临时文件
来源：http://xp.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yb.bookmarksfly.cn

[R77] 读取用户输入
来源：http://ir.haigaiapp.cn

read -rp "请输入: " ans
来源：http://ar.gzmigu.cn

[R78] 交互式菜单
来源：http://yc.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bo.521024.cn

[R79] 解析命令行选项
来源：http://hp.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kz.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://at.chemitech.net.cn

time ./run.sh
来源：http://yd.chemitech.net.cn

================================================================================
来源：http://bi.szsharing.cn

S. C / C++ 专题
来源：http://wm.newstarts.cn

================================================================================
来源：http://rc.yuntaijiaju.cn

[S01] C：Hello World
来源：http://or.huixiangedu.cn

#include <stdio.h>
来源：http://dy.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gr.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://sw.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://gd.muxihuayi.cn

[S03] C：读入整数
来源：http://kt.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://tb.shtwfgs.cn

[S04] C：字符串复制
来源：http://ih.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fx.huanxung.cn

[S05] C：字符串长度
来源：http://qp.jianghongdianzi.cn

strlen(s)
来源：http://sh.colortex.cn

[S06] C：字符串比较
来源：http://gm.huixiangedu.cn

strcmp(a, b) == 0
来源：http://yl.huanxung.cn

[S07] C：数组遍历求和
来源：http://ik.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ej.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://oj.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fr.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://si.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pi.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://fx.nszjky.cn

int *p = &a;  *p = 5;
来源：http://nc.521024.cn

[S11] C：逐行读文件
来源：http://pl.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://yg.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nm.jianghongdianzi.cn

fclose(f);
来源：http://sa.bjjhwx.cn

[S12] C：写文件
来源：http://af.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://js.bjjhwx.cn

[S13] C：宏定义
来源：http://uc.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ks.wgjwhj.cn

[S14] C：枚举
来源：http://fs.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://tc.huanxung.cn

[S15] C：类型转换
来源：http://sz.muxihuayi.cn

(double) a / b
来源：http://db.asd995.cn

[S16] C：位操作置位
来源：http://kl.jianghongdianzi.cn

x |= (1 << 3);
来源：http://cr.hahajie.cn

[S17] C：安全拼接字符串
来源：http://ic.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zz.newstarts.cn

[S18] C：命令行参数
来源：http://lv.gzmigu.cn

int main(int argc, char **argv)
来源：http://kz.nicolike.cn

[S19] C：快速排序
来源：http://vg.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://za.shtwfgs.cn

[S20] C：二分查找
来源：http://zg.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yc.szsharing.cn

[S21] C：字符类别判断
来源：http://ix.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dk.shtwfgs.cn

[S22] C：字符串转数字
来源：http://gv.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://od.asd995.cn

[S23] C：随机数
来源：http://pe.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fw.wgjwhj.cn

[S24] C：获取本地时间
来源：http://jj.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qg.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://wa.nszjky.cn

memcpy(dst, src, n);
来源：http://rr.521024.cn

[S26] C：内存清零
来源：http://pr.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://gf.yuexingan06.cn

[S27] C：定义常量
来源：http://ze.asd995.cn

const double PI = 3.14159;
来源：http://xr.bookmarksfly.cn

[S28] C：静态变量
来源：http://ht.huanxung.cn

static int counter = 0;
来源：http://ds.yuntaijiaju.cn

[S29] C：变参函数
来源：http://fu.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tg.huixiangedu.cn

[S30] C：头文件保护
来源：http://kj.szsharing.cn

#ifndef X_H
来源：http://ql.colortex.cn

#define X_H
来源：http://yc.newstarts.cn

#endif
来源：http://qp.huanxung.cn

[S31] C++：Hello World
来源：http://vl.huixiangedu.cn

#include <iostream>
来源：http://il.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://au.huanxung.cn

[S32] C++：字符串
来源：http://kn.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://of.nszjky.cn

[S33] C++：vector 增删
来源：http://zk.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yp.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://sp.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://ct.huanxung.cn

[S35] C++：map
来源：http://qh.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eg.wgjwhj.cn

[S36] C++：unordered_map
来源：http://gw.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yg.wgjwhj.cn

[S37] C++：set
来源：http://rj.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ol.shxzskj.cn

[S38] C++：排序
来源：http://az.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://fr.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://ln.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://du.bookmarksfly.cn

[S40] C++：查找元素
来源：http://np.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qq.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://np.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gl.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://jn.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://ds.chemitech.net.cn

[S43] C++：智能指针
来源：http://wr.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://gn.gzmigu.cn

[S44] C++：引用传参
来源：http://cw.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://nf.yuexingan06.cn

[S45] C++：lambda
来源：http://pb.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://io.muxihuayi.cn

[S46] C++：函数模板
来源：http://xx.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cr.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://yf.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://za.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://sb.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nc.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://zx.asd995.cn

[S49] C++：写文件
来源：http://vu.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ki.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://vg.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jb.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://mx.chemitech.net.cn

static_cast<double>(a) / b
来源：http://nm.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://lp.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://my.szsharing.cn

[S53] C++：移动语义
来源：http://oi.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://tb.bjjhwx.cn

[S54] C++：异常处理
来源：http://wm.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bk.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://uf.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://an.gzmigu.cn

[S56] C++：optional
来源：http://cg.huixinmuqiang.cn


<!-- 参考信息 -->