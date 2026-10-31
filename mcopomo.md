代发 wailian999

[Q84] 去除首尾空格
来源：http://qo.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://hc.muxihuayi.cn

[Q85] 数值取整
来源：http://nk.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tx.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://ia.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://an.szsharing.cn

[Q87] JSON 字段做条件
来源：http://ib.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qb.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://vm.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tm.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ij.huanxung.cn

[Q89] 判断表是否存在
来源：http://py.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xw.wgjwhj.cn

[Q90] 生成序号列
来源：http://je.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://re.hahajie.cn

================================================================================
来源：http://bz.bjjhwx.cn

R. Bash 专题
来源：http://an.huixiangedu.cn

================================================================================
来源：http://cz.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://pa.lnxyls.cn

#!/usr/bin/env bash
来源：http://fk.jctech888.com.cn

set -euo pipefail
来源：http://lz.nicolike.cn

[R02] 变量赋值与使用
来源：http://vi.521024.cn

name="Tom"; echo "$name"
来源：http://gf.newstarts.cn

[R03] 只读变量
来源：http://aq.shxzukj.cn

readonly PI=3.14
来源：http://fx.gzmigu.cn

[R04] 位置参数
来源：http://ml.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vi.nszjky.cn

[R05] 参数默认值
来源：http://tz.haigaiapp.cn

name="${1:-default}"
来源：http://kf.lnxyls.cn

[R06] 判断命令是否存在
来源：http://fm.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nt.521024.cn

[R07] if 判断文件
来源：http://wr.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://db.jianghongdianzi.cn

[R08] 数值比较
来源：http://ut.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sa.521024.cn

[R09] 字符串比较
来源：http://wz.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lg.521024.cn

[R10] 正则匹配
来源：http://lx.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dt.gzmigu.cn

[R11] case 多分支
来源：http://ze.nicolike.cn

case "$1" in
来源：http://en.newstarts.cn

start) echo "启动" ;;
来源：http://gw.hnjuh.cn

stop)  echo "停止" ;;
来源：http://tm.colortex.cn

*)     echo "未知命令" ;;
来源：http://ep.huanxung.cn

esac
来源：http://of.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://px.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://ck.shxzskj.cn

[R13] for 计数循环
来源：http://yt.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://ot.colortex.cn

[R14] C 风格 for
来源：http://jq.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://da.yuexingan06.cn

[R15] while 逐行读文件
来源：http://uf.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ff.haigaiapp.cn

[R16] until 等待条件
来源：http://fq.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jv.lnxyls.cn

[R17] 数组定义与取值
来源：http://ab.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rx.shxzukj.cn

[R18] 遍历数组
来源：http://xt.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qn.hahajie.cn

[R19] 数组长度
来源：http://qm.9csxet.cn

echo "${#arr[@]}"
来源：http://sc.lnxyls.cn

[R20] 关联数组（字典）
来源：http://qe.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://td.shxzskj.cn

[R21] 字符串长度
来源：http://us.hnjuh.cn

echo "${#s}"
来源：http://yv.muxihuayi.cn

[R22] 截取子串
来源：http://ta.hahajie.cn

echo "${s:0:5}"
来源：http://hk.muxihuayi.cn

[R23] 字符串替换
来源：http://px.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uf.nicolike.cn

[R24] 大小写转换
来源：http://cw.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pt.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://tc.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sq.jctech888.com.cn

[R26] 命令替换
来源：http://jo.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://ls.yuntaijiaju.cn

[R27] 算术展开
来源：http://pa.nicolike.cn

echo $((1 + 2 * 3))
来源：http://jf.shxzskj.cn

[R28] 浮点运算
来源：http://ez.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://ei.szxytkj.cn

[R29] 定义函数
来源：http://le.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ih.muxihuayi.cn

[R30] 函数返回状态码
来源：http://jh.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://sj.wgjwhj.cn

[R31] 局部变量
来源：http://lk.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://tg.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://xl.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bb.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://ps.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hp.jianghongdianzi.cn

[R34] 退出时清理
来源：http://fi.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bg.muxihuayi.cn

[R35] 后台执行并等待
来源：http://hq.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://do.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://oy.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://po.colortex.cn

[R37] 把输出赋给变量
来源：http://nm.yuntaijiaju.cn

files=$(ls -1)
来源：http://vb.huanxung.cn

[R38] 管道串联
来源：http://zj.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://um.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://kv.bjjhwx.cn

cmd > out.log 2>&1
来源：http://vy.huixiangedu.cn

