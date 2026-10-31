代发 wailian999

[Q82] 字符长度与字节长度
来源：http://ja.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cr.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://ip.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yv.hahajie.cn

[Q84] 去除首尾空格
来源：http://pi.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://ju.huanxung.cn

[Q85] 数值取整
来源：http://hi.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aa.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://oi.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xz.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://rb.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fy.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://lk.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wl.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vp.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://zw.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vq.shxzskj.cn

[Q90] 生成序号列
来源：http://vj.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cr.shtwfgs.cn

================================================================================
来源：http://uh.nicolike.cn

R. Bash 专题
来源：http://fp.yuntaijiaju.cn

================================================================================
来源：http://nz.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://zs.colortex.cn

#!/usr/bin/env bash
来源：http://iq.shxzukj.cn

set -euo pipefail
来源：http://dp.huanxung.cn

[R02] 变量赋值与使用
来源：http://vg.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://me.huanxung.cn

[R03] 只读变量
来源：http://kk.asd995.cn

readonly PI=3.14
来源：http://hm.szxytkj.cn

[R04] 位置参数
来源：http://ft.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xg.shxzukj.cn

[R05] 参数默认值
来源：http://wk.hahajie.cn

name="${1:-default}"
来源：http://cc.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://qc.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rl.nszjky.cn

[R07] if 判断文件
来源：http://jp.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zc.huixinmuqiang.cn

[R08] 数值比较
来源：http://hh.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uc.nicolike.cn

[R09] 字符串比较
来源：http://sn.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ek.panjiajie.cn

[R10] 正则匹配
来源：http://oe.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lo.hnjuh.cn

[R11] case 多分支
来源：http://qu.jianghongdianzi.cn

case "$1" in
来源：http://ri.hahajie.cn

start) echo "启动" ;;
来源：http://lv.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://pl.szsharing.cn

*)     echo "未知命令" ;;
来源：http://wh.panjiajie.cn

esac
来源：http://fo.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://ii.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://qd.yuntaijiaju.cn

[R13] for 计数循环
来源：http://sk.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://vi.gzmigu.cn

[R14] C 风格 for
来源：http://qr.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bz.9csxet.cn

[R15] while 逐行读文件
来源：http://me.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xk.hahajie.cn

[R16] until 等待条件
来源：http://cn.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lt.lnxyls.cn

[R17] 数组定义与取值
来源：http://cy.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gi.chemitech.net.cn

[R18] 遍历数组
来源：http://eu.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ln.szsharing.cn

[R19] 数组长度
来源：http://ct.nicolike.cn

echo "${#arr[@]}"
来源：http://mk.newstarts.cn

[R20] 关联数组（字典）
来源：http://ux.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://av.521024.cn

[R21] 字符串长度
来源：http://os.asd995.cn

echo "${#s}"
来源：http://va.muxihuayi.cn

[R22] 截取子串
来源：http://lt.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://op.bjjhwx.cn

[R23] 字符串替换
来源：http://xo.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xy.huixinmuqiang.cn

[R24] 大小写转换
来源：http://cs.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qm.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://yt.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ls.lnxyls.cn

[R26] 命令替换
来源：http://oz.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://wy.bjjhwx.cn

[R27] 算术展开
来源：http://uz.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://ga.nicolike.cn

[R28] 浮点运算
来源：http://ox.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://tg.nszjky.cn

[R29] 定义函数
来源：http://xz.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qc.yuexingan06.cn

[R30] 函数返回状态码
来源：http://qg.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://yd.shtwfgs.cn

[R31] 局部变量
来源：http://yn.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://go.yuexingan06.cn

[R32] 参数个数校验
来源：http://rt.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fn.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://mh.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bs.shtwfgs.cn

[R34] 退出时清理
来源：http://ty.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jj.newstarts.cn

[R35] 后台执行并等待
来源：http://zu.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xn.panjiajie.cn

[R36] 并发执行多个任务
来源：http://lv.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zw.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://qb.521024.cn

files=$(ls -1)
来源：http://sj.huixinmuqiang.cn

[R38] 管道串联
来源：http://xk.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://hu.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://za.szxytkj.cn

cmd > out.log 2>&1
来源：http://ca.bjjhwx.cn

[R40] 追加写日志
来源：http://ex.colortex.cn

echo "log" >> out.log
来源：http://xa.asd995.cn

