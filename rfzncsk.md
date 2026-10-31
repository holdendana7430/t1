代发 wailian999

[Q80] 字符串截取
来源：http://vw.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nf.colortex.cn

[Q81] 字符串替换
来源：http://pr.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://if.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://xa.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qj.hahajie.cn

[Q83] 大小写转换
来源：http://cl.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fy.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://qd.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://tt.wgjwhj.cn

[Q85] 数值取整
来源：http://zq.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ry.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://zr.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ep.asd995.cn

[Q87] JSON 字段做条件
来源：http://im.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vi.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://ul.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bj.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://os.huanxung.cn

[Q89] 判断表是否存在
来源：http://vb.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rq.szsharing.cn

[Q90] 生成序号列
来源：http://df.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kr.hnjuh.cn

================================================================================
来源：http://cy.shxzukj.cn

R. Bash 专题
来源：http://bv.shxzskj.cn

================================================================================
来源：http://kz.hahajie.cn

[R01] shebang 与严格模式
来源：http://nw.szsharing.cn

#!/usr/bin/env bash
来源：http://dy.colortex.cn

set -euo pipefail
来源：http://ha.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://ve.hahajie.cn

name="Tom"; echo "$name"
来源：http://xk.huixinmuqiang.cn

[R03] 只读变量
来源：http://jx.muxihuayi.cn

readonly PI=3.14
来源：http://gd.newstarts.cn

[R04] 位置参数
来源：http://pl.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mj.yuexingan06.cn

[R05] 参数默认值
来源：http://es.nicolike.cn

name="${1:-default}"
来源：http://hj.shxzskj.cn

[R06] 判断命令是否存在
来源：http://ss.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sp.chemitech.net.cn

[R07] if 判断文件
来源：http://gl.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://na.nicolike.cn

[R08] 数值比较
来源：http://bv.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sm.panjiajie.cn

[R09] 字符串比较
来源：http://un.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xa.jianghongdianzi.cn

[R10] 正则匹配
来源：http://wa.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zq.gzmigu.cn

[R11] case 多分支
来源：http://ke.huixiangedu.cn

case "$1" in
来源：http://xo.9csxet.cn

start) echo "启动" ;;
来源：http://tx.nszjky.cn

stop)  echo "停止" ;;
来源：http://yk.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://ml.yuntaijiaju.cn

esac
来源：http://ci.jctech888.com.cn

[R12] for 遍历文件
来源：http://nd.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://fx.shtwfgs.cn

[R13] for 计数循环
来源：http://wj.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ee.shtwfgs.cn

[R14] C 风格 for
来源：http://co.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iq.shtwfgs.cn

[R15] while 逐行读文件
来源：http://yi.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jw.haigaiapp.cn

[R16] until 等待条件
来源：http://ze.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yl.hahajie.cn

[R17] 数组定义与取值
来源：http://kr.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bx.huanxung.cn

[R18] 遍历数组
来源：http://ll.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://re.huixinmuqiang.cn

[R19] 数组长度
来源：http://so.jctech888.com.cn

echo "${#arr[@]}"
来源：http://bt.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://kq.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bd.haigaiapp.cn

[R21] 字符串长度
来源：http://mq.bjjhwx.cn

echo "${#s}"
来源：http://hg.lnxyls.cn

[R22] 截取子串
来源：http://ie.shxzukj.cn

echo "${s:0:5}"
来源：http://us.shxzskj.cn

[R23] 字符串替换
来源：http://yz.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gc.haigaiapp.cn

[R24] 大小写转换
来源：http://rb.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wz.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://gp.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fx.chemitech.net.cn

[R26] 命令替换
来源：http://uk.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://bc.jctech888.com.cn

[R27] 算术展开
来源：http://hi.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://an.muxihuayi.cn

[R28] 浮点运算
来源：http://ow.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://uf.hahajie.cn

[R29] 定义函数
来源：http://ls.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xu.yuexingan06.cn

[R30] 函数返回状态码
来源：http://vb.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://ud.huixinmuqiang.cn

[R31] 局部变量
来源：http://dv.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://vf.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://hu.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pe.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://ij.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fx.hahajie.cn

[R34] 退出时清理
来源：http://ji.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cm.shxzukj.cn

[R35] 后台执行并等待
来源：http://vh.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sm.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://wz.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pp.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://nn.yuntaijiaju.cn

