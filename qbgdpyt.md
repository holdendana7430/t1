代发 wailian999

[Q76] 按天统计
来源：http://qq.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pl.wgjwhj.cn

[Q77] 时间加减
来源：http://ra.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://at.colortex.cn

[Q78] 当前时间
来源：http://la.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xg.bjjhwx.cn

[Q79] 字符串拼接
来源：http://nd.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ax.jctech888.com.cn

[Q80] 字符串截取
来源：http://rj.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xz.shtwfgs.cn

[Q81] 字符串替换
来源：http://au.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qu.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://nc.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nc.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://zh.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://av.9csxet.cn

[Q84] 去除首尾空格
来源：http://vx.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://ey.gzmigu.cn

[Q85] 数值取整
来源：http://lq.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qu.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://ex.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://si.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://ef.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jm.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://bq.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ke.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hm.asd995.cn

[Q89] 判断表是否存在
来源：http://ae.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pi.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://wk.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ya.shxzukj.cn

================================================================================
来源：http://vr.chemitech.net.cn

R. Bash 专题
来源：http://vw.shxzukj.cn

================================================================================
来源：http://kf.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://nm.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://hr.yuntaijiaju.cn

set -euo pipefail
来源：http://tn.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://dx.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://dg.yuexingan06.cn

[R03] 只读变量
来源：http://hw.huanxung.cn

readonly PI=3.14
来源：http://vt.wgjwhj.cn

[R04] 位置参数
来源：http://mk.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kg.szxytkj.cn

[R05] 参数默认值
来源：http://wq.lnxyls.cn

name="${1:-default}"
来源：http://cl.gzmigu.cn

[R06] 判断命令是否存在
来源：http://rh.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kb.nicolike.cn

[R07] if 判断文件
来源：http://hi.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xs.bjjhwx.cn

[R08] 数值比较
来源：http://nz.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ho.gzmigu.cn

[R09] 字符串比较
来源：http://zk.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gk.hahajie.cn

[R10] 正则匹配
来源：http://uq.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wn.chemitech.net.cn

[R11] case 多分支
来源：http://ka.panjiajie.cn

case "$1" in
来源：http://gw.gzmigu.cn

start) echo "启动" ;;
来源：http://rv.huanxung.cn

stop)  echo "停止" ;;
来源：http://sm.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://oq.yuexingan06.cn

esac
来源：http://is.lnxyls.cn

[R12] for 遍历文件
来源：http://ba.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://fn.szxytkj.cn

[R13] for 计数循环
来源：http://yh.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://vh.huixiangedu.cn

[R14] C 风格 for
来源：http://wz.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ut.colortex.cn

[R15] while 逐行读文件
来源：http://ac.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nl.huanxung.cn

[R16] until 等待条件
来源：http://um.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yl.shxzskj.cn

[R17] 数组定义与取值
来源：http://pj.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jb.jctech888.com.cn

[R18] 遍历数组
来源：http://ny.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qs.szxytkj.cn

[R19] 数组长度
来源：http://zz.haigaiapp.cn

echo "${#arr[@]}"
来源：http://ll.newstarts.cn

[R20] 关联数组（字典）
来源：http://kx.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rn.haigaiapp.cn

[R21] 字符串长度
来源：http://im.nszjky.cn

echo "${#s}"
来源：http://jv.hnjuh.cn

[R22] 截取子串
来源：http://bv.nszjky.cn

echo "${s:0:5}"
来源：http://xo.jianghongdianzi.cn

[R23] 字符串替换
来源：http://tb.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ew.newstarts.cn

[R24] 大小写转换
来源：http://fh.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zj.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://yi.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dc.jianghongdianzi.cn

[R26] 命令替换
来源：http://lq.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://dy.gzmigu.cn

[R27] 算术展开
来源：http://hb.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://pw.chemitech.net.cn

[R28] 浮点运算
来源：http://rd.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://zc.hnjuh.cn

[R29] 定义函数
来源：http://em.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ld.asd995.cn

[R30] 函数返回状态码
来源：http://cb.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://lk.hahajie.cn

[R31] 局部变量
来源：http://sx.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://ic.asd995.cn

[R32] 参数个数校验
来源：http://up.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ql.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://nc.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ar.muxihuayi.cn

[R34] 退出时清理
来源：http://oi.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://er.asd995.cn

