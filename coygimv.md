代发 wailian999

[Q78] 当前时间
来源：http://ea.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tw.muxihuayi.cn

[Q79] 字符串拼接
来源：http://xb.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gs.szxytkj.cn

[Q80] 字符串截取
来源：http://or.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bh.szsharing.cn

[Q81] 字符串替换
来源：http://qk.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ry.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://fa.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zl.haigaiapp.cn

[Q83] 大小写转换
来源：http://jb.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wd.shxzukj.cn

[Q84] 去除首尾空格
来源：http://hn.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://fm.huanxung.cn

[Q85] 数值取整
来源：http://mp.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vz.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://qo.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lz.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://rn.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://io.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://tu.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vr.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dr.hnjuh.cn

[Q89] 判断表是否存在
来源：http://et.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bb.shxzukj.cn

[Q90] 生成序号列
来源：http://ys.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wq.shxzukj.cn

================================================================================
来源：http://ei.chemitech.net.cn

R. Bash 专题
来源：http://ed.jianghongdianzi.cn

================================================================================
来源：http://pn.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://iv.jctech888.com.cn

#!/usr/bin/env bash
来源：http://dg.wgjwhj.cn

set -euo pipefail
来源：http://nu.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://ro.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://ad.yuexingan06.cn

[R03] 只读变量
来源：http://fo.lnxyls.cn

readonly PI=3.14
来源：http://yn.yuexingan06.cn

[R04] 位置参数
来源：http://en.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ed.newstarts.cn

[R05] 参数默认值
来源：http://gg.jctech888.com.cn

name="${1:-default}"
来源：http://tt.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://yq.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rn.shxzskj.cn

[R07] if 判断文件
来源：http://qj.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sm.chemitech.net.cn

[R08] 数值比较
来源：http://iw.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ec.yuntaijiaju.cn

[R09] 字符串比较
来源：http://fe.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jt.yuntaijiaju.cn

[R10] 正则匹配
来源：http://mr.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ri.chemitech.net.cn

[R11] case 多分支
来源：http://fj.gzmigu.cn

case "$1" in
来源：http://fj.hahajie.cn

start) echo "启动" ;;
来源：http://hv.newstarts.cn

stop)  echo "停止" ;;
来源：http://cj.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://km.huixiangedu.cn

esac
来源：http://rx.bookmarksfly.cn

[R12] for 遍历文件
来源：http://ad.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://vo.jctech888.com.cn

[R13] for 计数循环
来源：http://co.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://oc.bookmarksfly.cn

[R14] C 风格 for
来源：http://ky.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aw.nszjky.cn

[R15] while 逐行读文件
来源：http://va.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tg.nszjky.cn

[R16] until 等待条件
来源：http://rr.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ek.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://qy.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ud.haigaiapp.cn

[R18] 遍历数组
来源：http://yh.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zh.bookmarksfly.cn

[R19] 数组长度
来源：http://si.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://ln.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://pg.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qg.shxzukj.cn

[R21] 字符串长度
来源：http://fx.asd995.cn

echo "${#s}"
来源：http://av.jianghongdianzi.cn

[R22] 截取子串
来源：http://ro.huanxung.cn

echo "${s:0:5}"
来源：http://ud.jianghongdianzi.cn

[R23] 字符串替换
来源：http://ea.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xn.bookmarksfly.cn

[R24] 大小写转换
来源：http://zq.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://on.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://cv.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hc.haigaiapp.cn

[R26] 命令替换
来源：http://hb.asd995.cn

now=$(date +%F); echo "$now"
来源：http://pl.panjiajie.cn

[R27] 算术展开
来源：http://gl.nicolike.cn

echo $((1 + 2 * 3))
来源：http://hl.521024.cn

[R28] 浮点运算
来源：http://ry.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://wt.yuexingan06.cn

[R29] 定义函数
来源：http://gu.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pd.9csxet.cn

[R30] 函数返回状态码
来源：http://mu.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://kv.newstarts.cn

[R31] 局部变量
来源：http://mi.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://lq.gzmigu.cn

[R32] 参数个数校验
来源：http://ud.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rk.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://rp.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ff.lnxyls.cn

