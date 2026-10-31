代发 wailian999

[Q84] 去除首尾空格
来源：http://wt.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://bu.bjjhwx.cn

[Q85] 数值取整
来源：http://sh.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cg.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://kp.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bj.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://jt.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ze.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://au.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vc.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rs.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://tj.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nc.hnjuh.cn

[Q90] 生成序号列
来源：http://ua.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nc.9csxet.cn

================================================================================
来源：http://vn.shtwfgs.cn

R. Bash 专题
来源：http://ak.huixinmuqiang.cn

================================================================================
来源：http://qt.szxytkj.cn

[R01] shebang 与严格模式
来源：http://lm.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://xk.colortex.cn

set -euo pipefail
来源：http://qz.asd995.cn

[R02] 变量赋值与使用
来源：http://gm.asd995.cn

name="Tom"; echo "$name"
来源：http://ox.huixiangedu.cn

[R03] 只读变量
来源：http://sl.9csxet.cn

readonly PI=3.14
来源：http://jr.yuntaijiaju.cn

[R04] 位置参数
来源：http://yq.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tb.shxzukj.cn

[R05] 参数默认值
来源：http://oq.bookmarksfly.cn

name="${1:-default}"
来源：http://bn.shxzskj.cn

[R06] 判断命令是否存在
来源：http://ua.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jk.shtwfgs.cn

[R07] if 判断文件
来源：http://aw.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yf.nicolike.cn

[R08] 数值比较
来源：http://fk.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jz.chemitech.net.cn

[R09] 字符串比较
来源：http://aj.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ft.szsharing.cn

[R10] 正则匹配
来源：http://nz.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qb.shxzskj.cn

[R11] case 多分支
来源：http://rr.newstarts.cn

case "$1" in
来源：http://mv.gzmigu.cn

start) echo "启动" ;;
来源：http://rs.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://pu.9csxet.cn

*)     echo "未知命令" ;;
来源：http://ge.wgjwhj.cn

esac
来源：http://vo.haigaiapp.cn

[R12] for 遍历文件
来源：http://ct.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://du.szsharing.cn

[R13] for 计数循环
来源：http://hn.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://kp.521024.cn

[R14] C 风格 for
来源：http://po.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bq.szsharing.cn

[R15] while 逐行读文件
来源：http://df.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hc.huanxung.cn

[R16] until 等待条件
来源：http://qc.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tt.colortex.cn

[R17] 数组定义与取值
来源：http://qp.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tw.huixinmuqiang.cn

[R18] 遍历数组
来源：http://gi.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xq.hahajie.cn

[R19] 数组长度
来源：http://nr.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://rv.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://cy.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yc.huixinmuqiang.cn

[R21] 字符串长度
来源：http://ov.huixinmuqiang.cn

echo "${#s}"
来源：http://xg.gzmigu.cn

[R22] 截取子串
来源：http://sv.huixiangedu.cn

echo "${s:0:5}"
来源：http://nv.hnjuh.cn

[R23] 字符串替换
来源：http://hh.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zu.shtwfgs.cn

[R24] 大小写转换
来源：http://br.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ne.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://ia.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pw.521024.cn

[R26] 命令替换
来源：http://ob.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://or.gzmigu.cn

[R27] 算术展开
来源：http://yf.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://kn.bjjhwx.cn

[R28] 浮点运算
来源：http://ih.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://uu.9csxet.cn

[R29] 定义函数
来源：http://co.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ws.wgjwhj.cn

[R30] 函数返回状态码
来源：http://om.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://tc.shtwfgs.cn

[R31] 局部变量
来源：http://ip.521024.cn

f() { local x=1; echo "$x"; }
来源：http://wy.gzmigu.cn

[R32] 参数个数校验
来源：http://wa.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ua.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://yd.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vr.chemitech.net.cn

[R34] 退出时清理
来源：http://jk.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ae.chemitech.net.cn

[R35] 后台执行并等待
来源：http://to.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zd.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://id.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ct.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://yo.panjiajie.cn

files=$(ls -1)
来源：http://ap.huixiangedu.cn

[R38] 管道串联
来源：http://hn.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://bm.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://kj.jctech888.com.cn

cmd > out.log 2>&1
来源：http://yz.muxihuayi.cn

[R40] 追加写日志
来源：http://fq.bjjhwx.cn

echo "log" >> out.log
来源：http://qk.bookmarksfly.cn