[R35] 后台执行并等待
来源：http://ne.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vf.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://qb.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xi.nicolike.cn

[R37] 把输出赋给变量
来源：http://km.yuexingan06.cn

files=$(ls -1)
来源：http://gd.wgjwhj.cn

[R38] 管道串联
来源：http://wg.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://ug.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://cx.wgjwhj.cn

cmd > out.log 2>&1
来源：http://hp.jctech888.com.cn

[R40] 追加写日志
来源：http://vz.shtwfgs.cn

echo "log" >> out.log
来源：http://zx.lnxyls.cn

[R41] 丢弃输出
来源：http://yp.nszjky.cn

cmd >/dev/null 2>&1
来源：http://wy.haigaiapp.cn

[R42] 输入重定向
来源：http://kh.bookmarksfly.cn

wc -l < a.txt
来源：http://it.jctech888.com.cn

[R43] 按名字查找文件
来源：http://gn.wgjwhj.cn

find . -name "*.log" -type f
来源：http://vx.jctech888.com.cn

[R44] 按修改时间查找
来源：http://gn.bjjhwx.cn

find . -mtime -7 -type f
来源：http://es.panjiajie.cn

[R45] 批量删除
来源：http://vf.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://xh.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://yy.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vj.haigaiapp.cn

[R47] sed 单行替换
来源：http://an.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vy.hahajie.cn

[R48] awk 取指定列
来源：http://hh.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://cm.colortex.cn

[R49] awk 带条件
来源：http://qb.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uh.nszjky.cn

[R50] awk 求和
来源：http://wn.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ii.yuexingan06.cn

[R51] 排序去重取前几
来源：http://ml.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://er.shtwfgs.cn

[R52] 统计行数
来源：http://zh.gzmigu.cn

wc -l a.txt
来源：http://xp.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://zq.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ex.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://bw.shtwfgs.cn

diff a.txt b.txt
来源：http://na.newstarts.cn

[R55] 压缩与解压
来源：http://ul.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zx.yuexingan06.cn

[R56] 远程拷贝
来源：http://gc.asd995.cn

scp file user@host:/path/
来源：http://ye.shxzukj.cn

[R57] 远程执行命令
来源：http://dc.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://dr.nicolike.cn

[R58] 下载文件
来源：http://sr.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://to.hahajie.cn

[R59] 发 POST JSON
来源：http://ri.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bl.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://ar.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tr.huixiangedu.cn

[R61] 磁盘占用
来源：http://nl.szsharing.cn

df -h;  du -sh *
来源：http://rx.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://mu.asd995.cn

du -ah . | sort -rh | head -10
来源：http://mx.huanxung.cn

[R63] 内存与进程
来源：http://wk.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://du.jianghongdianzi.cn

[R64] 结束进程
来源：http://oh.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://gs.9csxet.cn

[R65] 查看端口占用
来源：http://xj.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ft.shtwfgs.cn

[R66] 定时任务
来源：http://ke.huanxung.cn

crontab -e;  crontab -l
来源：http://jo.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://ff.bjjhwx.cn

openssl rand -hex 16
来源：http://ne.panjiajie.cn

[R68] 计算文件校验值
来源：http://xh.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ws.huixiangedu.cn

[R69] 生成随机密码
来源：http://jc.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://sh.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://st.nicolike.cn

date +%s;  date -d @1700000000
来源：http://tb.9csxet.cn

[R71] 日期格式化
来源：http://oq.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fg.9csxet.cn

[R72] 等待端口就绪
来源：http://ez.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xn.bookmarksfly.cn

[R73] 分割大日志
来源：http://zt.huixiangedu.cn

split -l 1000 big.log part_
来源：http://jh.shxzukj.cn

[R74] 批量重命名
来源：http://bt.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iu.yuexingan06.cn

[R75] 导出环境变量
来源：http://bd.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://rp.bjjhwx.cn

[R76] 使用临时文件
来源：http://ko.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tg.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://nq.panjiajie.cn

read -rp "请输入: " ans
来源：http://kh.newstarts.cn

[R78] 交互式菜单
来源：http://ps.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ot.nicolike.cn

[R79] 解析命令行选项
来源：http://gg.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dz.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://rw.bookmarksfly.cn

time ./run.sh
来源：http://wk.521024.cn

================================================================================
来源：http://cy.huixiangedu.cn

