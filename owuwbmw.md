代发 wailian999

[Q80] 字符串截取
来源：http://qb.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://on.hnjuh.cn

[Q81] 字符串替换
来源：http://lr.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ie.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://ru.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tm.hnjuh.cn

[Q83] 大小写转换
来源：http://wn.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xq.panjiajie.cn

[Q84] 去除首尾空格
来源：http://ik.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://bk.szsharing.cn

[Q85] 数值取整
来源：http://ee.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xh.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://nh.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yy.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://mm.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fj.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://sd.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bi.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uh.szsharing.cn

[Q89] 判断表是否存在
来源：http://jn.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nh.huixiangedu.cn

[Q90] 生成序号列
来源：http://dc.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ad.yuntaijiaju.cn

================================================================================
来源：http://pd.szsharing.cn

R. Bash 专题
来源：http://uj.lnxyls.cn

================================================================================
来源：http://al.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://ri.asd995.cn

#!/usr/bin/env bash
来源：http://oj.521024.cn

set -euo pipefail
来源：http://ru.gzmigu.cn

[R02] 变量赋值与使用
来源：http://cm.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://ar.jctech888.com.cn

[R03] 只读变量
来源：http://of.yuntaijiaju.cn

readonly PI=3.14
来源：http://bf.muxihuayi.cn

[R04] 位置参数
来源：http://fx.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dn.yuexingan06.cn

[R05] 参数默认值
来源：http://yq.nszjky.cn

name="${1:-default}"
来源：http://dt.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://ki.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hj.asd995.cn

[R07] if 判断文件
来源：http://pu.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vg.szxytkj.cn

[R08] 数值比较
来源：http://sy.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pj.huixiangedu.cn

[R09] 字符串比较
来源：http://cm.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hx.9csxet.cn

[R10] 正则匹配
来源：http://lw.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kd.colortex.cn

[R11] case 多分支
来源：http://hd.newstarts.cn

case "$1" in
来源：http://qj.chemitech.net.cn

start) echo "启动" ;;
来源：http://ko.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://ky.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://ge.hahajie.cn

esac
来源：http://ci.szxytkj.cn

[R12] for 遍历文件
来源：http://lh.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://co.shxzukj.cn

[R13] for 计数循环
来源：http://ib.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://id.huixiangedu.cn

[R14] C 风格 for
来源：http://ev.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lr.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://hd.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://el.521024.cn

[R16] until 等待条件
来源：http://mb.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fq.colortex.cn

[R17] 数组定义与取值
来源：http://xp.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nq.yuexingan06.cn

[R18] 遍历数组
来源：http://xu.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lu.wgjwhj.cn

[R19] 数组长度
来源：http://or.shxzukj.cn

echo "${#arr[@]}"
来源：http://rt.szsharing.cn

[R20] 关联数组（字典）
来源：http://rw.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ci.jctech888.com.cn

[R21] 字符串长度
来源：http://oh.gzmigu.cn

echo "${#s}"
来源：http://cr.shtwfgs.cn

[R22] 截取子串
来源：http://xx.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://tr.nicolike.cn

[R23] 字符串替换
来源：http://qz.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ph.9csxet.cn

[R24] 大小写转换
来源：http://nf.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xt.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://mf.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://on.hahajie.cn

[R26] 命令替换
来源：http://qm.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://xx.szsharing.cn

[R27] 算术展开
来源：http://lj.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://yj.huanxung.cn

[R28] 浮点运算
来源：http://xa.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://fy.hnjuh.cn

[R29] 定义函数
来源：http://td.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zj.shtwfgs.cn

[R30] 函数返回状态码
来源：http://pm.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://gp.asd995.cn

[R31] 局部变量
来源：http://cz.521024.cn

f() { local x=1; echo "$x"; }
来源：http://sr.bookmarksfly.cn

[R32] 参数个数校验
来源：http://mx.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iw.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://zk.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ob.bjjhwx.cn

[R34] 退出时清理
来源：http://kq.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wk.asd995.cn

[R35] 后台执行并等待
来源：http://ja.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qf.nicolike.cn

[R36] 并发执行多个任务
来源：http://jn.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mw.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://kc.bjjhwx.cn

files=$(ls -1)
来源：http://ys.panjiajie.cn

[R38] 管道串联
来源：http://ar.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://hw.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://sz.jctech888.com.cn

