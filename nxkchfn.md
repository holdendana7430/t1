代发 wailian999

[Q84] 去除首尾空格
来源：http://sr.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://lx.yuntaijiaju.cn

[Q85] 数值取整
来源：http://ue.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zp.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://tc.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ow.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://fl.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://th.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://pd.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://to.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yu.gzmigu.cn

[Q89] 判断表是否存在
来源：http://wv.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eg.hahajie.cn

[Q90] 生成序号列
来源：http://yc.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vk.gzmigu.cn

================================================================================
来源：http://hs.bookmarksfly.cn

R. Bash 专题
来源：http://pe.gzmigu.cn

================================================================================
来源：http://lv.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://gx.szxytkj.cn

#!/usr/bin/env bash
来源：http://ib.hahajie.cn

set -euo pipefail
来源：http://ss.hnjuh.cn

[R02] 变量赋值与使用
来源：http://ac.lnxyls.cn

name="Tom"; echo "$name"
来源：http://qu.hnjuh.cn

[R03] 只读变量
来源：http://pg.nicolike.cn

readonly PI=3.14
来源：http://rg.9csxet.cn

[R04] 位置参数
来源：http://zx.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ok.szsharing.cn

[R05] 参数默认值
来源：http://dd.hahajie.cn

name="${1:-default}"
来源：http://lu.panjiajie.cn

[R06] 判断命令是否存在
来源：http://yn.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ku.lnxyls.cn

[R07] if 判断文件
来源：http://ub.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pr.521024.cn

[R08] 数值比较
来源：http://vc.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nx.huanxung.cn

[R09] 字符串比较
来源：http://xa.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tl.shxzskj.cn

[R10] 正则匹配
来源：http://pb.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kz.shxzukj.cn

[R11] case 多分支
来源：http://pu.huixinmuqiang.cn

case "$1" in
来源：http://zu.asd995.cn

start) echo "启动" ;;
来源：http://xw.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://az.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://nz.shtwfgs.cn

esac
来源：http://eb.muxihuayi.cn

[R12] for 遍历文件
来源：http://vv.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://jd.jctech888.com.cn

[R13] for 计数循环
来源：http://cb.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://aw.wgjwhj.cn

[R14] C 风格 for
来源：http://qx.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ag.gzmigu.cn

[R15] while 逐行读文件
来源：http://nu.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ui.chemitech.net.cn

[R16] until 等待条件
来源：http://gg.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zz.hnjuh.cn

[R17] 数组定义与取值
来源：http://di.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wp.jianghongdianzi.cn

[R18] 遍历数组
来源：http://bv.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yt.chemitech.net.cn

[R19] 数组长度
来源：http://jp.jctech888.com.cn

echo "${#arr[@]}"
来源：http://rz.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://rd.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kg.lnxyls.cn

[R21] 字符串长度
来源：http://if.shtwfgs.cn

echo "${#s}"
来源：http://sh.asd995.cn

[R22] 截取子串
来源：http://yu.nicolike.cn

echo "${s:0:5}"
来源：http://vq.asd995.cn

[R23] 字符串替换
来源：http://ak.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ol.szsharing.cn

[R24] 大小写转换
来源：http://ul.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wp.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://yt.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://al.bjjhwx.cn

[R26] 命令替换
来源：http://js.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://mh.newstarts.cn

[R27] 算术展开
来源：http://ry.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://so.nicolike.cn

[R28] 浮点运算
来源：http://fq.521024.cn

echo "scale=2; 10/3" | bc
来源：http://ev.bjjhwx.cn

[R29] 定义函数
来源：http://zt.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mf.panjiajie.cn

[R30] 函数返回状态码
来源：http://xg.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ed.wgjwhj.cn

[R31] 局部变量
来源：http://kq.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://fe.hnjuh.cn

[R32] 参数个数校验
来源：http://my.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cy.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://nf.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cn.chemitech.net.cn

[R34] 退出时清理
来源：http://zy.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gp.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://kw.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gk.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://dq.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xt.lnxyls.cn

[R37] 把输出赋给变量
来源：http://rh.jctech888.com.cn

files=$(ls -1)
来源：http://ii.szxytkj.cn

[R38] 管道串联
来源：http://nv.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://vk.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://tu.asd995.cn

cmd > out.log 2>&1
来源：http://md.bookmarksfly.cn

[R40] 追加写日志
来源：http://gi.bookmarksfly.cn

echo "log" >> out.log
来源：http://kk.szxytkj.cn

