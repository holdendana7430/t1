代发 wailian999

[Q78] 当前时间
来源：http://fy.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sc.gzmigu.cn

[Q79] 字符串拼接
来源：http://kh.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dg.lnxyls.cn

[Q80] 字符串截取
来源：http://tp.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://am.shxzskj.cn

[Q81] 字符串替换
来源：http://hg.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rd.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://tx.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yk.bjjhwx.cn

[Q83] 大小写转换
来源：http://wq.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ef.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://ar.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://ho.yuntaijiaju.cn

[Q85] 数值取整
来源：http://hg.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xe.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://fy.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jr.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://ty.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bz.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://sb.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wd.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yw.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://kz.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://af.asd995.cn

[Q90] 生成序号列
来源：http://xm.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xb.hnjuh.cn

================================================================================
来源：http://io.haigaiapp.cn

R. Bash 专题
来源：http://ru.bjjhwx.cn

================================================================================
来源：http://os.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://wo.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://on.haigaiapp.cn

set -euo pipefail
来源：http://bl.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://bu.szxytkj.cn

name="Tom"; echo "$name"
来源：http://kd.yuexingan06.cn

[R03] 只读变量
来源：http://jy.muxihuayi.cn

readonly PI=3.14
来源：http://yh.jianghongdianzi.cn

[R04] 位置参数
来源：http://kk.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mo.gzmigu.cn

[R05] 参数默认值
来源：http://yx.muxihuayi.cn

name="${1:-default}"
来源：http://au.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://yh.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oz.jianghongdianzi.cn

[R07] if 判断文件
来源：http://vy.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://py.asd995.cn

[R08] 数值比较
来源：http://zw.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iy.muxihuayi.cn

[R09] 字符串比较
来源：http://vj.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rz.szxytkj.cn

[R10] 正则匹配
来源：http://go.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ge.nszjky.cn

[R11] case 多分支
来源：http://mo.9csxet.cn

case "$1" in
来源：http://uw.haigaiapp.cn

start) echo "启动" ;;
来源：http://ec.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://yb.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://ip.colortex.cn

esac
来源：http://rl.chemitech.net.cn

[R12] for 遍历文件
来源：http://za.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://rp.shxzskj.cn

[R13] for 计数循环
来源：http://zt.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://of.muxihuayi.cn

[R14] C 风格 for
来源：http://bo.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pg.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://eq.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ez.521024.cn

[R16] until 等待条件
来源：http://kl.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cn.9csxet.cn

[R17] 数组定义与取值
来源：http://kk.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wd.shxzskj.cn

[R18] 遍历数组
来源：http://ry.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ee.nszjky.cn

[R19] 数组长度
来源：http://yk.newstarts.cn

echo "${#arr[@]}"
来源：http://rz.hnjuh.cn

[R20] 关联数组（字典）
来源：http://pq.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ip.huixiangedu.cn

[R21] 字符串长度
来源：http://ht.huixiangedu.cn

echo "${#s}"
来源：http://qk.lnxyls.cn

[R22] 截取子串
来源：http://xw.huixiangedu.cn

echo "${s:0:5}"
来源：http://ao.yuntaijiaju.cn

[R23] 字符串替换
来源：http://uk.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zl.huixinmuqiang.cn

[R24] 大小写转换
来源：http://wg.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gy.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://ot.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vy.hahajie.cn

[R26] 命令替换
来源：http://lv.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://ru.nicolike.cn

[R27] 算术展开
来源：http://qx.521024.cn

echo $((1 + 2 * 3))
来源：http://pp.huanxung.cn

[R28] 浮点运算
来源：http://dc.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://gh.nszjky.cn

[R29] 定义函数
来源：http://vq.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jv.9csxet.cn

[R30] 函数返回状态码
来源：http://fr.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://po.huixiangedu.cn

[R31] 局部变量
来源：http://jb.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://im.shtwfgs.cn

[R32] 参数个数校验
来源：http://rp.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xf.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://ja.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ay.panjiajie.cn

[R34] 退出时清理
来源：http://wc.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qw.bjjhwx.cn

[R35] 后台执行并等待
来源：http://fx.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://to.9csxet.cn

