代发 wailian999

[Q82] 字符长度与字节长度
来源：http://wj.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lv.szsharing.cn

[Q83] 大小写转换
来源：http://eo.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lg.newstarts.cn

[Q84] 去除首尾空格
来源：http://ci.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://ej.jctech888.com.cn

[Q85] 数值取整
来源：http://uy.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fk.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://ii.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xn.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://cj.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tn.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://sx.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dn.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://of.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://bj.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gp.jctech888.com.cn

[Q90] 生成序号列
来源：http://zv.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ql.bjjhwx.cn

================================================================================
来源：http://se.muxihuayi.cn

R. Bash 专题
来源：http://dv.shtwfgs.cn

================================================================================
来源：http://vm.newstarts.cn

[R01] shebang 与严格模式
来源：http://ef.huanxung.cn

#!/usr/bin/env bash
来源：http://yg.huixinmuqiang.cn

set -euo pipefail
来源：http://at.nicolike.cn

[R02] 变量赋值与使用
来源：http://mb.lnxyls.cn

name="Tom"; echo "$name"
来源：http://cb.yuexingan06.cn

[R03] 只读变量
来源：http://ni.panjiajie.cn

readonly PI=3.14
来源：http://rh.chemitech.net.cn

[R04] 位置参数
来源：http://sl.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://di.521024.cn

[R05] 参数默认值
来源：http://xx.shxzskj.cn

name="${1:-default}"
来源：http://ev.newstarts.cn

[R06] 判断命令是否存在
来源：http://sx.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ig.haigaiapp.cn

[R07] if 判断文件
来源：http://oc.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wt.huixinmuqiang.cn

[R08] 数值比较
来源：http://ri.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oo.shxzukj.cn

[R09] 字符串比较
来源：http://xb.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wp.bookmarksfly.cn

[R10] 正则匹配
来源：http://mk.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xo.nszjky.cn

[R11] case 多分支
来源：http://nc.chemitech.net.cn

case "$1" in
来源：http://ve.panjiajie.cn

start) echo "启动" ;;
来源：http://hh.szxytkj.cn

stop)  echo "停止" ;;
来源：http://ca.521024.cn

*)     echo "未知命令" ;;
来源：http://es.newstarts.cn

esac
来源：http://yu.lnxyls.cn

[R12] for 遍历文件
来源：http://lm.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://lq.nszjky.cn

[R13] for 计数循环
来源：http://lo.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://ds.szxytkj.cn

[R14] C 风格 for
来源：http://zw.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mb.panjiajie.cn

[R15] while 逐行读文件
来源：http://cg.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sg.wgjwhj.cn

[R16] until 等待条件
来源：http://er.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wi.yuexingan06.cn

[R17] 数组定义与取值
来源：http://kw.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://px.jianghongdianzi.cn

[R18] 遍历数组
来源：http://sz.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lz.nicolike.cn

[R19] 数组长度
来源：http://kd.colortex.cn

echo "${#arr[@]}"
来源：http://co.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://vh.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lj.bjjhwx.cn

[R21] 字符串长度
来源：http://ys.jianghongdianzi.cn

echo "${#s}"
来源：http://gf.shtwfgs.cn

[R22] 截取子串
来源：http://ua.wgjwhj.cn

echo "${s:0:5}"
来源：http://av.bjjhwx.cn

[R23] 字符串替换
来源：http://km.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://an.szsharing.cn

[R24] 大小写转换
来源：http://ml.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tw.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://vm.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uf.jctech888.com.cn

[R26] 命令替换
来源：http://hl.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://yu.asd995.cn

[R27] 算术展开
来源：http://ki.9csxet.cn

echo $((1 + 2 * 3))
来源：http://ns.shtwfgs.cn

[R28] 浮点运算
来源：http://mh.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://sy.yuexingan06.cn

[R29] 定义函数
来源：http://li.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oi.chemitech.net.cn

[R30] 函数返回状态码
来源：http://hr.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://cb.nszjky.cn

[R31] 局部变量
来源：http://ae.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://ul.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://ad.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pl.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://ui.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gl.shxzskj.cn

[R34] 退出时清理
来源：http://ln.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cj.hnjuh.cn

[R35] 后台执行并等待
来源：http://ol.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ir.hahajie.cn

[R36] 并发执行多个任务
来源：http://xg.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iy.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://zz.nszjky.cn

files=$(ls -1)
来源：http://vo.gzmigu.cn

[R38] 管道串联
来源：http://lr.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://xo.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://mu.huanxung.cn