[R41] 丢弃输出
来源：http://xb.nicolike.cn

cmd >/dev/null 2>&1
来源：http://pq.wgjwhj.cn

[R42] 输入重定向
来源：http://oi.shxzskj.cn

wc -l < a.txt
来源：http://qr.szxytkj.cn

[R43] 按名字查找文件
来源：http://je.asd995.cn

find . -name "*.log" -type f
来源：http://vc.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://jj.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://hb.panjiajie.cn

[R45] 批量删除
来源：http://sr.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://rt.hnjuh.cn

[R46] 递归替换文件内容
来源：http://dy.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xj.nszjky.cn

[R47] sed 单行替换
来源：http://qs.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nw.nicolike.cn

[R48] awk 取指定列
来源：http://wv.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://ed.9csxet.cn

[R49] awk 带条件
来源：http://xk.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uh.yuntaijiaju.cn

[R50] awk 求和
来源：http://qy.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cb.haigaiapp.cn

[R51] 排序去重取前几
来源：http://kl.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ha.yuntaijiaju.cn

[R52] 统计行数
来源：http://sd.shxzukj.cn

wc -l a.txt
来源：http://ns.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://iz.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wj.shtwfgs.cn

[R54] 比较两个文件
来源：http://sw.hahajie.cn

diff a.txt b.txt
来源：http://gw.huixiangedu.cn

[R55] 压缩与解压
来源：http://ao.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kp.haigaiapp.cn

[R56] 远程拷贝
来源：http://xh.huixiangedu.cn

scp file user@host:/path/
来源：http://zd.jctech888.com.cn

[R57] 远程执行命令
来源：http://uw.9csxet.cn

ssh user@host 'uptime'
来源：http://gg.gzmigu.cn

[R58] 下载文件
来源：http://im.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vb.huanxung.cn

[R59] 发 POST JSON
来源：http://hp.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lc.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://kc.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qr.yuexingan06.cn

[R61] 磁盘占用
来源：http://ll.gzmigu.cn

df -h;  du -sh *
来源：http://qi.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://in.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://cd.hnjuh.cn

[R63] 内存与进程
来源：http://iz.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://yd.bookmarksfly.cn

[R64] 结束进程
来源：http://ha.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://iw.muxihuayi.cn

[R65] 查看端口占用
来源：http://ez.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lf.asd995.cn

[R66] 定时任务
来源：http://ye.asd995.cn

crontab -e;  crontab -l
来源：http://ms.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://oa.gzmigu.cn

openssl rand -hex 16
来源：http://rm.gzmigu.cn

[R68] 计算文件校验值
来源：http://dj.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ca.9csxet.cn

[R69] 生成随机密码
来源：http://el.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://cc.colortex.cn

[R70] 时间戳与互转
来源：http://uj.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://dg.szxytkj.cn

[R71] 日期格式化
来源：http://ab.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pi.yuexingan06.cn

[R72] 等待端口就绪
来源：http://vw.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ep.huixinmuqiang.cn

[R73] 分割大日志
来源：http://dz.colortex.cn

split -l 1000 big.log part_
来源：http://ww.jctech888.com.cn

[R74] 批量重命名
来源：http://ub.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tm.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://ae.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://fx.jctech888.com.cn

[R76] 使用临时文件
来源：http://tl.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ii.yuexingan06.cn

[R77] 读取用户输入
来源：http://ak.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://em.lnxyls.cn

[R78] 交互式菜单
来源：http://pf.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ag.nicolike.cn

[R79] 解析命令行选项
来源：http://wq.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ia.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://jf.panjiajie.cn

time ./run.sh
来源：http://mn.shxzskj.cn

================================================================================
来源：http://nu.wgjwhj.cn

S. C / C++ 专题
来源：http://iw.shtwfgs.cn

================================================================================
来源：http://ll.521024.cn

[S01] C：Hello World
来源：http://lu.yuntaijiaju.cn

#include <stdio.h>
来源：http://lj.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ka.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://ox.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://fx.gzmigu.cn

[S03] C：读入整数
来源：http://te.hahajie.cn

int x; scanf("%d", &x);
来源：http://ci.bookmarksfly.cn

[S04] C：字符串复制
来源：http://et.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://am.nicolike.cn

[S05] C：字符串长度
来源：http://qw.lnxyls.cn

strlen(s)
来源：http://rx.9csxet.cn

