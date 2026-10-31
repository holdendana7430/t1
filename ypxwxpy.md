代发 wailian999

[Q84] 去除首尾空格
来源：http://ir.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://nf.bookmarksfly.cn

[Q85] 数值取整
来源：http://ke.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://su.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://rz.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ao.asd995.cn

[Q87] JSON 字段做条件
来源：http://xa.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wd.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://jx.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fd.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://it.521024.cn

[Q89] 判断表是否存在
来源：http://lz.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lz.gzmigu.cn

[Q90] 生成序号列
来源：http://nf.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fy.szxytkj.cn

================================================================================
来源：http://ha.nicolike.cn

R. Bash 专题
来源：http://wl.szsharing.cn

================================================================================
来源：http://wh.panjiajie.cn

[R01] shebang 与严格模式
来源：http://al.muxihuayi.cn

#!/usr/bin/env bash
来源：http://vh.lnxyls.cn

set -euo pipefail
来源：http://xk.panjiajie.cn

[R02] 变量赋值与使用
来源：http://ls.shxzskj.cn

name="Tom"; echo "$name"
来源：http://er.colortex.cn

[R03] 只读变量
来源：http://ah.521024.cn

readonly PI=3.14
来源：http://qb.huanxung.cn

[R04] 位置参数
来源：http://li.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://of.nszjky.cn

[R05] 参数默认值
来源：http://cr.lnxyls.cn

name="${1:-default}"
来源：http://ep.szsharing.cn

[R06] 判断命令是否存在
来源：http://sr.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ij.shxzskj.cn

[R07] if 判断文件
来源：http://cm.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ze.nszjky.cn

[R08] 数值比较
来源：http://mc.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qm.521024.cn

[R09] 字符串比较
来源：http://zq.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vf.jctech888.com.cn

[R10] 正则匹配
来源：http://bk.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://da.szxytkj.cn

[R11] case 多分支
来源：http://mc.szsharing.cn

case "$1" in
来源：http://dt.asd995.cn

start) echo "启动" ;;
来源：http://oc.hahajie.cn

stop)  echo "停止" ;;
来源：http://gd.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://qs.nicolike.cn

esac
来源：http://tf.9csxet.cn

[R12] for 遍历文件
来源：http://de.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://yx.muxihuayi.cn

[R13] for 计数循环
来源：http://at.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://tb.jianghongdianzi.cn

[R14] C 风格 for
来源：http://rr.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ap.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://vs.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nt.chemitech.net.cn

[R16] until 等待条件
来源：http://xf.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pc.shtwfgs.cn

[R17] 数组定义与取值
来源：http://gz.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://db.nicolike.cn

[R18] 遍历数组
来源：http://ul.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eu.newstarts.cn

[R19] 数组长度
来源：http://zq.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://uo.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://qe.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://so.bookmarksfly.cn

[R21] 字符串长度
来源：http://hb.panjiajie.cn

echo "${#s}"
来源：http://fe.huixinmuqiang.cn

[R22] 截取子串
来源：http://cn.szxytkj.cn

echo "${s:0:5}"
来源：http://cp.chemitech.net.cn

[R23] 字符串替换
来源：http://ap.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ow.9csxet.cn

[R24] 大小写转换
来源：http://nh.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vh.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://jm.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xe.shxzskj.cn

[R26] 命令替换
来源：http://zm.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://wn.bjjhwx.cn

[R27] 算术展开
来源：http://vr.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://xp.wgjwhj.cn

[R28] 浮点运算
来源：http://yx.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://tg.huanxung.cn

[R29] 定义函数
来源：http://ww.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fa.yuexingan06.cn

[R30] 函数返回状态码
来源：http://lq.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://sw.bjjhwx.cn

[R31] 局部变量
来源：http://an.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://nj.hahajie.cn

[R32] 参数个数校验
来源：http://ky.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yg.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://df.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yo.shxzukj.cn

[R34] 退出时清理
来源：http://ta.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pw.muxihuayi.cn

[R35] 后台执行并等待
来源：http://ft.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zm.szxytkj.cn

[R36] 并发执行多个任务
来源：http://bn.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ih.huanxung.cn

[R37] 把输出赋给变量
来源：http://mr.hnjuh.cn

files=$(ls -1)
来源：http://ec.huanxung.cn

[R38] 管道串联
来源：http://yh.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://ld.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://qo.newstarts.cn

