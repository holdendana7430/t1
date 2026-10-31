代发 wailian999

[Q78] 当前时间
来源：http://dg.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://md.9csxet.cn

[Q79] 字符串拼接
来源：http://uu.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wg.huixiangedu.cn

[Q80] 字符串截取
来源：http://ya.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hf.bookmarksfly.cn

[Q81] 字符串替换
来源：http://er.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tg.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://lk.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bx.szsharing.cn

[Q83] 大小写转换
来源：http://sk.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qu.521024.cn

[Q84] 去除首尾空格
来源：http://uc.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://su.gzmigu.cn

[Q85] 数值取整
来源：http://hg.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ml.colortex.cn

[Q86] 读取 JSON 字段
来源：http://ef.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kk.asd995.cn

[Q87] JSON 字段做条件
来源：http://xs.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jv.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://ex.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fp.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xj.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://jq.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sy.hnjuh.cn

[Q90] 生成序号列
来源：http://eo.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ra.hnjuh.cn

================================================================================
来源：http://ks.huixiangedu.cn

R. Bash 专题
来源：http://mi.jianghongdianzi.cn

================================================================================
来源：http://fe.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://ln.bjjhwx.cn

#!/usr/bin/env bash
来源：http://js.nicolike.cn

set -euo pipefail
来源：http://oz.newstarts.cn

[R02] 变量赋值与使用
来源：http://qb.nszjky.cn

name="Tom"; echo "$name"
来源：http://aj.9csxet.cn

[R03] 只读变量
来源：http://lu.bjjhwx.cn

readonly PI=3.14
来源：http://li.nicolike.cn

[R04] 位置参数
来源：http://sl.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ge.huixinmuqiang.cn

[R05] 参数默认值
来源：http://xq.haigaiapp.cn

name="${1:-default}"
来源：http://an.hnjuh.cn

[R06] 判断命令是否存在
来源：http://kd.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wo.9csxet.cn

[R07] if 判断文件
来源：http://lc.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://as.hahajie.cn

[R08] 数值比较
来源：http://vw.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ac.jianghongdianzi.cn

[R09] 字符串比较
来源：http://ei.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yk.shtwfgs.cn

[R10] 正则匹配
来源：http://mf.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hp.shxzskj.cn

[R11] case 多分支
来源：http://tb.shxzskj.cn

case "$1" in
来源：http://xk.colortex.cn

start) echo "启动" ;;
来源：http://zr.panjiajie.cn

stop)  echo "停止" ;;
来源：http://bk.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://pt.szxytkj.cn

esac
来源：http://zp.lnxyls.cn

[R12] for 遍历文件
来源：http://vr.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://ty.bjjhwx.cn

[R13] for 计数循环
来源：http://pu.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://jk.521024.cn

[R14] C 风格 for
来源：http://cc.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tw.521024.cn

[R15] while 逐行读文件
来源：http://vp.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ud.wgjwhj.cn

[R16] until 等待条件
来源：http://wd.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yw.shxzskj.cn

[R17] 数组定义与取值
来源：http://fy.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qb.szsharing.cn

[R18] 遍历数组
来源：http://qk.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xb.szxytkj.cn

[R19] 数组长度
来源：http://xv.colortex.cn

echo "${#arr[@]}"
来源：http://oo.panjiajie.cn

[R20] 关联数组（字典）
来源：http://bx.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bk.521024.cn

[R21] 字符串长度
来源：http://gk.yuntaijiaju.cn

echo "${#s}"
来源：http://ny.muxihuayi.cn

[R22] 截取子串
来源：http://lb.hnjuh.cn

echo "${s:0:5}"
来源：http://sj.panjiajie.cn

[R23] 字符串替换
来源：http://mr.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://od.jianghongdianzi.cn

[R24] 大小写转换
来源：http://oy.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mq.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://uu.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://va.muxihuayi.cn

[R26] 命令替换
来源：http://jb.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://bt.jctech888.com.cn

[R27] 算术展开
来源：http://sa.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://hf.yuntaijiaju.cn

[R28] 浮点运算
来源：http://lr.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://kn.huixiangedu.cn

[R29] 定义函数
来源：http://kr.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gx.shxzukj.cn

[R30] 函数返回状态码
来源：http://tz.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://aa.bjjhwx.cn

[R31] 局部变量
来源：http://px.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://jr.hahajie.cn

[R32] 参数个数校验
来源：http://vc.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iu.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://om.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dh.newstarts.cn

[R34] 退出时清理
来源：http://ot.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jn.nszjky.cn