[R36] 并发执行多个任务
来源：http://oh.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gj.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://ef.521024.cn

files=$(ls -1)
来源：http://xn.huanxung.cn

[R38] 管道串联
来源：http://si.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://uk.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://uj.panjiajie.cn

cmd > out.log 2>&1
来源：http://kj.asd995.cn

[R40] 追加写日志
来源：http://uf.huixinmuqiang.cn

echo "log" >> out.log
来源：http://fw.huanxung.cn

[R41] 丢弃输出
来源：http://zv.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://me.lnxyls.cn

[R42] 输入重定向
来源：http://bg.nicolike.cn

wc -l < a.txt
来源：http://yy.newstarts.cn

[R43] 按名字查找文件
来源：http://av.newstarts.cn

find . -name "*.log" -type f
来源：http://ow.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://gd.huanxung.cn

find . -mtime -7 -type f
来源：http://ev.newstarts.cn

[R45] 批量删除
来源：http://tn.nszjky.cn

find . -name "*.tmp" -delete
来源：http://kb.gzmigu.cn

[R46] 递归替换文件内容
来源：http://li.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://la.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://fv.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ty.chemitech.net.cn

[R48] awk 取指定列
来源：http://vf.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://ye.shxzukj.cn

[R49] awk 带条件
来源：http://ze.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://me.lnxyls.cn

[R50] awk 求和
来源：http://bs.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qi.jctech888.com.cn

[R51] 排序去重取前几
来源：http://lz.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pi.yuntaijiaju.cn

[R52] 统计行数
来源：http://oh.jianghongdianzi.cn

wc -l a.txt
来源：http://yp.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://go.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ue.gzmigu.cn

[R54] 比较两个文件
来源：http://ep.szxytkj.cn

diff a.txt b.txt
来源：http://uz.colortex.cn

[R55] 压缩与解压
来源：http://aw.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://am.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ad.521024.cn

scp file user@host:/path/
来源：http://vs.asd995.cn

[R57] 远程执行命令
来源：http://af.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://ks.hnjuh.cn

[R58] 下载文件
来源：http://zv.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oj.haigaiapp.cn

[R59] 发 POST JSON
来源：http://tk.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://df.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://ed.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ur.muxihuayi.cn

[R61] 磁盘占用
来源：http://ux.chemitech.net.cn

df -h;  du -sh *
来源：http://yz.nicolike.cn

[R62] 找最占空间的文件
来源：http://ut.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://px.colortex.cn

[R63] 内存与进程
来源：http://su.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://pl.szsharing.cn

[R64] 结束进程
来源：http://xc.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://vc.szsharing.cn

[R65] 查看端口占用
来源：http://vc.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sm.jianghongdianzi.cn

[R66] 定时任务
来源：http://am.muxihuayi.cn

crontab -e;  crontab -l
来源：http://cg.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://ph.bookmarksfly.cn

openssl rand -hex 16
来源：http://dk.wgjwhj.cn

[R68] 计算文件校验值
来源：http://na.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uf.asd995.cn

[R69] 生成随机密码
来源：http://mh.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://lq.gzmigu.cn

[R70] 时间戳与互转
来源：http://yj.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://wb.szxytkj.cn

[R71] 日期格式化
来源：http://zf.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vh.gzmigu.cn

[R72] 等待端口就绪
来源：http://on.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yl.wgjwhj.cn

[R73] 分割大日志
来源：http://kw.colortex.cn

split -l 1000 big.log part_
来源：http://qm.9csxet.cn

[R74] 批量重命名
来源：http://og.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://go.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://tw.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://hj.huanxung.cn

[R76] 使用临时文件
来源：http://gn.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cp.shtwfgs.cn

[R77] 读取用户输入
来源：http://ro.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://xq.shxzukj.cn

[R78] 交互式菜单
来源：http://at.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qr.huixiangedu.cn

[R79] 解析命令行选项
来源：http://pq.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dy.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://gs.bookmarksfly.cn

time ./run.sh
来源：http://ax.muxihuayi.cn

================================================================================
来源：http://ik.huixinmuqiang.cn

S. C / C++ 专题
来源：http://um.521024.cn

================================================================================
来源：http://bd.9csxet.cn