S. C / C++ 专题
来源：http://py.newstarts.cn

================================================================================
来源：http://ys.shtwfgs.cn

[S01] C：Hello World
来源：http://mw.muxihuayi.cn

#include <stdio.h>
来源：http://qr.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mo.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://gj.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://ds.muxihuayi.cn

[S03] C：读入整数
来源：http://tf.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://ys.lnxyls.cn

[S04] C：字符串复制
来源：http://lo.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://at.jctech888.com.cn

[S05] C：字符串长度
来源：http://hi.lnxyls.cn

strlen(s)
来源：http://hk.gzmigu.cn

[S06] C：字符串比较
来源：http://fi.hnjuh.cn

strcmp(a, b) == 0
来源：http://di.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://uj.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nb.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://ll.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vu.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://ck.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rs.9csxet.cn

[S10] C：指针与解引用
来源：http://ja.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://sv.huanxung.cn

[S11] C：逐行读文件
来源：http://nm.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ci.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://om.bookmarksfly.cn

fclose(f);
来源：http://kh.9csxet.cn

[S12] C：写文件
来源：http://ii.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wx.szsharing.cn

[S13] C：宏定义
来源：http://gd.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://il.hnjuh.cn

[S14] C：枚举
来源：http://on.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://dh.lnxyls.cn

[S15] C：类型转换
来源：http://fc.haigaiapp.cn

(double) a / b
来源：http://wv.shxzskj.cn

[S16] C：位操作置位
来源：http://yu.muxihuayi.cn

x |= (1 << 3);
来源：http://ev.szsharing.cn

[S17] C：安全拼接字符串
来源：http://lg.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wr.shxzukj.cn

[S18] C：命令行参数
来源：http://am.newstarts.cn

int main(int argc, char **argv)
来源：http://dv.hahajie.cn

[S19] C：快速排序
来源：http://zn.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vm.bjjhwx.cn

[S20] C：二分查找
来源：http://xy.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://do.asd995.cn

[S21] C：字符类别判断
来源：http://ul.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mh.hahajie.cn

[S22] C：字符串转数字
来源：http://tq.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://of.huixinmuqiang.cn

[S23] C：随机数
来源：http://bo.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kn.hnjuh.cn

[S24] C：获取本地时间
来源：http://ut.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oq.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://kx.haigaiapp.cn

memcpy(dst, src, n);
来源：http://wb.9csxet.cn

[S26] C：内存清零
来源：http://yw.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://bg.shxzukj.cn

[S27] C：定义常量
来源：http://zm.shxzskj.cn

const double PI = 3.14159;
来源：http://wk.nszjky.cn

[S28] C：静态变量
来源：http://ct.asd995.cn

static int counter = 0;
来源：http://gm.yuexingan06.cn

[S29] C：变参函数
来源：http://gz.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hc.jctech888.com.cn

[S30] C：头文件保护
来源：http://or.shxzukj.cn

#ifndef X_H
来源：http://tz.huixinmuqiang.cn

#define X_H
来源：http://xd.nicolike.cn

#endif
来源：http://ru.muxihuayi.cn

[S31] C++：Hello World
来源：http://rz.lnxyls.cn

#include <iostream>
来源：http://mh.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://al.shxzukj.cn

[S32] C++：字符串
来源：http://as.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://ao.shxzskj.cn

[S33] C++：vector 增删
来源：http://lq.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ry.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://bl.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://fe.yuntaijiaju.cn

[S35] C++：map
来源：http://ny.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xe.521024.cn

[S36] C++：unordered_map
来源：http://qj.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xp.wgjwhj.cn

[S37] C++：set
来源：http://zp.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uw.colortex.cn

[S38] C++：排序
来源：http://av.colortex.cn

std::sort(v.begin(), v.end());
来源：http://im.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://iw.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iz.gzmigu.cn

[S40] C++：查找元素
来源：http://ds.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jr.shxzukj.cn

[S41] C++：类与构造函数
来源：http://lf.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ho.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://yh.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://cx.chemitech.net.cn

[S43] C++：智能指针
来源：http://ke.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://zt.panjiajie.cn

[S44] C++：引用传参
来源：http://rp.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://my.colortex.cn

[S45] C++：lambda
来源：http://zq.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ap.521024.cn

[S46] C++：函数模板
来源：http://mn.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dy.yuexingan06.cn


<!-- 参考信息 -->