[R40] 追加写日志
来源：http://vt.gzmigu.cn

echo "log" >> out.log
来源：http://cd.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://ow.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://ie.hahajie.cn

[R42] 输入重定向
来源：http://vk.bookmarksfly.cn

wc -l < a.txt
来源：http://nc.huanxung.cn

[R43] 按名字查找文件
来源：http://ki.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://dr.hnjuh.cn

[R44] 按修改时间查找
来源：http://uh.shtwfgs.cn

find . -mtime -7 -type f
来源：http://wc.haigaiapp.cn

[R45] 批量删除
来源：http://ls.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://kj.gzmigu.cn

[R46] 递归替换文件内容
来源：http://cj.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qi.lnxyls.cn

[R47] sed 单行替换
来源：http://eo.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fd.shxzukj.cn

[R48] awk 取指定列
来源：http://sk.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://ad.szsharing.cn

[R49] awk 带条件
来源：http://ar.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://id.bookmarksfly.cn

[R50] awk 求和
来源：http://hw.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wp.newstarts.cn

[R51] 排序去重取前几
来源：http://dg.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wx.hahajie.cn

[R52] 统计行数
来源：http://fo.jctech888.com.cn

wc -l a.txt
来源：http://rs.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://mq.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zx.lnxyls.cn

[R54] 比较两个文件
来源：http://pe.yuexingan06.cn

diff a.txt b.txt
来源：http://wi.newstarts.cn

[R55] 压缩与解压
来源：http://im.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pd.shtwfgs.cn

[R56] 远程拷贝
来源：http://dl.yuntaijiaju.cn

scp file user@host:/path/
来源：http://tk.9csxet.cn

[R57] 远程执行命令
来源：http://oe.yuexingan06.cn

ssh user@host 'uptime'
来源：http://zy.chemitech.net.cn

[R58] 下载文件
来源：http://ju.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qk.szxytkj.cn

[R59] 发 POST JSON
来源：http://ri.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://so.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://zc.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lc.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://bl.colortex.cn

df -h;  du -sh *
来源：http://nf.newstarts.cn

[R62] 找最占空间的文件
来源：http://wz.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://yt.hahajie.cn

[R63] 内存与进程
来源：http://he.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://mv.jianghongdianzi.cn

[R64] 结束进程
来源：http://xf.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://vu.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://ci.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eh.muxihuayi.cn

[R66] 定时任务
来源：http://tt.hahajie.cn

crontab -e;  crontab -l
来源：http://fw.hahajie.cn

[R67] 生成随机十六进制串
来源：http://cc.9csxet.cn

openssl rand -hex 16
来源：http://bz.chemitech.net.cn

[R68] 计算文件校验值
来源：http://yi.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zf.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://so.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://xr.haigaiapp.cn

[R70] 时间戳与互转
来源：http://xv.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://db.yuexingan06.cn

[R71] 日期格式化
来源：http://dv.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iu.hahajie.cn

[R72] 等待端口就绪
来源：http://zq.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gm.bookmarksfly.cn

[R73] 分割大日志
来源：http://dr.bjjhwx.cn

split -l 1000 big.log part_
来源：http://qm.huixinmuqiang.cn

[R74] 批量重命名
来源：http://sz.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yr.shxzukj.cn

[R75] 导出环境变量
来源：http://oc.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://jg.huanxung.cn

[R76] 使用临时文件
来源：http://ku.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zb.huixiangedu.cn

[R77] 读取用户输入
来源：http://yr.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://uh.chemitech.net.cn

[R78] 交互式菜单
来源：http://zd.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dy.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://wi.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lw.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://oy.szsharing.cn

time ./run.sh
来源：http://yc.huixiangedu.cn

================================================================================
来源：http://rh.newstarts.cn

S. C / C++ 专题
来源：http://xn.shxzukj.cn

================================================================================
来源：http://we.shtwfgs.cn

[S01] C：Hello World
来源：http://eh.szxytkj.cn

#include <stdio.h>
来源：http://oz.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ss.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://ps.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://kj.bookmarksfly.cn

[S03] C：读入整数
来源：http://vx.9csxet.cn

int x; scanf("%d", &x);
来源：http://pf.szxytkj.cn

[S04] C：字符串复制
来源：http://co.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ly.shtwfgs.cn

[S05] C：字符串长度
来源：http://lv.jctech888.com.cn

strlen(s)
来源：http://ut.szxytkj.cn

