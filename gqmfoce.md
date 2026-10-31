代发 wailian999

ANALYZE TABLE users;
来源：http://pe.colortex.cn

[Q71] 查看建表语句
来源：http://yo.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ab.huixinmuqiang.cn

[Q72] 查看索引
来源：http://zg.hahajie.cn

SHOW INDEX FROM users;
来源：http://xm.huixiangedu.cn

[Q73] 查看表状态
来源：http://gl.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xr.muxihuayi.cn

[Q74] 强制使用索引
来源：http://yb.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tg.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://bm.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://so.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bf.bjjhwx.cn

[Q76] 按天统计
来源：http://pd.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://te.asd995.cn

[Q77] 时间加减
来源：http://pp.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jo.haigaiapp.cn

[Q78] 当前时间
来源：http://ql.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mc.szxytkj.cn

[Q79] 字符串拼接
来源：http://lq.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yt.shxzskj.cn

[Q80] 字符串截取
来源：http://sx.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bi.huixiangedu.cn

[Q81] 字符串替换
来源：http://af.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nw.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://db.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xt.nicolike.cn

[Q83] 大小写转换
来源：http://da.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nh.colortex.cn

[Q84] 去除首尾空格
来源：http://kl.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://xp.huanxung.cn

[Q85] 数值取整
来源：http://ch.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lw.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://xk.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pj.521024.cn

[Q87] JSON 字段做条件
来源：http://xi.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zz.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://nj.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wz.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ah.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://kz.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yv.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://xg.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rv.hnjuh.cn

================================================================================
来源：http://iu.lnxyls.cn

R. Bash 专题
来源：http://ri.gzmigu.cn

================================================================================
来源：http://ov.shxzukj.cn

[R01] shebang 与严格模式
来源：http://ug.newstarts.cn

#!/usr/bin/env bash
来源：http://wi.9csxet.cn

set -euo pipefail
来源：http://ry.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://tc.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://ho.gzmigu.cn

[R03] 只读变量
来源：http://mb.jctech888.com.cn

readonly PI=3.14
来源：http://fn.huixinmuqiang.cn

[R04] 位置参数
来源：http://ss.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://er.panjiajie.cn

[R05] 参数默认值
来源：http://re.muxihuayi.cn

name="${1:-default}"
来源：http://kc.gzmigu.cn

[R06] 判断命令是否存在
来源：http://hb.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://an.gzmigu.cn

[R07] if 判断文件
来源：http://ch.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wa.bjjhwx.cn

[R08] 数值比较
来源：http://se.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://km.lnxyls.cn

[R09] 字符串比较
来源：http://rk.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cv.haigaiapp.cn

[R10] 正则匹配
来源：http://zg.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ql.yuexingan06.cn

[R11] case 多分支
来源：http://sf.newstarts.cn

case "$1" in
来源：http://tj.huixiangedu.cn

start) echo "启动" ;;
来源：http://aq.shxzskj.cn

stop)  echo "停止" ;;
来源：http://pg.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://xc.asd995.cn

esac
来源：http://ut.hahajie.cn

[R12] for 遍历文件
来源：http://yh.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://dz.hahajie.cn

[R13] for 计数循环
来源：http://st.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://si.yuntaijiaju.cn

[R14] C 风格 for
来源：http://bd.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oo.hnjuh.cn

[R15] while 逐行读文件
来源：http://pu.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zm.wgjwhj.cn

[R16] until 等待条件
来源：http://ya.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oe.wgjwhj.cn

[R17] 数组定义与取值
来源：http://os.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ih.asd995.cn

[R18] 遍历数组
来源：http://uv.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yk.9csxet.cn

[R19] 数组长度
来源：http://zn.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://zl.lnxyls.cn

[R20] 关联数组（字典）
来源：http://hi.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pt.yuntaijiaju.cn

[R21] 字符串长度
来源：http://pf.muxihuayi.cn

echo "${#s}"
来源：http://ht.shxzskj.cn

[R22] 截取子串
来源：http://so.521024.cn

echo "${s:0:5}"
来源：http://qc.muxihuayi.cn

[R23] 字符串替换
来源：http://rw.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eb.jianghongdianzi.cn

[R24] 大小写转换
来源：http://ye.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ho.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://fs.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://so.521024.cn

[R26] 命令替换
来源：http://hq.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://th.newstarts.cn

[R27] 算术展开
来源：http://te.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://jj.9csxet.cn

[R28] 浮点运算
来源：http://ac.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://tj.yuntaijiaju.cn