cmd > out.log 2>&1
来源：http://ps.haigaiapp.cn

[R40] 追加写日志
来源：http://ep.colortex.cn

echo "log" >> out.log
来源：http://cz.hnjuh.cn

[R41] 丢弃输出
来源：http://jf.colortex.cn

cmd >/dev/null 2>&1
来源：http://qy.chemitech.net.cn

[R42] 输入重定向
来源：http://dj.9csxet.cn

wc -l < a.txt
来源：http://tr.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://nt.haigaiapp.cn

find . -name "*.log" -type f
来源：http://zg.nszjky.cn

[R44] 按修改时间查找
来源：http://xe.gzmigu.cn

find . -mtime -7 -type f
来源：http://yd.panjiajie.cn

[R45] 批量删除
来源：http://gs.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://yp.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://df.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wd.hahajie.cn

[R47] sed 单行替换
来源：http://sc.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sx.newstarts.cn

[R48] awk 取指定列
来源：http://lr.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://ka.huixiangedu.cn

[R49] awk 带条件
来源：http://cj.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vt.nszjky.cn

[R50] awk 求和
来源：http://ut.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nw.huixiangedu.cn

[R51] 排序去重取前几
来源：http://pe.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yh.huanxung.cn

[R52] 统计行数
来源：http://vg.chemitech.net.cn

wc -l a.txt
来源：http://go.521024.cn

[R53] 查看文件头与实时尾
来源：http://kt.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://el.521024.cn

[R54] 比较两个文件
来源：http://fm.bjjhwx.cn

diff a.txt b.txt
来源：http://fs.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://am.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ih.521024.cn

[R56] 远程拷贝
来源：http://uq.jctech888.com.cn

scp file user@host:/path/
来源：http://qz.panjiajie.cn

[R57] 远程执行命令
来源：http://ja.gzmigu.cn

ssh user@host 'uptime'
来源：http://em.nicolike.cn

[R58] 下载文件
来源：http://qg.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dq.gzmigu.cn

[R59] 发 POST JSON
来源：http://ih.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lc.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://zw.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fx.9csxet.cn

[R61] 磁盘占用
来源：http://jn.bjjhwx.cn

df -h;  du -sh *
来源：http://jn.gzmigu.cn

[R62] 找最占空间的文件
来源：http://hk.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://ao.jianghongdianzi.cn

[R63] 内存与进程
来源：http://tz.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://bp.hahajie.cn

[R64] 结束进程
来源：http://jg.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://qz.bookmarksfly.cn

[R65] 查看端口占用
来源：http://vc.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aa.huixinmuqiang.cn

[R66] 定时任务
来源：http://yi.nicolike.cn

crontab -e;  crontab -l
来源：http://om.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://cc.jctech888.com.cn

openssl rand -hex 16
来源：http://op.panjiajie.cn

[R68] 计算文件校验值
来源：http://wi.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wb.newstarts.cn

[R69] 生成随机密码
来源：http://eh.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://ua.huanxung.cn

[R70] 时间戳与互转
来源：http://sf.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://ij.wgjwhj.cn

[R71] 日期格式化
来源：http://sj.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lx.wgjwhj.cn

[R72] 等待端口就绪
来源：http://iu.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fw.huixiangedu.cn

[R73] 分割大日志
来源：http://ki.hahajie.cn

split -l 1000 big.log part_
来源：http://pl.shxzskj.cn

[R74] 批量重命名
来源：http://um.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://us.colortex.cn

[R75] 导出环境变量
来源：http://vl.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://us.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://bb.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ic.huanxung.cn

[R77] 读取用户输入
来源：http://oh.521024.cn

read -rp "请输入: " ans
来源：http://qr.huixiangedu.cn

[R78] 交互式菜单
来源：http://oo.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sj.bjjhwx.cn

[R79] 解析命令行选项
来源：http://ms.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hh.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://xs.chemitech.net.cn

time ./run.sh
来源：http://ai.chemitech.net.cn

================================================================================
来源：http://lb.nszjky.cn

S. C / C++ 专题
来源：http://lu.lnxyls.cn

================================================================================
来源：http://oq.jianghongdianzi.cn

[S01] C：Hello World
来源：http://yj.shxzskj.cn

#include <stdio.h>
来源：http://rh.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ac.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://sy.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://qf.lnxyls.cn