[S01] C：Hello World
来源：http://gt.muxihuayi.cn

#include <stdio.h>
来源：http://ph.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gg.huanxung.cn

[S02] C：变量与格式化输出
来源：http://hw.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://te.9csxet.cn

[S03] C：读入整数
来源：http://pc.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://py.huanxung.cn

[S04] C：字符串复制
来源：http://au.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ax.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://lh.nicolike.cn

strlen(s)
来源：http://ay.muxihuayi.cn

[S06] C：字符串比较
来源：http://pg.521024.cn

strcmp(a, b) == 0
来源：http://ql.hahajie.cn

[S07] C：数组遍历求和
来源：http://lz.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vk.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://oz.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mi.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://us.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xh.hahajie.cn

[S10] C：指针与解引用
来源：http://yp.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://mq.szxytkj.cn

[S11] C：逐行读文件
来源：http://qg.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://aa.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dg.colortex.cn

fclose(f);
来源：http://lq.lnxyls.cn

[S12] C：写文件
来源：http://bs.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pv.hnjuh.cn

[S13] C：宏定义
来源：http://ce.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ng.521024.cn

[S14] C：枚举
来源：http://eu.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://rg.asd995.cn

[S15] C：类型转换
来源：http://sg.hnjuh.cn

(double) a / b
来源：http://mf.shxzukj.cn

[S16] C：位操作置位
来源：http://oz.haigaiapp.cn

x |= (1 << 3);
来源：http://nn.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://xp.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rr.colortex.cn

[S18] C：命令行参数
来源：http://dw.wgjwhj.cn

int main(int argc, char **argv)
来源：http://rw.yuntaijiaju.cn

[S19] C：快速排序
来源：http://ii.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rf.bjjhwx.cn

[S20] C：二分查找
来源：http://ko.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zh.yuexingan06.cn

[S21] C：字符类别判断
来源：http://pv.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hs.nicolike.cn

[S22] C：字符串转数字
来源：http://as.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bk.wgjwhj.cn

[S23] C：随机数
来源：http://cs.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tr.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://gu.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ww.panjiajie.cn

[S25] C：内存拷贝
来源：http://mb.shxzskj.cn

memcpy(dst, src, n);
来源：http://bo.nszjky.cn

[S26] C：内存清零
来源：http://no.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://cf.shxzskj.cn

[S27] C：定义常量
来源：http://kq.hahajie.cn

const double PI = 3.14159;
来源：http://xm.szxytkj.cn

[S28] C：静态变量
来源：http://pc.haigaiapp.cn

static int counter = 0;
来源：http://st.nszjky.cn

[S29] C：变参函数
来源：http://mo.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kl.newstarts.cn

[S30] C：头文件保护
来源：http://ol.szxytkj.cn

#ifndef X_H
来源：http://cc.gzmigu.cn

#define X_H
来源：http://pg.wgjwhj.cn

#endif
来源：http://mv.newstarts.cn

[S31] C++：Hello World
来源：http://mo.asd995.cn

#include <iostream>
来源：http://cf.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://qr.huixinmuqiang.cn

[S32] C++：字符串
来源：http://tx.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://sb.nszjky.cn

[S33] C++：vector 增删
来源：http://hn.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mb.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://fq.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://bs.yuntaijiaju.cn

[S35] C++：map
来源：http://ls.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://su.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://zj.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ui.muxihuayi.cn

[S37] C++：set
来源：http://aw.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://es.hnjuh.cn

[S38] C++：排序
来源：http://yt.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://iu.asd995.cn

[S39] C++：自定义比较器排序
来源：http://oy.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iv.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://ii.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zf.nszjky.cn

[S41] C++：类与构造函数
来源：http://hc.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xx.hahajie.cn

[S42] C++：继承与虚函数
来源：http://ji.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://zx.panjiajie.cn

[S43] C++：智能指针
来源：http://ry.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://bv.wgjwhj.cn

[S44] C++：引用传参
来源：http://mr.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://jb.jctech888.com.cn

[S45] C++：lambda
来源：http://ib.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wv.shtwfgs.cn

[S46] C++：函数模板
来源：http://bw.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yw.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://nc.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fk.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://fe.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gi.hahajie.cn


<!-- 参考信息 -->