[R41] 丢弃输出
来源：http://pv.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://td.szxytkj.cn

[R42] 输入重定向
来源：http://xc.chemitech.net.cn

wc -l < a.txt
来源：http://ps.gzmigu.cn

[R43] 按名字查找文件
来源：http://ex.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://nc.panjiajie.cn

[R44] 按修改时间查找
来源：http://ln.newstarts.cn

find . -mtime -7 -type f
来源：http://rk.shxzukj.cn

[R45] 批量删除
来源：http://of.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://bp.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://yo.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ro.asd995.cn

[R47] sed 单行替换
来源：http://au.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ol.shxzskj.cn

[R48] awk 取指定列
来源：http://kx.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://bd.newstarts.cn

[R49] awk 带条件
来源：http://bb.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ih.9csxet.cn

[R50] awk 求和
来源：http://kc.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sg.lnxyls.cn

[R51] 排序去重取前几
来源：http://ns.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hq.9csxet.cn

[R52] 统计行数
来源：http://vw.jianghongdianzi.cn

wc -l a.txt
来源：http://jr.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://os.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ai.asd995.cn

[R54] 比较两个文件
来源：http://ev.nicolike.cn

diff a.txt b.txt
来源：http://vf.haigaiapp.cn

[R55] 压缩与解压
来源：http://yb.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dg.szxytkj.cn

[R56] 远程拷贝
来源：http://gk.szxytkj.cn

scp file user@host:/path/
来源：http://rt.yuexingan06.cn

[R57] 远程执行命令
来源：http://vg.hnjuh.cn

ssh user@host 'uptime'
来源：http://ut.hahajie.cn

[R58] 下载文件
来源：http://zh.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tr.muxihuayi.cn

[R59] 发 POST JSON
来源：http://ne.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yu.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://qi.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://df.muxihuayi.cn

[R61] 磁盘占用
来源：http://cy.haigaiapp.cn

df -h;  du -sh *
来源：http://dc.lnxyls.cn

[R62] 找最占空间的文件
来源：http://mo.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://lq.yuntaijiaju.cn

[R63] 内存与进程
来源：http://ia.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://rd.muxihuayi.cn

[R64] 结束进程
来源：http://ay.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://cj.szsharing.cn

[R65] 查看端口占用
来源：http://dm.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ig.yuntaijiaju.cn

[R66] 定时任务
来源：http://qc.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://ie.newstarts.cn

[R67] 生成随机十六进制串
来源：http://dy.szsharing.cn

openssl rand -hex 16
来源：http://up.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://sp.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kb.shxzskj.cn

[R69] 生成随机密码
来源：http://jv.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://lk.jctech888.com.cn

[R70] 时间戳与互转
来源：http://sh.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://kh.huixinmuqiang.cn

[R71] 日期格式化
来源：http://tn.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ux.yuexingan06.cn

[R72] 等待端口就绪
来源：http://bd.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cl.panjiajie.cn

[R73] 分割大日志
来源：http://jx.nszjky.cn

split -l 1000 big.log part_
来源：http://bz.hahajie.cn

[R74] 批量重命名
来源：http://hh.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gh.yuexingan06.cn

[R75] 导出环境变量
来源：http://sv.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://cs.bookmarksfly.cn

[R76] 使用临时文件
来源：http://rm.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qu.shxzskj.cn

[R77] 读取用户输入
来源：http://gq.colortex.cn

read -rp "请输入: " ans
来源：http://sv.muxihuayi.cn

[R78] 交互式菜单
来源：http://xo.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lu.huanxung.cn

[R79] 解析命令行选项
来源：http://tc.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nc.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://wg.haigaiapp.cn

time ./run.sh
来源：http://jt.hahajie.cn

================================================================================
来源：http://de.nicolike.cn

S. C / C++ 专题
来源：http://yf.newstarts.cn

================================================================================
来源：http://tp.newstarts.cn

[S01] C：Hello World
来源：http://sh.yuexingan06.cn

#include <stdio.h>
来源：http://kj.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dk.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://wn.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://vk.yuntaijiaju.cn

[S03] C：读入整数
来源：http://se.nszjky.cn

int x; scanf("%d", &x);
来源：http://nd.hnjuh.cn

[S04] C：字符串复制
来源：http://am.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gk.huanxung.cn

[S05] C：字符串长度
来源：http://fe.wgjwhj.cn

strlen(s)
来源：http://pq.hnjuh.cn