files=$(ls -1)
来源：http://xz.jianghongdianzi.cn

[R38] 管道串联
来源：http://ew.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://ih.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://el.chemitech.net.cn

cmd > out.log 2>&1
来源：http://ox.hnjuh.cn

[R40] 追加写日志
来源：http://pg.huixinmuqiang.cn

echo "log" >> out.log
来源：http://ng.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://ew.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://co.hahajie.cn

[R42] 输入重定向
来源：http://nu.huanxung.cn

wc -l < a.txt
来源：http://sf.asd995.cn

[R43] 按名字查找文件
来源：http://jx.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ya.szsharing.cn

[R44] 按修改时间查找
来源：http://va.hnjuh.cn

find . -mtime -7 -type f
来源：http://dt.szxytkj.cn

[R45] 批量删除
来源：http://vp.521024.cn

find . -name "*.tmp" -delete
来源：http://ap.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://gn.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://em.9csxet.cn

[R47] sed 单行替换
来源：http://oj.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lo.bookmarksfly.cn

[R48] awk 取指定列
来源：http://nm.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://ny.hnjuh.cn

[R49] awk 带条件
来源：http://zw.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wr.jctech888.com.cn

[R50] awk 求和
来源：http://ea.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ma.shxzukj.cn

[R51] 排序去重取前几
来源：http://ju.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ve.521024.cn

[R52] 统计行数
来源：http://ms.panjiajie.cn

wc -l a.txt
来源：http://me.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://ud.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jw.panjiajie.cn

[R54] 比较两个文件
来源：http://bm.hahajie.cn

diff a.txt b.txt
来源：http://hu.lnxyls.cn

[R55] 压缩与解压
来源：http://bq.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vl.panjiajie.cn

[R56] 远程拷贝
来源：http://tq.muxihuayi.cn

scp file user@host:/path/
来源：http://fa.chemitech.net.cn

[R57] 远程执行命令
来源：http://yr.hahajie.cn

ssh user@host 'uptime'
来源：http://bc.shxzukj.cn

[R58] 下载文件
来源：http://mj.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://om.bjjhwx.cn

[R59] 发 POST JSON
来源：http://jm.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zn.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://dr.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ky.shxzskj.cn

[R61] 磁盘占用
来源：http://cq.szxytkj.cn

df -h;  du -sh *
来源：http://vb.szsharing.cn

[R62] 找最占空间的文件
来源：http://mt.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://kj.asd995.cn

[R63] 内存与进程
来源：http://ly.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://rj.huixiangedu.cn

[R64] 结束进程
来源：http://vg.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://gh.yuexingan06.cn

[R65] 查看端口占用
来源：http://au.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vj.chemitech.net.cn

[R66] 定时任务
来源：http://jp.nicolike.cn

crontab -e;  crontab -l
来源：http://xc.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://mf.521024.cn

openssl rand -hex 16
来源：http://oq.huixiangedu.cn

[R68] 计算文件校验值
来源：http://id.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ak.nszjky.cn

[R69] 生成随机密码
来源：http://rf.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://pl.szxytkj.cn

[R70] 时间戳与互转
来源：http://mw.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://qx.nicolike.cn

[R71] 日期格式化
来源：http://qw.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rt.chemitech.net.cn

[R72] 等待端口就绪
来源：http://jb.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ox.nicolike.cn

[R73] 分割大日志
来源：http://kt.chemitech.net.cn

split -l 1000 big.log part_
来源：http://dh.szxytkj.cn

[R74] 批量重命名
来源：http://bj.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jg.panjiajie.cn

[R75] 导出环境变量
来源：http://fw.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://rj.shxzskj.cn

[R76] 使用临时文件
来源：http://xl.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ng.shxzukj.cn

[R77] 读取用户输入
来源：http://ki.hnjuh.cn

read -rp "请输入: " ans
来源：http://tm.asd995.cn

[R78] 交互式菜单
来源：http://tt.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bg.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://bc.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nk.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://gn.colortex.cn

time ./run.sh
来源：http://tx.yuexingan06.cn

================================================================================
来源：http://ya.shtwfgs.cn

S. C / C++ 专题
来源：http://sp.nszjky.cn

================================================================================
来源：http://vh.jctech888.com.cn

[S01] C：Hello World
来源：http://zj.colortex.cn

#include <stdio.h>
来源：http://ig.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kf.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://ju.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://jr.gzmigu.cn