cmd > out.log 2>&1
来源：http://zh.yuexingan06.cn

[R40] 追加写日志
来源：http://wo.wgjwhj.cn

echo "log" >> out.log
来源：http://uz.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://ti.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://ds.chemitech.net.cn

[R42] 输入重定向
来源：http://mi.hnjuh.cn

wc -l < a.txt
来源：http://uy.hnjuh.cn

[R43] 按名字查找文件
来源：http://tv.521024.cn

find . -name "*.log" -type f
来源：http://dt.colortex.cn

[R44] 按修改时间查找
来源：http://df.nszjky.cn

find . -mtime -7 -type f
来源：http://pv.shtwfgs.cn

[R45] 批量删除
来源：http://sa.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://tx.nszjky.cn

[R46] 递归替换文件内容
来源：http://wr.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qp.bjjhwx.cn

[R47] sed 单行替换
来源：http://rv.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vt.bookmarksfly.cn

[R48] awk 取指定列
来源：http://ya.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://gb.chemitech.net.cn

[R49] awk 带条件
来源：http://ys.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ay.huixiangedu.cn

[R50] awk 求和
来源：http://bw.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bo.wgjwhj.cn

[R51] 排序去重取前几
来源：http://eo.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ip.521024.cn

[R52] 统计行数
来源：http://oq.newstarts.cn

wc -l a.txt
来源：http://jj.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://qh.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lm.chemitech.net.cn

[R54] 比较两个文件
来源：http://qk.haigaiapp.cn

diff a.txt b.txt
来源：http://hm.szxytkj.cn

[R55] 压缩与解压
来源：http://bd.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mc.gzmigu.cn

[R56] 远程拷贝
来源：http://vf.hnjuh.cn

scp file user@host:/path/
来源：http://nf.colortex.cn

[R57] 远程执行命令
来源：http://pb.9csxet.cn

ssh user@host 'uptime'
来源：http://ch.muxihuayi.cn

[R58] 下载文件
来源：http://pu.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fa.gzmigu.cn

[R59] 发 POST JSON
来源：http://em.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dq.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://cp.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://st.bjjhwx.cn

[R61] 磁盘占用
来源：http://ez.shxzukj.cn

df -h;  du -sh *
来源：http://lu.lnxyls.cn

[R62] 找最占空间的文件
来源：http://cz.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://iq.nicolike.cn

[R63] 内存与进程
来源：http://pg.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://pj.shxzskj.cn

[R64] 结束进程
来源：http://fh.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://ou.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://xv.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zm.lnxyls.cn

[R66] 定时任务
来源：http://gu.jctech888.com.cn

crontab -e;  crontab -l
来源：http://mx.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://rp.haigaiapp.cn

openssl rand -hex 16
来源：http://sr.colortex.cn

[R68] 计算文件校验值
来源：http://vd.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tx.hnjuh.cn

[R69] 生成随机密码
来源：http://bl.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://jm.nicolike.cn

[R70] 时间戳与互转
来源：http://db.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://fh.szsharing.cn

[R71] 日期格式化
来源：http://zc.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fm.chemitech.net.cn

[R72] 等待端口就绪
来源：http://ba.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yv.chemitech.net.cn

[R73] 分割大日志
来源：http://bu.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://tw.jianghongdianzi.cn

[R74] 批量重命名
来源：http://ec.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jd.wgjwhj.cn

[R75] 导出环境变量
来源：http://iu.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://pi.9csxet.cn

[R76] 使用临时文件
来源：http://ke.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yl.shtwfgs.cn

[R77] 读取用户输入
来源：http://ci.huanxung.cn

read -rp "请输入: " ans
来源：http://ki.szxytkj.cn

[R78] 交互式菜单
来源：http://sf.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ar.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://jq.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mc.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://sn.lnxyls.cn

time ./run.sh
来源：http://cw.shxzskj.cn

================================================================================
来源：http://ja.jianghongdianzi.cn

S. C / C++ 专题
来源：http://in.asd995.cn

================================================================================
来源：http://ro.newstarts.cn

[S01] C：Hello World
来源：http://gz.chemitech.net.cn

#include <stdio.h>
来源：http://zp.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iq.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://sg.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://vb.shxzukj.cn

[S03] C：读入整数
来源：http://fm.huanxung.cn

int x; scanf("%d", &x);
来源：http://ws.colortex.cn

[S04] C：字符串复制
来源：http://zm.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nd.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://xe.jianghongdianzi.cn

strlen(s)
来源：http://jl.huixiangedu.cn