[R29] 定义函数
来源：http://ik.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ut.yuexingan06.cn

[R30] 函数返回状态码
来源：http://nz.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://zr.9csxet.cn

[R31] 局部变量
来源：http://gi.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://ac.521024.cn

[R32] 参数个数校验
来源：http://dq.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oe.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://sz.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ym.hnjuh.cn

[R34] 退出时清理
来源：http://aw.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uf.9csxet.cn

[R35] 后台执行并等待
来源：http://dg.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tf.shxzskj.cn

[R36] 并发执行多个任务
来源：http://ei.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fv.shxzukj.cn

[R37] 把输出赋给变量
来源：http://dz.9csxet.cn

files=$(ls -1)
来源：http://rp.nicolike.cn

[R38] 管道串联
来源：http://hf.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://il.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://wf.szsharing.cn

cmd > out.log 2>&1
来源：http://ew.lnxyls.cn

[R40] 追加写日志
来源：http://gj.panjiajie.cn

echo "log" >> out.log
来源：http://tq.colortex.cn

[R41] 丢弃输出
来源：http://zg.nszjky.cn

cmd >/dev/null 2>&1
来源：http://wk.szxytkj.cn

[R42] 输入重定向
来源：http://zj.jianghongdianzi.cn

wc -l < a.txt
来源：http://sn.yuexingan06.cn

[R43] 按名字查找文件
来源：http://my.gzmigu.cn

find . -name "*.log" -type f
来源：http://gc.gzmigu.cn

[R44] 按修改时间查找
来源：http://fy.szxytkj.cn

find . -mtime -7 -type f
来源：http://av.9csxet.cn

[R45] 批量删除
来源：http://nb.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://gc.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://ap.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vh.asd995.cn

[R47] sed 单行替换
来源：http://cz.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sy.bookmarksfly.cn

[R48] awk 取指定列
来源：http://bg.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://xs.bookmarksfly.cn

[R49] awk 带条件
来源：http://te.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uo.jianghongdianzi.cn

[R50] awk 求和
来源：http://ld.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pk.jctech888.com.cn

[R51] 排序去重取前几
来源：http://va.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mk.huanxung.cn

[R52] 统计行数
来源：http://ev.panjiajie.cn

wc -l a.txt
来源：http://ts.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://nm.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wa.wgjwhj.cn

[R54] 比较两个文件
来源：http://ks.hnjuh.cn

diff a.txt b.txt
来源：http://kf.nicolike.cn

[R55] 压缩与解压
来源：http://mc.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tc.colortex.cn

[R56] 远程拷贝
来源：http://kr.nicolike.cn

scp file user@host:/path/
来源：http://zw.gzmigu.cn

[R57] 远程执行命令
来源：http://wd.nicolike.cn

ssh user@host 'uptime'
来源：http://qw.lnxyls.cn

[R58] 下载文件
来源：http://pc.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xd.wgjwhj.cn

[R59] 发 POST JSON
来源：http://gp.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fa.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://gv.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kg.521024.cn

[R61] 磁盘占用
来源：http://st.muxihuayi.cn

df -h;  du -sh *
来源：http://dq.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://nd.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://sg.nszjky.cn

[R63] 内存与进程
来源：http://wr.colortex.cn

free -h;  ps aux | grep nginx
来源：http://gc.jctech888.com.cn

[R64] 结束进程
来源：http://od.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://fg.huixiangedu.cn

[R65] 查看端口占用
来源：http://to.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gq.lnxyls.cn

[R66] 定时任务
来源：http://jf.colortex.cn

crontab -e;  crontab -l
来源：http://dj.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://wb.yuexingan06.cn

openssl rand -hex 16
来源：http://oq.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://qd.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://um.shtwfgs.cn

[R69] 生成随机密码
来源：http://hn.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://nk.asd995.cn

[R70] 时间戳与互转
来源：http://iw.huanxung.cn

date +%s;  date -d @1700000000
来源：http://xg.bookmarksfly.cn

[R71] 日期格式化
来源：http://qn.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ya.shxzukj.cn

[R72] 等待端口就绪
来源：http://ig.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jn.9csxet.cn

[R73] 分割大日志
来源：http://dq.jctech888.com.cn

split -l 1000 big.log part_
来源：http://hm.521024.cn

[R74] 批量重命名
来源：http://ic.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://je.panjiajie.cn

[R75] 导出环境变量
来源：http://ft.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://ar.yuexingan06.cn

[R76] 使用临时文件
来源：http://yg.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://we.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://qq.huixiangedu.cn