[R41] 丢弃输出
来源：http://cd.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://ad.colortex.cn

[R42] 输入重定向
来源：http://fj.shxzukj.cn

wc -l < a.txt
来源：http://ha.huixiangedu.cn

[R43] 按名字查找文件
来源：http://yt.521024.cn

find . -name "*.log" -type f
来源：http://at.asd995.cn

[R44] 按修改时间查找
来源：http://xo.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://bt.jianghongdianzi.cn

[R45] 批量删除
来源：http://sr.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://wr.lnxyls.cn

[R46] 递归替换文件内容
来源：http://tc.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gu.colortex.cn

[R47] sed 单行替换
来源：http://cj.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://db.colortex.cn

[R48] awk 取指定列
来源：http://mv.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://za.huixiangedu.cn

[R49] awk 带条件
来源：http://gs.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lb.bookmarksfly.cn

[R50] awk 求和
来源：http://hw.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://md.chemitech.net.cn

[R51] 排序去重取前几
来源：http://ed.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yg.szxytkj.cn

[R52] 统计行数
来源：http://lr.chemitech.net.cn

wc -l a.txt
来源：http://ud.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://ju.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zl.haigaiapp.cn

[R54] 比较两个文件
来源：http://wm.9csxet.cn

diff a.txt b.txt
来源：http://ov.asd995.cn

[R55] 压缩与解压
来源：http://yy.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fz.shxzukj.cn

[R56] 远程拷贝
来源：http://ci.wgjwhj.cn

scp file user@host:/path/
来源：http://bj.bjjhwx.cn

[R57] 远程执行命令
来源：http://nm.wgjwhj.cn

ssh user@host 'uptime'
来源：http://ie.gzmigu.cn

[R58] 下载文件
来源：http://eu.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://el.nicolike.cn

[R59] 发 POST JSON
来源：http://jd.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kv.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://pa.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bo.muxihuayi.cn

[R61] 磁盘占用
来源：http://dg.nicolike.cn

df -h;  du -sh *
来源：http://wt.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://um.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://ty.shtwfgs.cn

[R63] 内存与进程
来源：http://um.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://pi.huanxung.cn

[R64] 结束进程
来源：http://im.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://pm.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://at.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lh.jctech888.com.cn

[R66] 定时任务
来源：http://uc.yuexingan06.cn

crontab -e;  crontab -l
来源：http://du.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://ky.jctech888.com.cn

openssl rand -hex 16
来源：http://sd.newstarts.cn

[R68] 计算文件校验值
来源：http://np.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://um.shtwfgs.cn

[R69] 生成随机密码
来源：http://xl.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://sf.shtwfgs.cn

[R70] 时间戳与互转
来源：http://qn.colortex.cn

date +%s;  date -d @1700000000
来源：http://um.chemitech.net.cn

[R71] 日期格式化
来源：http://pf.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zj.colortex.cn

[R72] 等待端口就绪
来源：http://bg.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jo.muxihuayi.cn

[R73] 分割大日志
来源：http://vn.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://nz.yuntaijiaju.cn

[R74] 批量重命名
来源：http://md.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hv.gzmigu.cn

[R75] 导出环境变量
来源：http://xt.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://qi.hnjuh.cn

[R76] 使用临时文件
来源：http://oq.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aq.nszjky.cn

[R77] 读取用户输入
来源：http://ln.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://xr.shxzukj.cn

[R78] 交互式菜单
来源：http://nm.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cs.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://he.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nk.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://ga.wgjwhj.cn

time ./run.sh
来源：http://zp.szxytkj.cn

================================================================================
来源：http://es.lnxyls.cn

S. C / C++ 专题
来源：http://rd.shxzskj.cn

================================================================================
来源：http://cb.nszjky.cn

[S01] C：Hello World
来源：http://lv.szsharing.cn

#include <stdio.h>
来源：http://ym.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rc.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://pv.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://yr.yuntaijiaju.cn

[S03] C：读入整数
来源：http://kf.szxytkj.cn

int x; scanf("%d", &x);
来源：http://sy.nicolike.cn

[S04] C：字符串复制
来源：http://zo.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mr.nicolike.cn

[S05] C：字符串长度
来源：http://en.muxihuayi.cn

strlen(s)
来源：http://vt.szsharing.cn

[S06] C：字符串比较
来源：http://yy.wgjwhj.cn

strcmp(a, b) == 0
来源：http://ul.szsharing.cn