cmd > out.log 2>&1
来源：http://fp.nszjky.cn

[R40] 追加写日志
来源：http://mo.521024.cn

echo "log" >> out.log
来源：http://mc.muxihuayi.cn

[R41] 丢弃输出
来源：http://cx.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://om.muxihuayi.cn

[R42] 输入重定向
来源：http://tf.shxzskj.cn

wc -l < a.txt
来源：http://fb.9csxet.cn

[R43] 按名字查找文件
来源：http://tu.szxytkj.cn

find . -name "*.log" -type f
来源：http://vz.nicolike.cn

[R44] 按修改时间查找
来源：http://oi.wgjwhj.cn

find . -mtime -7 -type f
来源：http://yr.huixiangedu.cn

[R45] 批量删除
来源：http://yy.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://ys.szxytkj.cn

[R46] 递归替换文件内容
来源：http://ht.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dt.huanxung.cn

[R47] sed 单行替换
来源：http://jo.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ls.bjjhwx.cn

[R48] awk 取指定列
来源：http://ed.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://wb.szsharing.cn

[R49] awk 带条件
来源：http://ez.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rd.asd995.cn

[R50] awk 求和
来源：http://kx.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ho.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://iu.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gk.nszjky.cn

[R52] 统计行数
来源：http://wt.hnjuh.cn

wc -l a.txt
来源：http://ct.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://dr.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bc.nicolike.cn

[R54] 比较两个文件
来源：http://wl.9csxet.cn

diff a.txt b.txt
来源：http://iz.panjiajie.cn

[R55] 压缩与解压
来源：http://ao.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ff.lnxyls.cn

[R56] 远程拷贝
来源：http://zl.panjiajie.cn

scp file user@host:/path/
来源：http://ve.nszjky.cn

[R57] 远程执行命令
来源：http://xm.haigaiapp.cn

ssh user@host 'uptime'
来源：http://dx.hnjuh.cn

[R58] 下载文件
来源：http://qn.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sb.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://gr.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dg.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://df.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mk.hnjuh.cn

[R61] 磁盘占用
来源：http://ju.nicolike.cn

df -h;  du -sh *
来源：http://nc.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://pj.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://cm.newstarts.cn

[R63] 内存与进程
来源：http://zd.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://fs.gzmigu.cn

[R64] 结束进程
来源：http://fl.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://rf.nicolike.cn

[R65] 查看端口占用
来源：http://zz.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ou.haigaiapp.cn

[R66] 定时任务
来源：http://yj.yuexingan06.cn

crontab -e;  crontab -l
来源：http://xg.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://pp.521024.cn

openssl rand -hex 16
来源：http://lz.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://oe.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nd.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://wy.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://gh.haigaiapp.cn

[R70] 时间戳与互转
来源：http://dt.colortex.cn

date +%s;  date -d @1700000000
来源：http://pj.huixiangedu.cn

[R71] 日期格式化
来源：http://sy.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wq.shxzukj.cn

[R72] 等待端口就绪
来源：http://xm.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wh.9csxet.cn

[R73] 分割大日志
来源：http://dz.yuexingan06.cn

split -l 1000 big.log part_
来源：http://el.hnjuh.cn

[R74] 批量重命名
来源：http://vl.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lu.hahajie.cn

[R75] 导出环境变量
来源：http://rj.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://mj.nicolike.cn

[R76] 使用临时文件
来源：http://xe.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xk.panjiajie.cn

[R77] 读取用户输入
来源：http://gd.hahajie.cn

read -rp "请输入: " ans
来源：http://ze.hnjuh.cn

[R78] 交互式菜单
来源：http://ts.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://il.huanxung.cn

[R79] 解析命令行选项
来源：http://fm.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bd.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://ez.jctech888.com.cn

time ./run.sh
来源：http://cd.shxzskj.cn

================================================================================
来源：http://ip.yuntaijiaju.cn

S. C / C++ 专题
来源：http://vv.nicolike.cn

================================================================================
来源：http://sg.hahajie.cn

[S01] C：Hello World
来源：http://ow.chemitech.net.cn

#include <stdio.h>
来源：http://kb.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://he.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://hk.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://qg.jctech888.com.cn

[S03] C：读入整数
来源：http://vw.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://wc.szxytkj.cn

[S04] C：字符串复制
来源：http://vb.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tv.huixiangedu.cn