[S06] C：字符串比较
来源：http://oz.shxzukj.cn

strcmp(a, b) == 0
来源：http://nc.panjiajie.cn

[S07] C：数组遍历求和
来源：http://pu.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lh.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://hp.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xf.asd995.cn

[S09] C：结构体定义与初始化
来源：http://nb.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bk.lnxyls.cn

[S10] C：指针与解引用
来源：http://pa.newstarts.cn

int *p = &a;  *p = 5;
来源：http://fd.szxytkj.cn

[S11] C：逐行读文件
来源：http://gf.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://bw.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ru.yuntaijiaju.cn

fclose(f);
来源：http://cj.newstarts.cn

[S12] C：写文件
来源：http://vc.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zl.yuexingan06.cn

[S13] C：宏定义
来源：http://vw.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cj.hahajie.cn

[S14] C：枚举
来源：http://bx.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://xh.colortex.cn

[S15] C：类型转换
来源：http://et.huixiangedu.cn

(double) a / b
来源：http://mr.jctech888.com.cn

[S16] C：位操作置位
来源：http://ze.muxihuayi.cn

x |= (1 << 3);
来源：http://we.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://hq.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mb.wgjwhj.cn

[S18] C：命令行参数
来源：http://bc.asd995.cn

int main(int argc, char **argv)
来源：http://os.huixiangedu.cn

[S19] C：快速排序
来源：http://ra.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ka.shxzskj.cn

[S20] C：二分查找
来源：http://qr.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ir.nicolike.cn

[S21] C：字符类别判断
来源：http://vq.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ni.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://zp.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ms.jianghongdianzi.cn

[S23] C：随机数
来源：http://nd.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rt.huixiangedu.cn

[S24] C：获取本地时间
来源：http://yu.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zn.asd995.cn

[S25] C：内存拷贝
来源：http://jw.szsharing.cn

memcpy(dst, src, n);
来源：http://hu.colortex.cn

[S26] C：内存清零
来源：http://oc.newstarts.cn

memset(a, 0, sizeof a);
来源：http://pr.wgjwhj.cn

[S27] C：定义常量
来源：http://hg.bjjhwx.cn

const double PI = 3.14159;
来源：http://lx.yuexingan06.cn

[S28] C：静态变量
来源：http://hb.hnjuh.cn

static int counter = 0;
来源：http://sn.szxytkj.cn

[S29] C：变参函数
来源：http://jn.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xl.shxzukj.cn

[S30] C：头文件保护
来源：http://to.bjjhwx.cn

#ifndef X_H
来源：http://kz.colortex.cn

#define X_H
来源：http://ja.lnxyls.cn

#endif
来源：http://xt.wgjwhj.cn

[S31] C++：Hello World
来源：http://kp.colortex.cn

#include <iostream>
来源：http://mg.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://lk.haigaiapp.cn

[S32] C++：字符串
来源：http://bh.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://la.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://ah.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ow.shxzskj.cn

[S34] C++：遍历 vector
来源：http://wf.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://vi.nicolike.cn

[S35] C++：map
来源：http://nv.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ne.szsharing.cn

[S36] C++：unordered_map
来源：http://ob.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gn.huixiangedu.cn

[S37] C++：set
来源：http://xm.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pl.huixiangedu.cn

[S38] C++：排序
来源：http://uc.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://sq.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://lc.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ip.nicolike.cn

[S40] C++：查找元素
来源：http://ww.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rz.shxzukj.cn

[S41] C++：类与构造函数
来源：http://pr.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lp.9csxet.cn

[S42] C++：继承与虚函数
来源：http://ex.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://ln.huixiangedu.cn

[S43] C++：智能指针
来源：http://bx.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://mg.yuexingan06.cn

[S44] C++：引用传参
来源：http://lu.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://yr.szsharing.cn

[S45] C++：lambda
来源：http://ge.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wp.bjjhwx.cn

[S46] C++：函数模板
来源：http://qu.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xx.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://uq.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mj.hnjuh.cn

[S48] C++：逐行读文件
来源：http://kl.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jn.521024.cn

while (std::getline(in, line)) { }
来源：http://bq.asd995.cn

[S49] C++：写文件
来源：http://dh.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ek.521024.cn

[S50] C++：格式化数字
来源：http://vc.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mj.shxzskj.cn

[S51] C++：显式类型转换
来源：http://rc.yuexingan06.cn

static_cast<double>(a) / b
来源：http://gk.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://th.nicolike.cn


<!-- 参考信息 -->