[S06] C：字符串比较
来源：http://gu.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://tl.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://bm.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yl.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://fa.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cs.521024.cn

[S09] C：结构体定义与初始化
来源：http://fx.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tg.nicolike.cn

[S10] C：指针与解引用
来源：http://wk.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://ay.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://fi.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://qm.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kc.muxihuayi.cn

fclose(f);
来源：http://jk.newstarts.cn

[S12] C：写文件
来源：http://bu.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sb.bookmarksfly.cn

[S13] C：宏定义
来源：http://lk.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nc.nszjky.cn

[S14] C：枚举
来源：http://ej.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://ib.szxytkj.cn

[S15] C：类型转换
来源：http://de.lnxyls.cn

(double) a / b
来源：http://zh.shxzskj.cn

[S16] C：位操作置位
来源：http://zd.nszjky.cn

x |= (1 << 3);
来源：http://dr.9csxet.cn

[S17] C：安全拼接字符串
来源：http://iv.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qf.szsharing.cn

[S18] C：命令行参数
来源：http://go.yuexingan06.cn

int main(int argc, char **argv)
来源：http://nt.hnjuh.cn

[S19] C：快速排序
来源：http://zx.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cj.haigaiapp.cn

[S20] C：二分查找
来源：http://lr.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pk.yuexingan06.cn

[S21] C：字符类别判断
来源：http://ik.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hf.shxzskj.cn

[S22] C：字符串转数字
来源：http://ks.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pk.asd995.cn

[S23] C：随机数
来源：http://eo.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ea.szxytkj.cn

[S24] C：获取本地时间
来源：http://xv.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bj.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://df.shxzskj.cn

memcpy(dst, src, n);
来源：http://bv.huixinmuqiang.cn

[S26] C：内存清零
来源：http://ov.521024.cn

memset(a, 0, sizeof a);
来源：http://be.yuexingan06.cn

[S27] C：定义常量
来源：http://vt.bjjhwx.cn

const double PI = 3.14159;
来源：http://lz.haigaiapp.cn

[S28] C：静态变量
来源：http://mk.shtwfgs.cn

static int counter = 0;
来源：http://bd.szsharing.cn

[S29] C：变参函数
来源：http://tg.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ap.colortex.cn

[S30] C：头文件保护
来源：http://fc.szsharing.cn

#ifndef X_H
来源：http://kc.nicolike.cn

#define X_H
来源：http://cs.hahajie.cn

#endif
来源：http://kq.hahajie.cn

[S31] C++：Hello World
来源：http://zo.panjiajie.cn

#include <iostream>
来源：http://pc.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://oi.lnxyls.cn

[S32] C++：字符串
来源：http://nz.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://ql.lnxyls.cn

[S33] C++：vector 增删
来源：http://cq.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ck.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://en.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://hd.hnjuh.cn

[S35] C++：map
来源：http://mf.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ou.yuexingan06.cn

[S36] C++：unordered_map
来源：http://hw.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gg.bjjhwx.cn

[S37] C++：set
来源：http://nn.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rh.521024.cn

[S38] C++：排序
来源：http://zr.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://mx.521024.cn

[S39] C++：自定义比较器排序
来源：http://te.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sv.bjjhwx.cn

[S40] C++：查找元素
来源：http://lx.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gh.shxzskj.cn

[S41] C++：类与构造函数
来源：http://gz.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zw.nszjky.cn

[S42] C++：继承与虚函数
来源：http://gr.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://za.muxihuayi.cn

[S43] C++：智能指针
来源：http://dd.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://pu.bookmarksfly.cn

[S44] C++：引用传参
来源：http://tp.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://mc.muxihuayi.cn

[S45] C++：lambda
来源：http://lx.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bh.huanxung.cn

[S46] C++：函数模板
来源：http://yy.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zd.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://lt.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ae.asd995.cn

[S48] C++：逐行读文件
来源：http://ff.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zl.9csxet.cn

while (std::getline(in, line)) { }
来源：http://vp.jctech888.com.cn

[S49] C++：写文件
来源：http://ga.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wc.szsharing.cn

[S50] C++：格式化数字
来源：http://cg.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mk.hnjuh.cn

[S51] C++：显式类型转换
来源：http://yj.nszjky.cn

static_cast<double>(a) / b
来源：http://at.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://fu.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://nd.hnjuh.cn

[S53] C++：移动语义
来源：http://ki.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://ga.wgjwhj.cn

[S54] C++：异常处理
来源：http://ql.yuexingan06.cn


<!-- 参考信息 -->