[S03] C：读入整数
来源：http://wf.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://yb.nicolike.cn

[S04] C：字符串复制
来源：http://ak.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kc.huixiangedu.cn

[S05] C：字符串长度
来源：http://mj.huixiangedu.cn

strlen(s)
来源：http://mh.asd995.cn

[S06] C：字符串比较
来源：http://db.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://po.521024.cn

[S07] C：数组遍历求和
来源：http://zv.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ib.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://fo.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kn.521024.cn

[S09] C：结构体定义与初始化
来源：http://fd.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mg.shxzskj.cn

[S10] C：指针与解引用
来源：http://di.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://tb.jctech888.com.cn

[S11] C：逐行读文件
来源：http://rg.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://cy.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://of.colortex.cn

fclose(f);
来源：http://oj.asd995.cn

[S12] C：写文件
来源：http://ri.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fh.panjiajie.cn

[S13] C：宏定义
来源：http://wr.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wn.shtwfgs.cn

[S14] C：枚举
来源：http://xy.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://hp.chemitech.net.cn

[S15] C：类型转换
来源：http://pi.nicolike.cn

(double) a / b
来源：http://ln.asd995.cn

[S16] C：位操作置位
来源：http://eh.hahajie.cn

x |= (1 << 3);
来源：http://xp.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://dm.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ya.colortex.cn

[S18] C：命令行参数
来源：http://jj.panjiajie.cn

int main(int argc, char **argv)
来源：http://wy.hnjuh.cn

[S19] C：快速排序
来源：http://um.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://je.huixinmuqiang.cn

[S20] C：二分查找
来源：http://zu.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://va.nicolike.cn

[S21] C：字符类别判断
来源：http://po.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tl.nicolike.cn

[S22] C：字符串转数字
来源：http://lh.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mp.wgjwhj.cn

[S23] C：随机数
来源：http://ph.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ek.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://eh.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cq.asd995.cn

[S25] C：内存拷贝
来源：http://mu.newstarts.cn

memcpy(dst, src, n);
来源：http://th.nszjky.cn

[S26] C：内存清零
来源：http://ji.colortex.cn

memset(a, 0, sizeof a);
来源：http://wo.huixinmuqiang.cn

[S27] C：定义常量
来源：http://am.yuexingan06.cn

const double PI = 3.14159;
来源：http://ru.shxzskj.cn

[S28] C：静态变量
来源：http://hm.szsharing.cn

static int counter = 0;
来源：http://on.asd995.cn

[S29] C：变参函数
来源：http://xt.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qu.bookmarksfly.cn

[S30] C：头文件保护
来源：http://ej.jianghongdianzi.cn

#ifndef X_H
来源：http://bt.9csxet.cn

#define X_H
来源：http://qu.hnjuh.cn

#endif
来源：http://hh.chemitech.net.cn

[S31] C++：Hello World
来源：http://td.muxihuayi.cn

#include <iostream>
来源：http://hb.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://gw.nszjky.cn

[S32] C++：字符串
来源：http://wv.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://jh.shxzskj.cn

[S33] C++：vector 增删
来源：http://ri.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://na.hnjuh.cn

[S34] C++：遍历 vector
来源：http://eg.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://hq.huanxung.cn

[S35] C++：map
来源：http://ox.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tb.gzmigu.cn

[S36] C++：unordered_map
来源：http://cc.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tv.shxzukj.cn

[S37] C++：set
来源：http://tn.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yh.lnxyls.cn

[S38] C++：排序
来源：http://gz.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://kc.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://si.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ys.huixiangedu.cn

[S40] C++：查找元素
来源：http://xm.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bw.9csxet.cn

[S41] C++：类与构造函数
来源：http://ci.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qy.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://ox.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://bi.nicolike.cn

[S43] C++：智能指针
来源：http://rs.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://vg.haigaiapp.cn

[S44] C++：引用传参
来源：http://gp.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://zl.yuexingan06.cn

[S45] C++：lambda
来源：http://yu.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uf.hnjuh.cn

[S46] C++：函数模板
来源：http://lf.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hp.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://rm.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lf.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://nl.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xo.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://xs.shxzskj.cn

[S49] C++：写文件
来源：http://zt.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gg.hahajie.cn

[S50] C++：格式化数字
来源：http://ys.shxzskj.cn


<!-- 参考信息 -->