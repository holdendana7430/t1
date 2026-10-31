代发 wailian999

[Q76] 按天统计
来源：http://vu.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nszjky.cn

[Q77] 时间加减
来源：http://kn.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ob.9csxet.cn

[Q78] 当前时间
来源：http://bw.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://un.yuexingan06.cn

[Q79] 字符串拼接
来源：http://sh.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wa.gzmigu.cn

[Q80] 字符串截取
来源：http://jg.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qu.nicolike.cn

[Q81] 字符串替换
来源：http://gu.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xd.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://fm.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ww.nicolike.cn

[Q83] 大小写转换
来源：http://zt.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uu.hahajie.cn

[Q84] 去除首尾空格
来源：http://yn.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://mh.shtwfgs.cn

[Q85] 数值取整
来源：http://ni.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iy.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://ud.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tt.colortex.cn

[Q87] JSON 字段做条件
来源：http://jx.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mj.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://jm.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yi.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oc.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://ky.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ij.yuexingan06.cn

[Q90] 生成序号列
来源：http://ua.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hi.chemitech.net.cn

================================================================================
来源：http://sf.521024.cn

R. Bash 专题
来源：http://dg.chemitech.net.cn

================================================================================
来源：http://vp.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://xd.9csxet.cn

#!/usr/bin/env bash
来源：http://qy.huanxung.cn

set -euo pipefail
来源：http://lu.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://mi.lnxyls.cn

name="Tom"; echo "$name"
来源：http://zz.muxihuayi.cn

[R03] 只读变量
来源：http://ep.jctech888.com.cn

readonly PI=3.14
来源：http://nn.colortex.cn

[R04] 位置参数
来源：http://wc.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sh.haigaiapp.cn

[R05] 参数默认值
来源：http://sa.lnxyls.cn

name="${1:-default}"
来源：http://xk.lnxyls.cn

[R06] 判断命令是否存在
来源：http://zc.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kx.newstarts.cn

[R07] if 判断文件
来源：http://qa.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ji.yuexingan06.cn

[R08] 数值比较
来源：http://pn.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fj.shtwfgs.cn

[R09] 字符串比较
来源：http://pp.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rr.jctech888.com.cn

[R10] 正则匹配
来源：http://nm.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ny.muxihuayi.cn

[R11] case 多分支
来源：http://ox.panjiajie.cn

case "$1" in
来源：http://pb.haigaiapp.cn

start) echo "启动" ;;
来源：http://fu.szxytkj.cn

stop)  echo "停止" ;;
来源：http://jh.asd995.cn

*)     echo "未知命令" ;;
来源：http://qe.nicolike.cn

esac
来源：http://wd.lnxyls.cn

[R12] for 遍历文件
来源：http://xp.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://ai.9csxet.cn

[R13] for 计数循环
来源：http://oi.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://le.huixinmuqiang.cn

[R14] C 风格 for
来源：http://dl.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ou.nicolike.cn

[R15] while 逐行读文件
来源：http://qu.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qr.huanxung.cn

[R16] until 等待条件
来源：http://ex.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gk.colortex.cn

[R17] 数组定义与取值
来源：http://fx.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ek.haigaiapp.cn

[R18] 遍历数组
来源：http://nw.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tk.bjjhwx.cn

[R19] 数组长度
来源：http://kx.lnxyls.cn

echo "${#arr[@]}"
来源：http://ec.9csxet.cn

[R20] 关联数组（字典）
来源：http://es.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://id.muxihuayi.cn

[R21] 字符串长度
来源：http://ty.asd995.cn

echo "${#s}"
来源：http://th.9csxet.cn

[R22] 截取子串
来源：http://my.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://fx.szxytkj.cn

[R23] 字符串替换
来源：http://ga.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ga.shxzukj.cn

[R24] 大小写转换
来源：http://en.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uy.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://gy.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ea.hahajie.cn

[R26] 命令替换
来源：http://lp.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://fq.muxihuayi.cn

[R27] 算术展开
来源：http://xy.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://ur.shtwfgs.cn

[R28] 浮点运算
来源：http://jx.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://cu.huanxung.cn

[R29] 定义函数
来源：http://xg.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fi.bjjhwx.cn

[R30] 函数返回状态码
来源：http://pv.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://oa.colortex.cn

[R31] 局部变量
来源：http://xw.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://sw.shxzukj.cn

[R32] 参数个数校验
来源：http://gq.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bq.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://ji.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wx.521024.cn