[S06] C：字符串比较
来源：http://il.shxzskj.cn

strcmp(a, b) == 0
来源：http://rm.panjiajie.cn

[S07] C：数组遍历求和
来源：http://gu.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lh.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://ga.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aa.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://yy.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ai.haigaiapp.cn

[S10] C：指针与解引用
来源：http://xq.asd995.cn

int *p = &a;  *p = 5;
来源：http://ju.9csxet.cn

[S11] C：逐行读文件
来源：http://zu.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://kd.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://po.szsharing.cn

fclose(f);
来源：http://ak.szsharing.cn

[S12] C：写文件
来源：http://eq.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jk.panjiajie.cn

[S13] C：宏定义
来源：http://lt.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nq.nicolike.cn

[S14] C：枚举
来源：http://oe.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://qc.colortex.cn

[S15] C：类型转换
来源：http://jf.huixiangedu.cn

(double) a / b
来源：http://gf.huixiangedu.cn

[S16] C：位操作置位
来源：http://xh.yuexingan06.cn

x |= (1 << 3);
来源：http://fm.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://me.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mv.hnjuh.cn

[S18] C：命令行参数
来源：http://bm.chemitech.net.cn

int main(int argc, char **argv)
来源：http://ad.9csxet.cn

[S19] C：快速排序
来源：http://bx.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dx.asd995.cn

[S20] C：二分查找
来源：http://ig.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vz.yuexingan06.cn

[S21] C：字符类别判断
来源：http://kj.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rc.haigaiapp.cn

[S22] C：字符串转数字
来源：http://iq.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lr.wgjwhj.cn

[S23] C：随机数
来源：http://zz.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lg.bjjhwx.cn

[S24] C：获取本地时间
来源：http://ou.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tf.szsharing.cn

[S25] C：内存拷贝
来源：http://gh.nicolike.cn

memcpy(dst, src, n);
来源：http://lk.yuexingan06.cn

[S26] C：内存清零
来源：http://px.9csxet.cn

memset(a, 0, sizeof a);
来源：http://fz.szxytkj.cn

[S27] C：定义常量
来源：http://vh.huixiangedu.cn

const double PI = 3.14159;
来源：http://qm.szsharing.cn

[S28] C：静态变量
来源：http://dm.gzmigu.cn

static int counter = 0;
来源：http://cs.huanxung.cn

[S29] C：变参函数
来源：http://hz.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ac.nicolike.cn

[S30] C：头文件保护
来源：http://py.szxytkj.cn

#ifndef X_H
来源：http://zj.jianghongdianzi.cn

#define X_H
来源：http://pp.nszjky.cn

#endif
来源：http://kk.panjiajie.cn

[S31] C++：Hello World
来源：http://bb.lnxyls.cn

#include <iostream>
来源：http://uv.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://yi.shtwfgs.cn

[S32] C++：字符串
来源：http://fv.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://ir.yuexingan06.cn

[S33] C++：vector 增删
来源：http://ul.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://on.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://pn.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ub.szsharing.cn

[S35] C++：map
来源：http://cs.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ks.yuexingan06.cn

[S36] C++：unordered_map
来源：http://lw.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ut.yuexingan06.cn

[S37] C++：set
来源：http://ce.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ek.newstarts.cn

[S38] C++：排序
来源：http://ss.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://ct.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://hk.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ag.lnxyls.cn

[S40] C++：查找元素
来源：http://oi.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uc.asd995.cn

[S41] C++：类与构造函数
来源：http://wd.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tp.colortex.cn

[S42] C++：继承与虚函数
来源：http://sa.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://oz.asd995.cn

[S43] C++：智能指针
来源：http://lk.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://gn.colortex.cn

[S44] C++：引用传参
来源：http://nn.szsharing.cn

void inc(int &x) { ++x; }
来源：http://qc.yuexingan06.cn

[S45] C++：lambda
来源：http://hd.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cu.lnxyls.cn

[S46] C++：函数模板
来源：http://dl.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://od.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://wk.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ep.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://yx.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nk.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://dv.asd995.cn

[S49] C++：写文件
来源：http://nu.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rk.nszjky.cn

[S50] C++：格式化数字
来源：http://ue.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://de.nszjky.cn

[S51] C++：显式类型转换
来源：http://di.521024.cn

static_cast<double>(a) / b
来源：http://do.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://vx.nszjky.cn


<!-- 参考信息 -->