[S03] C：读入整数
来源：http://xw.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://av.wgjwhj.cn

[S04] C：字符串复制
来源：http://nj.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bp.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://pl.chemitech.net.cn

strlen(s)
来源：http://vu.szsharing.cn

[S06] C：字符串比较
来源：http://xa.bjjhwx.cn

strcmp(a, b) == 0
来源：http://ic.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://ip.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gu.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://bz.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bc.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://jq.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tr.huanxung.cn

[S10] C：指针与解引用
来源：http://pf.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://iz.wgjwhj.cn

[S11] C：逐行读文件
来源：http://vp.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://fm.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ne.colortex.cn

fclose(f);
来源：http://eo.szsharing.cn

[S12] C：写文件
来源：http://ra.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yp.lnxyls.cn

[S13] C：宏定义
来源：http://nn.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gb.9csxet.cn

[S14] C：枚举
来源：http://lw.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://je.asd995.cn

[S15] C：类型转换
来源：http://nt.shxzskj.cn

(double) a / b
来源：http://kw.wgjwhj.cn

[S16] C：位操作置位
来源：http://ae.nszjky.cn

x |= (1 << 3);
来源：http://kz.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://tb.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mg.9csxet.cn

[S18] C：命令行参数
来源：http://xu.szsharing.cn

int main(int argc, char **argv)
来源：http://qd.panjiajie.cn

[S19] C：快速排序
来源：http://wc.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aw.chemitech.net.cn

[S20] C：二分查找
来源：http://rq.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wz.huanxung.cn

[S21] C：字符类别判断
来源：http://oc.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mg.jctech888.com.cn

[S22] C：字符串转数字
来源：http://up.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wy.shxzskj.cn

[S23] C：随机数
来源：http://fz.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oz.9csxet.cn

[S24] C：获取本地时间
来源：http://bf.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jk.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://yx.huanxung.cn

memcpy(dst, src, n);
来源：http://vn.shtwfgs.cn

[S26] C：内存清零
来源：http://xa.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://kx.huanxung.cn

[S27] C：定义常量
来源：http://wn.shxzskj.cn

const double PI = 3.14159;
来源：http://eh.newstarts.cn

[S28] C：静态变量
来源：http://cy.newstarts.cn

static int counter = 0;
来源：http://pc.huixinmuqiang.cn

[S29] C：变参函数
来源：http://eh.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bo.nicolike.cn

[S30] C：头文件保护
来源：http://nx.wgjwhj.cn

#ifndef X_H
来源：http://kz.nszjky.cn

#define X_H
来源：http://uj.shxzskj.cn

#endif
来源：http://mi.wgjwhj.cn

[S31] C++：Hello World
来源：http://tf.yuntaijiaju.cn

#include <iostream>
来源：http://ng.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://ab.jianghongdianzi.cn

[S32] C++：字符串
来源：http://ov.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://hj.chemitech.net.cn

[S33] C++：vector 增删
来源：http://pe.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yo.huanxung.cn

[S34] C++：遍历 vector
来源：http://pr.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://xf.jianghongdianzi.cn

[S35] C++：map
来源：http://vp.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mv.9csxet.cn

[S36] C++：unordered_map
来源：http://js.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nf.szsharing.cn

[S37] C++：set
来源：http://dd.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ld.bookmarksfly.cn

[S38] C++：排序
来源：http://tq.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://gb.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://gv.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ro.newstarts.cn

[S40] C++：查找元素
来源：http://ok.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gw.szsharing.cn

[S41] C++：类与构造函数
来源：http://nw.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lf.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://jl.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://dg.shxzskj.cn

[S43] C++：智能指针
来源：http://ri.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://ps.shxzukj.cn

[S44] C++：引用传参
来源：http://xh.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://cf.lnxyls.cn

[S45] C++：lambda
来源：http://lt.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nl.bookmarksfly.cn

[S46] C++：函数模板
来源：http://hp.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wm.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://iw.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pf.szxytkj.cn

[S48] C++：逐行读文件
来源：http://dw.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mk.nicolike.cn

while (std::getline(in, line)) { }
来源：http://ka.bjjhwx.cn

[S49] C++：写文件
来源：http://gt.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://im.hahajie.cn

[S50] C++：格式化数字
来源：http://fu.shxzukj.cn


<!-- 参考信息 -->