[R34] 退出时清理
来源：http://wx.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dj.haigaiapp.cn

[R35] 后台执行并等待
来源：http://aq.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ir.szxytkj.cn

[R36] 并发执行多个任务
来源：http://sq.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hd.521024.cn

[R37] 把输出赋给变量
来源：http://wo.bookmarksfly.cn

files=$(ls -1)
来源：http://tm.shxzukj.cn

[R38] 管道串联
来源：http://qi.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://vq.asd995.cn

[R39] 重定向标准输出与错误
来源：http://lh.shtwfgs.cn

cmd > out.log 2>&1
来源：http://wi.szxytkj.cn

[R40] 追加写日志
来源：http://yd.bjjhwx.cn

echo "log" >> out.log
来源：http://wy.nicolike.cn

[R41] 丢弃输出
来源：http://tc.9csxet.cn

cmd >/dev/null 2>&1
来源：http://hy.lnxyls.cn

[R42] 输入重定向
来源：http://nu.nszjky.cn

wc -l < a.txt
来源：http://yj.jctech888.com.cn

[R43] 按名字查找文件
来源：http://yp.colortex.cn

find . -name "*.log" -type f
来源：http://wk.panjiajie.cn

[R44] 按修改时间查找
来源：http://bg.huanxung.cn

find . -mtime -7 -type f
来源：http://gq.hnjuh.cn

[R45] 批量删除
来源：http://st.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://rz.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://dg.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zh.huixiangedu.cn

[R47] sed 单行替换
来源：http://is.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jh.haigaiapp.cn

[R48] awk 取指定列
来源：http://up.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://qc.shtwfgs.cn

[R49] awk 带条件
来源：http://ja.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://in.hahajie.cn

[R50] awk 求和
来源：http://nq.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ee.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://bk.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://io.chemitech.net.cn

[R52] 统计行数
来源：http://ke.521024.cn

wc -l a.txt
来源：http://oo.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://rn.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nr.shxzskj.cn

[R54] 比较两个文件
来源：http://we.szxytkj.cn

diff a.txt b.txt
来源：http://dp.huanxung.cn

[R55] 压缩与解压
来源：http://lh.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xe.nszjky.cn

[R56] 远程拷贝
来源：http://zu.huixinmuqiang.cn

scp file user@host:/path/
来源：http://ul.chemitech.net.cn

[R57] 远程执行命令
来源：http://cr.yuexingan06.cn

ssh user@host 'uptime'
来源：http://mv.nszjky.cn

[R58] 下载文件
来源：http://qo.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vw.huixiangedu.cn

[R59] 发 POST JSON
来源：http://ro.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ae.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://ui.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mp.shxzukj.cn

[R61] 磁盘占用
来源：http://nt.jianghongdianzi.cn

df -h;  du -sh *
来源：http://mg.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://ly.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://ql.nszjky.cn

[R63] 内存与进程
来源：http://fz.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://hx.hahajie.cn

[R64] 结束进程
来源：http://lo.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://cw.colortex.cn

[R65] 查看端口占用
来源：http://rq.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tb.panjiajie.cn

[R66] 定时任务
来源：http://nn.nicolike.cn

crontab -e;  crontab -l
来源：http://ak.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://ko.asd995.cn

openssl rand -hex 16
来源：http://mn.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://tv.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ye.lnxyls.cn

[R69] 生成随机密码
来源：http://sj.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://oj.szsharing.cn

[R70] 时间戳与互转
来源：http://ex.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://gx.wgjwhj.cn

[R71] 日期格式化
来源：http://kl.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lc.hnjuh.cn

[R72] 等待端口就绪
来源：http://px.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://og.nicolike.cn

[R73] 分割大日志
来源：http://cl.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://es.jianghongdianzi.cn

[R74] 批量重命名
来源：http://bl.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gz.muxihuayi.cn

[R75] 导出环境变量
来源：http://pu.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://ev.wgjwhj.cn

[R76] 使用临时文件
来源：http://zd.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hs.panjiajie.cn

[R77] 读取用户输入
来源：http://bp.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://pp.nszjky.cn

[R78] 交互式菜单
来源：http://mf.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uk.gzmigu.cn

[R79] 解析命令行选项
来源：http://pm.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vh.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://ed.521024.cn

time ./run.sh
来源：http://ht.szxytkj.cn

================================================================================
来源：http://up.huixiangedu.cn