[S07] C：数组遍历求和
来源：http://dt.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sz.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://ot.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zb.521024.cn

[S09] C：结构体定义与初始化
来源：http://ov.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://be.bjjhwx.cn

[S10] C：指针与解引用
来源：http://mr.colortex.cn

int *p = &a;  *p = 5;
来源：http://sf.panjiajie.cn

[S11] C：逐行读文件
来源：http://uz.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://zd.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fx.colortex.cn

fclose(f);
来源：http://ie.huixiangedu.cn

[S12] C：写文件
来源：http://zh.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ys.9csxet.cn

[S13] C：宏定义
来源：http://vl.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pk.panjiajie.cn

[S14] C：枚举
来源：http://oa.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://ne.haigaiapp.cn

[S15] C：类型转换
来源：http://fo.shxzukj.cn

(double) a / b
来源：http://rt.szsharing.cn

[S16] C：位操作置位
来源：http://fm.muxihuayi.cn

x |= (1 << 3);
来源：http://lm.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://rp.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fm.yuexingan06.cn

[S18] C：命令行参数
来源：http://bz.9csxet.cn

int main(int argc, char **argv)
来源：http://rn.hnjuh.cn

[S19] C：快速排序
来源：http://yr.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wc.huixinmuqiang.cn

[S20] C：二分查找
来源：http://gk.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jl.yuexingan06.cn

[S21] C：字符类别判断
来源：http://uq.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vl.wgjwhj.cn

[S22] C：字符串转数字
来源：http://wq.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lf.yuntaijiaju.cn

[S23] C：随机数
来源：http://cc.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uu.gzmigu.cn

[S24] C：获取本地时间
来源：http://wc.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://of.nszjky.cn

[S25] C：内存拷贝
来源：http://tp.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://xm.haigaiapp.cn

[S26] C：内存清零
来源：http://bm.hahajie.cn

memset(a, 0, sizeof a);
来源：http://et.yuntaijiaju.cn

[S27] C：定义常量
来源：http://sv.jctech888.com.cn

const double PI = 3.14159;
来源：http://yn.huixiangedu.cn

[S28] C：静态变量
来源：http://fd.hnjuh.cn

static int counter = 0;
来源：http://cw.hnjuh.cn

[S29] C：变参函数
来源：http://gw.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nk.huanxung.cn

[S30] C：头文件保护
来源：http://ao.szsharing.cn

#ifndef X_H
来源：http://yo.bjjhwx.cn

#define X_H
来源：http://kr.huixinmuqiang.cn

#endif
来源：http://py.lnxyls.cn

[S31] C++：Hello World
来源：http://mp.yuexingan06.cn

#include <iostream>
来源：http://xf.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://ks.nicolike.cn

[S32] C++：字符串
来源：http://mm.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://ss.jctech888.com.cn

[S33] C++：vector 增删
来源：http://ip.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ti.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://hs.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://sr.colortex.cn

[S35] C++：map
来源：http://ml.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bj.521024.cn

[S36] C++：unordered_map
来源：http://pg.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pv.huixiangedu.cn

[S37] C++：set
来源：http://ma.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://im.huanxung.cn

[S38] C++：排序
来源：http://vl.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://gz.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://sr.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tv.9csxet.cn

[S40] C++：查找元素
来源：http://ti.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gb.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://tp.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lj.521024.cn

[S42] C++：继承与虚函数
来源：http://td.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://go.9csxet.cn

[S43] C++：智能指针
来源：http://vj.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://uu.asd995.cn

[S44] C++：引用传参
来源：http://ms.newstarts.cn

void inc(int &x) { ++x; }
来源：http://ko.newstarts.cn

[S45] C++：lambda
来源：http://yt.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pp.bjjhwx.cn

[S46] C++：函数模板
来源：http://cb.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ms.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://yg.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vt.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://yt.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vq.nszjky.cn

while (std::getline(in, line)) { }
来源：http://pm.panjiajie.cn

[S49] C++：写文件
来源：http://ki.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://he.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://sf.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lu.panjiajie.cn

[S51] C++：显式类型转换
来源：http://fo.shxzskj.cn

static_cast<double>(a) / b
来源：http://oi.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://mq.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://vz.bookmarksfly.cn

[S53] C++：移动语义
来源：http://cm.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://ky.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://qm.jctech888.com.cn


<!-- 参考信息 -->