[R34] 退出时清理
来源：http://lf.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gh.szxytkj.cn

[R35] 后台执行并等待
来源：http://ye.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wa.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://cl.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wf.521024.cn

[R37] 把输出赋给变量
来源：http://bb.szxytkj.cn

files=$(ls -1)
来源：http://tf.haigaiapp.cn

[R38] 管道串联
来源：http://vf.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://be.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://mh.shxzukj.cn

cmd > out.log 2>&1
来源：http://rk.jianghongdianzi.cn

[R40] 追加写日志
来源：http://au.szsharing.cn

echo "log" >> out.log
来源：http://ox.lnxyls.cn

[R41] 丢弃输出
来源：http://hy.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://lu.colortex.cn

[R42] 输入重定向
来源：http://dn.shxzukj.cn

wc -l < a.txt
来源：http://fb.wgjwhj.cn

[R43] 按名字查找文件
来源：http://vv.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ao.9csxet.cn

[R44] 按修改时间查找
来源：http://wo.hnjuh.cn

find . -mtime -7 -type f
来源：http://rh.huanxung.cn

[R45] 批量删除
来源：http://aa.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://gp.newstarts.cn

[R46] 递归替换文件内容
来源：http://ir.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ae.bjjhwx.cn

[R47] sed 单行替换
来源：http://ga.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://la.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://nh.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://cb.huixinmuqiang.cn

[R49] awk 带条件
来源：http://vl.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yq.shxzukj.cn

[R50] awk 求和
来源：http://kg.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://su.colortex.cn

[R51] 排序去重取前几
来源：http://fd.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jp.szxytkj.cn

[R52] 统计行数
来源：http://an.panjiajie.cn

wc -l a.txt
来源：http://pp.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://xd.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wc.hnjuh.cn

[R54] 比较两个文件
来源：http://tf.jctech888.com.cn

diff a.txt b.txt
来源：http://hc.asd995.cn

[R55] 压缩与解压
来源：http://wf.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mp.521024.cn

[R56] 远程拷贝
来源：http://ux.huanxung.cn

scp file user@host:/path/
来源：http://vd.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://yy.shtwfgs.cn

ssh user@host 'uptime'
来源：http://zv.szsharing.cn

[R58] 下载文件
来源：http://vh.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zv.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://gi.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wd.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://vp.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ja.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://tl.colortex.cn

df -h;  du -sh *
来源：http://gu.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://mt.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://ny.huixinmuqiang.cn

[R63] 内存与进程
来源：http://vt.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://sg.shxzskj.cn

[R64] 结束进程
来源：http://ah.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://th.asd995.cn

[R65] 查看端口占用
来源：http://cc.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sj.yuntaijiaju.cn

[R66] 定时任务
来源：http://sx.shtwfgs.cn

crontab -e;  crontab -l
来源：http://yh.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://wc.shxzukj.cn

openssl rand -hex 16
来源：http://yt.nszjky.cn

[R68] 计算文件校验值
来源：http://ct.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bx.9csxet.cn

[R69] 生成随机密码
来源：http://lk.521024.cn

head -c 16 /dev/urandom | base64
来源：http://tx.hahajie.cn

[R70] 时间戳与互转
来源：http://az.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://vb.muxihuayi.cn

[R71] 日期格式化
来源：http://er.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jy.muxihuayi.cn

[R72] 等待端口就绪
来源：http://md.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://de.haigaiapp.cn

[R73] 分割大日志
来源：http://df.chemitech.net.cn

split -l 1000 big.log part_
来源：http://uu.jctech888.com.cn

[R74] 批量重命名
来源：http://np.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pv.lnxyls.cn

[R75] 导出环境变量
来源：http://fw.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://zg.bjjhwx.cn

[R76] 使用临时文件
来源：http://lg.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ra.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://np.szsharing.cn

read -rp "请输入: " ans
来源：http://do.colortex.cn

[R78] 交互式菜单
来源：http://xz.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tf.hnjuh.cn

[R79] 解析命令行选项
来源：http://np.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cu.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://uv.haigaiapp.cn

time ./run.sh
来源：http://eu.nszjky.cn

================================================================================
来源：http://ds.yuexingan06.cn

S. C / C++ 专题
来源：http://fv.szxytkj.cn