[R35] 后台执行并等待
来源：http://gh.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cm.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://bl.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nh.521024.cn

[R37] 把输出赋给变量
来源：http://sj.chemitech.net.cn

files=$(ls -1)
来源：http://pj.jctech888.com.cn

[R38] 管道串联
来源：http://rb.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://uo.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://ug.panjiajie.cn

cmd > out.log 2>&1
来源：http://fa.shtwfgs.cn

[R40] 追加写日志
来源：http://li.huixinmuqiang.cn

echo "log" >> out.log
来源：http://dq.panjiajie.cn

[R41] 丢弃输出
来源：http://zv.nszjky.cn

cmd >/dev/null 2>&1
来源：http://hv.asd995.cn

[R42] 输入重定向
来源：http://wx.nszjky.cn

wc -l < a.txt
来源：http://je.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://ly.nicolike.cn

find . -name "*.log" -type f
来源：http://ge.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://re.nszjky.cn

find . -mtime -7 -type f
来源：http://pv.haigaiapp.cn

[R45] 批量删除
来源：http://tf.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://jr.newstarts.cn

[R46] 递归替换文件内容
来源：http://et.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ny.gzmigu.cn

[R47] sed 单行替换
来源：http://hw.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://me.haigaiapp.cn

[R48] awk 取指定列
来源：http://wa.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://kj.shxzukj.cn

[R49] awk 带条件
来源：http://zq.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lm.bjjhwx.cn

[R50] awk 求和
来源：http://ux.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cn.chemitech.net.cn

[R51] 排序去重取前几
来源：http://gu.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wi.huanxung.cn

[R52] 统计行数
来源：http://tm.wgjwhj.cn

wc -l a.txt
来源：http://wu.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://ey.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ae.huixiangedu.cn

[R54] 比较两个文件
来源：http://yy.panjiajie.cn

diff a.txt b.txt
来源：http://vz.wgjwhj.cn

[R55] 压缩与解压
来源：http://xd.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gs.huixiangedu.cn

[R56] 远程拷贝
来源：http://qh.shxzskj.cn

scp file user@host:/path/
来源：http://dc.521024.cn

[R57] 远程执行命令
来源：http://bo.panjiajie.cn

ssh user@host 'uptime'
来源：http://hj.yuexingan06.cn

[R58] 下载文件
来源：http://dr.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://za.shtwfgs.cn

[R59] 发 POST JSON
来源：http://lg.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dg.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://dd.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cn.szsharing.cn

[R61] 磁盘占用
来源：http://da.asd995.cn

df -h;  du -sh *
来源：http://ve.gzmigu.cn

[R62] 找最占空间的文件
来源：http://lv.colortex.cn

du -ah . | sort -rh | head -10
来源：http://kv.szxytkj.cn

[R63] 内存与进程
来源：http://tc.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://zg.nszjky.cn

[R64] 结束进程
来源：http://mh.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://lc.9csxet.cn

[R65] 查看端口占用
来源：http://la.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ky.lnxyls.cn

[R66] 定时任务
来源：http://mt.haigaiapp.cn

crontab -e;  crontab -l
来源：http://bn.colortex.cn

[R67] 生成随机十六进制串
来源：http://vd.huixinmuqiang.cn

openssl rand -hex 16
来源：http://gs.szsharing.cn

[R68] 计算文件校验值
来源：http://gr.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yb.shtwfgs.cn

[R69] 生成随机密码
来源：http://wq.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://pw.huanxung.cn

[R70] 时间戳与互转
来源：http://tr.huanxung.cn

date +%s;  date -d @1700000000
来源：http://es.hahajie.cn

[R71] 日期格式化
来源：http://op.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vu.newstarts.cn

[R72] 等待端口就绪
来源：http://kv.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fx.wgjwhj.cn

[R73] 分割大日志
来源：http://rp.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://ao.huixinmuqiang.cn

[R74] 批量重命名
来源：http://gn.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nu.hahajie.cn

[R75] 导出环境变量
来源：http://kf.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://wc.haigaiapp.cn

[R76] 使用临时文件
来源：http://lx.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tr.shtwfgs.cn

[R77] 读取用户输入
来源：http://bu.haigaiapp.cn

read -rp "请输入: " ans
来源：http://ds.asd995.cn

[R78] 交互式菜单
来源：http://la.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dr.shxzskj.cn

[R79] 解析命令行选项
来源：http://ya.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ws.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://bi.yuntaijiaju.cn

time ./run.sh
来源：http://yt.shxzskj.cn

================================================================================
来源：http://th.panjiajie.cn