[S05] C：字符串长度
来源：http://ey.wgjwhj.cn

strlen(s)
来源：http://jz.bjjhwx.cn

[S06] C：字符串比较
来源：http://zz.hahajie.cn

strcmp(a, b) == 0
来源：http://ju.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://nb.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mt.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://bx.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hr.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://mb.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vb.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://po.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://hv.hnjuh.cn

[S11] C：逐行读文件
来源：http://ae.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://ir.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rx.chemitech.net.cn

fclose(f);
来源：http://br.jctech888.com.cn

[S12] C：写文件
来源：http://vk.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xn.shxzskj.cn

[S13] C：宏定义
来源：http://ym.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qz.lnxyls.cn

[S14] C：枚举
来源：http://sf.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://ui.colortex.cn

[S15] C：类型转换
来源：http://tu.muxihuayi.cn

(double) a / b
来源：http://gp.haigaiapp.cn

[S16] C：位操作置位
来源：http://ke.wgjwhj.cn

x |= (1 << 3);
来源：http://st.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://lc.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ki.wgjwhj.cn

[S18] C：命令行参数
来源：http://go.szxytkj.cn

int main(int argc, char **argv)
来源：http://od.hahajie.cn

[S19] C：快速排序
来源：http://jg.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dr.hnjuh.cn

[S20] C：二分查找
来源：http://nz.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dd.newstarts.cn

[S21] C：字符类别判断
来源：http://xw.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dr.huixiangedu.cn

[S22] C：字符串转数字
来源：http://wn.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dx.yuntaijiaju.cn

[S23] C：随机数
来源：http://rh.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qs.nicolike.cn

[S24] C：获取本地时间
来源：http://yd.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fw.muxihuayi.cn

[S25] C：内存拷贝
来源：http://du.colortex.cn

memcpy(dst, src, n);
来源：http://dy.9csxet.cn

[S26] C：内存清零
来源：http://em.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://su.521024.cn

[S27] C：定义常量
来源：http://me.szxytkj.cn

const double PI = 3.14159;
来源：http://tw.521024.cn

[S28] C：静态变量
来源：http://rm.chemitech.net.cn

static int counter = 0;
来源：http://ah.lnxyls.cn

[S29] C：变参函数
来源：http://uz.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ln.lnxyls.cn

[S30] C：头文件保护
来源：http://rv.newstarts.cn

#ifndef X_H
来源：http://dx.jctech888.com.cn

#define X_H
来源：http://xr.gzmigu.cn

#endif
来源：http://va.hahajie.cn

[S31] C++：Hello World
来源：http://xv.chemitech.net.cn

#include <iostream>
来源：http://lm.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://xe.chemitech.net.cn

[S32] C++：字符串
来源：http://hf.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://zw.chemitech.net.cn

[S33] C++：vector 增删
来源：http://sa.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yo.9csxet.cn

[S34] C++：遍历 vector
来源：http://kj.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://vh.bookmarksfly.cn

[S35] C++：map
来源：http://ii.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dc.9csxet.cn

[S36] C++：unordered_map
来源：http://hk.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wr.panjiajie.cn

[S37] C++：set
来源：http://ei.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ib.wgjwhj.cn

[S38] C++：排序
来源：http://gt.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://tj.asd995.cn

[S39] C++：自定义比较器排序
来源：http://vv.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lk.521024.cn

[S40] C++：查找元素
来源：http://zc.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qx.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://kl.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://is.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://in.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://se.szsharing.cn

[S43] C++：智能指针
来源：http://kn.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://cx.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://jt.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://xe.gzmigu.cn

[S45] C++：lambda
来源：http://lh.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://se.shxzskj.cn

[S46] C++：函数模板
来源：http://vv.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gn.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://sm.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xy.hnjuh.cn

[S48] C++：逐行读文件
来源：http://hu.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cg.asd995.cn

while (std::getline(in, line)) { }
来源：http://ez.asd995.cn

[S49] C++：写文件
来源：http://qw.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fx.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://ow.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dq.hahajie.cn

[S51] C++：显式类型转换
来源：http://nl.newstarts.cn

static_cast<double>(a) / b
来源：http://wj.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://xq.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://ok.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://ss.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://dg.shxzskj.cn

[S54] C++：异常处理
来源：http://gu.asd995.cn


<!-- 参考信息 -->