================================================================================
来源：http://rn.jctech888.com.cn

[S01] C：Hello World
来源：http://mn.bookmarksfly.cn

#include <stdio.h>
来源：http://lu.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hv.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://se.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://ui.szxytkj.cn

[S03] C：读入整数
来源：http://aa.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://lk.yuexingan06.cn

[S04] C：字符串复制
来源：http://jl.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pj.shxzukj.cn

[S05] C：字符串长度
来源：http://ib.newstarts.cn

strlen(s)
来源：http://of.colortex.cn

[S06] C：字符串比较
来源：http://qj.hahajie.cn

strcmp(a, b) == 0
来源：http://xq.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://pa.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ur.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://de.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ob.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://lk.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oi.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://qw.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://cs.huixiangedu.cn

[S11] C：逐行读文件
来源：http://st.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://sw.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yp.panjiajie.cn

fclose(f);
来源：http://ah.jctech888.com.cn

[S12] C：写文件
来源：http://ch.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eo.huixiangedu.cn

[S13] C：宏定义
来源：http://ed.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qv.panjiajie.cn

[S14] C：枚举
来源：http://nx.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://rh.huixiangedu.cn

[S15] C：类型转换
来源：http://hp.szxytkj.cn

(double) a / b
来源：http://im.huanxung.cn

[S16] C：位操作置位
来源：http://dy.nszjky.cn

x |= (1 << 3);
来源：http://jr.9csxet.cn

[S17] C：安全拼接字符串
来源：http://qn.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://me.nicolike.cn

[S18] C：命令行参数
来源：http://qs.szxytkj.cn

int main(int argc, char **argv)
来源：http://hq.nicolike.cn

[S19] C：快速排序
来源：http://ch.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ur.asd995.cn

[S20] C：二分查找
来源：http://jj.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://js.nicolike.cn

[S21] C：字符类别判断
来源：http://nm.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cv.huanxung.cn

[S22] C：字符串转数字
来源：http://tt.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://el.huixiangedu.cn

[S23] C：随机数
来源：http://je.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sc.asd995.cn

[S24] C：获取本地时间
来源：http://ds.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mx.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://yg.muxihuayi.cn

memcpy(dst, src, n);
来源：http://mm.shtwfgs.cn

[S26] C：内存清零
来源：http://fw.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://oc.huixinmuqiang.cn

[S27] C：定义常量
来源：http://wr.gzmigu.cn

const double PI = 3.14159;
来源：http://tl.bookmarksfly.cn

[S28] C：静态变量
来源：http://eb.yuexingan06.cn

static int counter = 0;
来源：http://bs.panjiajie.cn

[S29] C：变参函数
来源：http://ln.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fi.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://jc.hahajie.cn

#ifndef X_H
来源：http://fi.haigaiapp.cn

#define X_H
来源：http://ig.521024.cn

#endif
来源：http://kp.9csxet.cn

[S31] C++：Hello World
来源：http://mh.huixiangedu.cn

#include <iostream>
来源：http://el.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://qg.521024.cn

[S32] C++：字符串
来源：http://jz.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://cf.nszjky.cn

[S33] C++：vector 增删
来源：http://yo.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jb.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://nk.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://wr.haigaiapp.cn

[S35] C++：map
来源：http://we.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gi.gzmigu.cn

[S36] C++：unordered_map
来源：http://xf.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ua.yuntaijiaju.cn

[S37] C++：set
来源：http://fi.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sv.jctech888.com.cn

[S38] C++：排序
来源：http://xm.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://gr.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://wn.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xw.wgjwhj.cn

[S40] C++：查找元素
来源：http://sf.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fi.nicolike.cn

[S41] C++：类与构造函数
来源：http://cs.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qj.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://np.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://ff.huanxung.cn

[S43] C++：智能指针
来源：http://vb.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://pk.shxzukj.cn

[S44] C++：引用传参
来源：http://iz.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://nw.9csxet.cn

[S45] C++：lambda
来源：http://hr.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ww.shxzukj.cn

[S46] C++：函数模板
来源：http://jl.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fb.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://lw.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uw.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://uj.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zd.newstarts.cn


<!-- 参考信息 -->