S. C / C++ 专题
来源：http://ql.bookmarksfly.cn

================================================================================
来源：http://zq.521024.cn

[S01] C：Hello World
来源：http://ah.panjiajie.cn

#include <stdio.h>
来源：http://wr.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zf.colortex.cn

[S02] C：变量与格式化输出
来源：http://px.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://vc.szsharing.cn

[S03] C：读入整数
来源：http://xx.newstarts.cn

int x; scanf("%d", &x);
来源：http://fj.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://jj.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ln.bjjhwx.cn

[S05] C：字符串长度
来源：http://fl.shtwfgs.cn

strlen(s)
来源：http://dy.bjjhwx.cn

[S06] C：字符串比较
来源：http://ii.chemitech.net.cn

strcmp(a, b) == 0
来源：http://wl.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://nn.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://no.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://xh.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sq.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://ix.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ql.szsharing.cn

[S10] C：指针与解引用
来源：http://me.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://ts.haigaiapp.cn

[S11] C：逐行读文件
来源：http://gw.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://gz.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ix.colortex.cn

fclose(f);
来源：http://pp.jianghongdianzi.cn

[S12] C：写文件
来源：http://xu.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zt.newstarts.cn

[S13] C：宏定义
来源：http://ur.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sg.gzmigu.cn

[S14] C：枚举
来源：http://bi.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://lr.huixiangedu.cn

[S15] C：类型转换
来源：http://cc.asd995.cn

(double) a / b
来源：http://bn.panjiajie.cn

[S16] C：位操作置位
来源：http://dx.hahajie.cn

x |= (1 << 3);
来源：http://un.521024.cn

[S17] C：安全拼接字符串
来源：http://fx.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xd.shtwfgs.cn

[S18] C：命令行参数
来源：http://sj.chemitech.net.cn

int main(int argc, char **argv)
来源：http://jb.huixiangedu.cn

[S19] C：快速排序
来源：http://az.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aj.hahajie.cn

[S20] C：二分查找
来源：http://mc.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mr.hnjuh.cn

[S21] C：字符类别判断
来源：http://cu.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sx.chemitech.net.cn

[S22] C：字符串转数字
来源：http://gl.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ng.szsharing.cn

[S23] C：随机数
来源：http://ev.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oz.muxihuayi.cn

[S24] C：获取本地时间
来源：http://hw.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fp.hahajie.cn

[S25] C：内存拷贝
来源：http://jt.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://ur.jianghongdianzi.cn

[S26] C：内存清零
来源：http://fc.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://ei.wgjwhj.cn

[S27] C：定义常量
来源：http://ud.muxihuayi.cn

const double PI = 3.14159;
来源：http://zn.hnjuh.cn

[S28] C：静态变量
来源：http://ec.huixinmuqiang.cn

static int counter = 0;
来源：http://kb.lnxyls.cn

[S29] C：变参函数
来源：http://ec.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hm.bjjhwx.cn

[S30] C：头文件保护
来源：http://yn.yuntaijiaju.cn

#ifndef X_H
来源：http://og.lnxyls.cn

#define X_H
来源：http://ok.huanxung.cn

#endif
来源：http://xu.yuexingan06.cn

[S31] C++：Hello World
来源：http://fp.huanxung.cn

#include <iostream>
来源：http://cl.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://jk.szsharing.cn

[S32] C++：字符串
来源：http://mt.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://bz.jctech888.com.cn

[S33] C++：vector 增删
来源：http://mb.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dm.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://ie.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://ag.jctech888.com.cn

[S35] C++：map
来源：http://hm.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rc.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://du.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vm.chemitech.net.cn

[S37] C++：set
来源：http://bn.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wv.asd995.cn

[S38] C++：排序
来源：http://ot.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://bp.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://fm.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fu.asd995.cn

[S40] C++：查找元素
来源：http://pe.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vh.hnjuh.cn

[S41] C++：类与构造函数
来源：http://gp.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pn.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://gc.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ap.huanxung.cn

[S43] C++：智能指针
来源：http://ac.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://sd.panjiajie.cn

[S44] C++：引用传参
来源：http://uv.521024.cn

void inc(int &x) { ++x; }
来源：http://hg.521024.cn

[S45] C++：lambda
来源：http://ln.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vh.huixiangedu.cn

[S46] C++：函数模板
来源：http://pr.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oq.szxytkj.cn


<!-- 参考信息 -->