read -rp "请输入: " ans
来源：http://ii.huanxung.cn

[R78] 交互式菜单
来源：http://ki.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://di.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://zp.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yi.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://bd.bookmarksfly.cn

time ./run.sh
来源：http://sk.gzmigu.cn

================================================================================
来源：http://rt.wgjwhj.cn

S. C / C++ 专题
来源：http://al.gzmigu.cn

================================================================================
来源：http://ai.nszjky.cn

[S01] C：Hello World
来源：http://ys.muxihuayi.cn

#include <stdio.h>
来源：http://aj.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vf.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://vv.521024.cn

int a = 10; printf("%d\n", a);
来源：http://em.huanxung.cn

[S03] C：读入整数
来源：http://yj.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://ab.chemitech.net.cn

[S04] C：字符串复制
来源：http://hg.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kn.shxzskj.cn

[S05] C：字符串长度
来源：http://iz.newstarts.cn

strlen(s)
来源：http://yr.shxzukj.cn

[S06] C：字符串比较
来源：http://ze.haigaiapp.cn

strcmp(a, b) == 0
来源：http://gz.panjiajie.cn

[S07] C：数组遍历求和
来源：http://er.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yw.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ga.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aa.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://wt.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xw.9csxet.cn

[S10] C：指针与解引用
来源：http://to.hahajie.cn

int *p = &a;  *p = 5;
来源：http://oe.szxytkj.cn

[S11] C：逐行读文件
来源：http://fg.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ka.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ug.asd995.cn

fclose(f);
来源：http://vp.chemitech.net.cn

[S12] C：写文件
来源：http://ao.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pq.huixinmuqiang.cn

[S13] C：宏定义
来源：http://vu.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kc.9csxet.cn

[S14] C：枚举
来源：http://iz.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://oq.bookmarksfly.cn

[S15] C：类型转换
来源：http://di.bookmarksfly.cn

(double) a / b
来源：http://rq.szxytkj.cn

[S16] C：位操作置位
来源：http://ov.newstarts.cn

x |= (1 << 3);
来源：http://fd.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://eq.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hq.panjiajie.cn

[S18] C：命令行参数
来源：http://mw.shxzskj.cn

int main(int argc, char **argv)
来源：http://fb.lnxyls.cn

[S19] C：快速排序
来源：http://of.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nr.asd995.cn

[S20] C：二分查找
来源：http://sh.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mc.lnxyls.cn

[S21] C：字符类别判断
来源：http://pj.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zh.hnjuh.cn

[S22] C：字符串转数字
来源：http://lv.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cp.yuexingan06.cn

[S23] C：随机数
来源：http://jg.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ci.muxihuayi.cn

[S24] C：获取本地时间
来源：http://ro.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://er.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://vy.newstarts.cn

memcpy(dst, src, n);
来源：http://as.bookmarksfly.cn

[S26] C：内存清零
来源：http://re.colortex.cn

memset(a, 0, sizeof a);
来源：http://pt.wgjwhj.cn

[S27] C：定义常量
来源：http://an.shxzskj.cn

const double PI = 3.14159;
来源：http://vf.yuntaijiaju.cn

[S28] C：静态变量
来源：http://zn.yuexingan06.cn

static int counter = 0;
来源：http://zi.jctech888.com.cn

[S29] C：变参函数
来源：http://ip.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vq.asd995.cn

[S30] C：头文件保护
来源：http://om.panjiajie.cn

#ifndef X_H
来源：http://vx.bookmarksfly.cn

#define X_H
来源：http://rp.bookmarksfly.cn

#endif
来源：http://nm.gzmigu.cn

[S31] C++：Hello World
来源：http://kc.asd995.cn

#include <iostream>
来源：http://bm.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://yo.nszjky.cn

[S32] C++：字符串
来源：http://zz.asd995.cn

std::string s = "hi";  s += "!";
来源：http://iz.lnxyls.cn

[S33] C++：vector 增删
来源：http://yc.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qs.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://yq.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://zb.bookmarksfly.cn

[S35] C++：map
来源：http://lk.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pl.chemitech.net.cn

[S36] C++：unordered_map
来源：http://tk.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://id.shtwfgs.cn

[S37] C++：set
来源：http://ll.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fp.gzmigu.cn

[S38] C++：排序
来源：http://fd.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://te.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://gq.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mp.haigaiapp.cn

[S40] C++：查找元素
来源：http://dr.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cj.jianghongdianzi.cn


<!-- 参考信息 -->