S. C / C++ 专题
来源：http://uy.szsharing.cn

================================================================================
来源：http://xd.bookmarksfly.cn

[S01] C：Hello World
来源：http://mk.asd995.cn

#include <stdio.h>
来源：http://qc.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kv.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://dp.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://fl.nicolike.cn

[S03] C：读入整数
来源：http://ga.colortex.cn

int x; scanf("%d", &x);
来源：http://sz.nicolike.cn

[S04] C：字符串复制
来源：http://ny.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wb.szsharing.cn

[S05] C：字符串长度
来源：http://bj.newstarts.cn

strlen(s)
来源：http://ng.muxihuayi.cn

[S06] C：字符串比较
来源：http://bd.hnjuh.cn

strcmp(a, b) == 0
来源：http://ff.521024.cn

[S07] C：数组遍历求和
来源：http://bn.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://db.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://hj.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eo.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://fi.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ab.huixiangedu.cn

[S10] C：指针与解引用
来源：http://le.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://zb.wgjwhj.cn

[S11] C：逐行读文件
来源：http://mo.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://we.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vr.asd995.cn

fclose(f);
来源：http://tv.jctech888.com.cn

[S12] C：写文件
来源：http://fc.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hv.shtwfgs.cn

[S13] C：宏定义
来源：http://yi.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ec.nszjky.cn

[S14] C：枚举
来源：http://ms.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://av.jctech888.com.cn

[S15] C：类型转换
来源：http://me.huanxung.cn

(double) a / b
来源：http://ui.shxzukj.cn

[S16] C：位操作置位
来源：http://ev.jctech888.com.cn

x |= (1 << 3);
来源：http://yh.521024.cn

[S17] C：安全拼接字符串
来源：http://ai.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vw.shxzukj.cn

[S18] C：命令行参数
来源：http://qk.bjjhwx.cn

int main(int argc, char **argv)
来源：http://ax.wgjwhj.cn

[S19] C：快速排序
来源：http://ry.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xn.gzmigu.cn

[S20] C：二分查找
来源：http://qw.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oc.9csxet.cn

[S21] C：字符类别判断
来源：http://dm.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qr.huanxung.cn

[S22] C：字符串转数字
来源：http://wu.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ca.jctech888.com.cn

[S23] C：随机数
来源：http://ca.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vp.szsharing.cn

[S24] C：获取本地时间
来源：http://ix.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jr.bjjhwx.cn

[S25] C：内存拷贝
来源：http://uy.bjjhwx.cn

memcpy(dst, src, n);
来源：http://ne.521024.cn

[S26] C：内存清零
来源：http://dl.521024.cn

memset(a, 0, sizeof a);
来源：http://gf.shxzukj.cn

[S27] C：定义常量
来源：http://oq.shtwfgs.cn

const double PI = 3.14159;
来源：http://aw.lnxyls.cn

[S28] C：静态变量
来源：http://gd.chemitech.net.cn

static int counter = 0;
来源：http://oz.muxihuayi.cn

[S29] C：变参函数
来源：http://bn.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sp.hahajie.cn

[S30] C：头文件保护
来源：http://kz.521024.cn

#ifndef X_H
来源：http://od.yuntaijiaju.cn

#define X_H
来源：http://ts.huixinmuqiang.cn

#endif
来源：http://ie.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://vk.yuntaijiaju.cn

#include <iostream>
来源：http://bu.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://fq.521024.cn

[S32] C++：字符串
来源：http://mt.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://nq.szsharing.cn

[S33] C++：vector 增删
来源：http://bb.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kx.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://ek.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://zp.gzmigu.cn

[S35] C++：map
来源：http://he.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rg.asd995.cn

[S36] C++：unordered_map
来源：http://jb.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ta.hnjuh.cn

[S37] C++：set
来源：http://ii.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zn.asd995.cn

[S38] C++：排序
来源：http://rr.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://hd.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://nd.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gz.yuexingan06.cn

[S40] C++：查找元素
来源：http://lq.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ow.newstarts.cn

[S41] C++：类与构造函数
来源：http://kd.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oj.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://rn.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://lr.asd995.cn

[S43] C++：智能指针
来源：http://ld.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://mi.huanxung.cn

[S44] C++：引用传参
来源：http://os.9csxet.cn

void inc(int &x) { ++x; }
来源：http://eg.asd995.cn

[S45] C++：lambda
来源：http://ic.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://as.jctech888.com.cn

[S46] C++：函数模板
来源：http://vw.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sv.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://nl.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://me.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://sg.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hy.haigaiapp.cn


<!-- 参考信息 -->