[S06] C：字符串比较
来源：http://ro.hahajie.cn

strcmp(a, b) == 0
来源：http://kn.nicolike.cn

[S07] C：数组遍历求和
来源：http://ug.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qa.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://nw.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qv.colortex.cn

[S09] C：结构体定义与初始化
来源：http://ph.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hw.muxihuayi.cn

[S10] C：指针与解引用
来源：http://vj.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://gv.hnjuh.cn

[S11] C：逐行读文件
来源：http://fg.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://qb.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ve.shxzskj.cn

fclose(f);
来源：http://cx.bookmarksfly.cn

[S12] C：写文件
来源：http://fr.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yo.haigaiapp.cn

[S13] C：宏定义
来源：http://kp.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pg.yuntaijiaju.cn

[S14] C：枚举
来源：http://tb.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://og.yuexingan06.cn

[S15] C：类型转换
来源：http://uh.521024.cn

(double) a / b
来源：http://hp.nicolike.cn

[S16] C：位操作置位
来源：http://lf.nicolike.cn

x |= (1 << 3);
来源：http://nr.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://vs.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gk.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://zb.panjiajie.cn

int main(int argc, char **argv)
来源：http://ak.huixiangedu.cn

[S19] C：快速排序
来源：http://lp.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oe.9csxet.cn

[S20] C：二分查找
来源：http://zt.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rf.haigaiapp.cn

[S21] C：字符类别判断
来源：http://ph.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://en.colortex.cn

[S22] C：字符串转数字
来源：http://qb.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rx.lnxyls.cn

[S23] C：随机数
来源：http://so.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wh.muxihuayi.cn

[S24] C：获取本地时间
来源：http://jl.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cb.bjjhwx.cn

[S25] C：内存拷贝
来源：http://tn.hnjuh.cn

memcpy(dst, src, n);
来源：http://du.asd995.cn

[S26] C：内存清零
来源：http://lk.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://co.lnxyls.cn

[S27] C：定义常量
来源：http://kw.huanxung.cn

const double PI = 3.14159;
来源：http://mj.jctech888.com.cn

[S28] C：静态变量
来源：http://pv.colortex.cn

static int counter = 0;
来源：http://zv.9csxet.cn

[S29] C：变参函数
来源：http://ig.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qp.shxzskj.cn

[S30] C：头文件保护
来源：http://ut.huixinmuqiang.cn

#ifndef X_H
来源：http://yh.szxytkj.cn

#define X_H
来源：http://ld.nicolike.cn

#endif
来源：http://gi.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://dz.yuntaijiaju.cn

#include <iostream>
来源：http://kg.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://bd.yuexingan06.cn

[S32] C++：字符串
来源：http://cw.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://sn.huixiangedu.cn

[S33] C++：vector 增删
来源：http://zw.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fp.9csxet.cn

[S34] C++：遍历 vector
来源：http://rj.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://oh.nicolike.cn

[S35] C++：map
来源：http://iq.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ai.huixiangedu.cn

[S36] C++：unordered_map
来源：http://gl.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ja.nicolike.cn

[S37] C++：set
来源：http://xt.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://og.szxytkj.cn

[S38] C++：排序
来源：http://sx.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://zg.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://yc.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ao.huixiangedu.cn

[S40] C++：查找元素
来源：http://xm.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://th.asd995.cn

[S41] C++：类与构造函数
来源：http://gl.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vb.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://vk.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://qy.huanxung.cn

[S43] C++：智能指针
来源：http://fy.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://ie.shtwfgs.cn

[S44] C++：引用传参
来源：http://xo.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://ku.shxzskj.cn

[S45] C++：lambda
来源：http://gq.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gj.lnxyls.cn

[S46] C++：函数模板
来源：http://jy.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hk.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://gb.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ix.lnxyls.cn

[S48] C++：逐行读文件
来源：http://ei.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bb.9csxet.cn

while (std::getline(in, line)) { }
来源：http://qn.shxzukj.cn

[S49] C++：写文件
来源：http://nv.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rm.newstarts.cn

[S50] C++：格式化数字
来源：http://wl.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://un.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://et.szxytkj.cn

static_cast<double>(a) / b
来源：http://gk.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://mz.521024.cn

int size() const noexcept { return n_; }
来源：http://de.panjiajie.cn

[S53] C++：移动语义
来源：http://uc.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://hk.nicolike.cn

[S54] C++：异常处理
来源：http://kt.nicolike.cn


<!-- 参考信息 -->