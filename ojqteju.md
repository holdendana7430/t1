代发 wailian999

ANALYZE TABLE users;
来源：http://xz.szsharing.cn

[Q71] 查看建表语句
来源：http://vq.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wj.wgjwhj.cn

[Q72] 查看索引
来源：http://uc.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://md.yuexingan06.cn

[Q73] 查看表状态
来源：http://qs.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xa.521024.cn

[Q74] 强制使用索引
来源：http://be.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jk.jctech888.com.cn

[Q75] 日期格式化
来源：http://ed.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sl.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gi.wgjwhj.cn

[Q76] 按天统计
来源：http://ao.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://es.hnjuh.cn

[Q77] 时间加减
来源：http://ok.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mx.bjjhwx.cn

[Q78] 当前时间
来源：http://qa.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hu.huixiangedu.cn

[Q79] 字符串拼接
来源：http://is.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nn.nszjky.cn

[Q80] 字符串截取
来源：http://xe.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ua.9csxet.cn

[Q81] 字符串替换
来源：http://xi.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://md.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://bn.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gx.huanxung.cn

[Q83] 大小写转换
来源：http://gz.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ku.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://ig.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://fq.nszjky.cn

[Q85] 数值取整
来源：http://rd.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://af.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://xd.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ah.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://wz.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gd.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://aa.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sp.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vm.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://tz.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xe.bjjhwx.cn

[Q90] 生成序号列
来源：http://bk.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sr.szxytkj.cn

================================================================================
来源：http://pd.lnxyls.cn

R. Bash 专题
来源：http://tz.asd995.cn

================================================================================
来源：http://ea.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://vm.colortex.cn

#!/usr/bin/env bash
来源：http://wa.jctech888.com.cn

set -euo pipefail
来源：http://sa.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://je.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://fr.muxihuayi.cn

[R03] 只读变量
来源：http://fx.szxytkj.cn

readonly PI=3.14
来源：http://uw.bookmarksfly.cn

[R04] 位置参数
来源：http://fn.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://di.yuexingan06.cn

[R05] 参数默认值
来源：http://rq.521024.cn

name="${1:-default}"
来源：http://rf.asd995.cn

[R06] 判断命令是否存在
来源：http://dz.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fl.newstarts.cn

[R07] if 判断文件
来源：http://gx.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fk.haigaiapp.cn

[R08] 数值比较
来源：http://cg.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xr.asd995.cn

[R09] 字符串比较
来源：http://dv.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jd.gzmigu.cn

[R10] 正则匹配
来源：http://oe.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ji.wgjwhj.cn

[R11] case 多分支
来源：http://qn.bookmarksfly.cn

case "$1" in
来源：http://io.shxzukj.cn

start) echo "启动" ;;
来源：http://io.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://eh.hahajie.cn

*)     echo "未知命令" ;;
来源：http://ln.shxzukj.cn

esac
来源：http://lf.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://xt.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://fo.lnxyls.cn

[R13] for 计数循环
来源：http://jm.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://mt.chemitech.net.cn

[R14] C 风格 for
来源：http://rr.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ok.lnxyls.cn

[R15] while 逐行读文件
来源：http://cc.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hahajie.cn

[R16] until 等待条件
来源：http://ha.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kp.huixiangedu.cn

[R17] 数组定义与取值
来源：http://gx.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://um.shxzukj.cn

[R18] 遍历数组
来源：http://jz.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cg.yuexingan06.cn

[R19] 数组长度
来源：http://ay.panjiajie.cn

echo "${#arr[@]}"
来源：http://fy.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://hx.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://of.wgjwhj.cn

[R21] 字符串长度
来源：http://tc.chemitech.net.cn

echo "${#s}"
来源：http://ja.jianghongdianzi.cn

[R22] 截取子串
来源：http://cb.wgjwhj.cn

echo "${s:0:5}"
来源：http://kc.hahajie.cn

[R23] 字符串替换
来源：http://db.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dr.shxzskj.cn

[R24] 大小写转换
来源：http://km.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nd.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://mj.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jd.shxzukj.cn

[R26] 命令替换
来源：http://hh.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://jm.wgjwhj.cn

[R27] 算术展开
来源：http://xb.colortex.cn

echo $((1 + 2 * 3))
来源：http://ec.hnjuh.cn

[R28] 浮点运算
来源：http://wn.521024.cn

echo "scale=2; 10/3" | bc
来源：http://qx.huixinmuqiang.cn

[R29] 定义函数
来源：http://fs.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pf.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://oi.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://im.panjiajie.cn

[R31] 局部变量
来源：http://ww.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://st.huixiangedu.cn

[R32] 参数个数校验
来源：http://xz.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yc.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://hd.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://he.panjiajie.cn

[R34] 退出时清理
来源：http://yn.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nj.wgjwhj.cn

[R35] 后台执行并等待
来源：http://ib.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nb.huanxung.cn

[R36] 并发执行多个任务
来源：http://om.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ca.colortex.cn

[R37] 把输出赋给变量
来源：http://fd.521024.cn

files=$(ls -1)
来源：http://ye.nicolike.cn

[R38] 管道串联
来源：http://eu.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://to.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://nx.gzmigu.cn

cmd > out.log 2>&1
来源：http://jm.hahajie.cn

[R40] 追加写日志
来源：http://fj.huanxung.cn

echo "log" >> out.log
来源：http://mm.muxihuayi.cn

[R41] 丢弃输出
来源：http://ts.nszjky.cn

cmd >/dev/null 2>&1
来源：http://ad.muxihuayi.cn

[R42] 输入重定向
来源：http://hb.jianghongdianzi.cn

wc -l < a.txt
来源：http://li.jctech888.com.cn

[R43] 按名字查找文件
来源：http://ou.shtwfgs.cn

find . -name "*.log" -type f
来源：http://ky.haigaiapp.cn

[R44] 按修改时间查找
来源：http://so.9csxet.cn

find . -mtime -7 -type f
来源：http://qk.huanxung.cn

[R45] 批量删除
来源：http://di.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://xt.lnxyls.cn

[R46] 递归替换文件内容
来源：http://lu.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eh.haigaiapp.cn

[R47] sed 单行替换
来源：http://sx.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ya.nicolike.cn

[R48] awk 取指定列
来源：http://lb.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://gs.lnxyls.cn

[R49] awk 带条件
来源：http://ot.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ld.lnxyls.cn

[R50] awk 求和
来源：http://ex.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bz.muxihuayi.cn

[R51] 排序去重取前几
来源：http://uv.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pf.9csxet.cn

[R52] 统计行数
来源：http://cc.huanxung.cn

wc -l a.txt
来源：http://ua.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://vf.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rn.nszjky.cn

[R54] 比较两个文件
来源：http://mv.yuexingan06.cn

diff a.txt b.txt
来源：http://nl.shxzskj.cn

[R55] 压缩与解压
来源：http://ph.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tl.haigaiapp.cn

[R56] 远程拷贝
来源：http://lz.gzmigu.cn

scp file user@host:/path/
来源：http://ig.gzmigu.cn

[R57] 远程执行命令
来源：http://ue.szsharing.cn

ssh user@host 'uptime'
来源：http://ea.lnxyls.cn

[R58] 下载文件
来源：http://ut.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zs.lnxyls.cn

[R59] 发 POST JSON
来源：http://re.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gu.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://px.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://na.newstarts.cn

[R61] 磁盘占用
来源：http://lc.hnjuh.cn

df -h;  du -sh *
来源：http://hx.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://pl.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://aa.lnxyls.cn

[R63] 内存与进程
来源：http://rw.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://yl.hahajie.cn

[R64] 结束进程
来源：http://yu.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://ko.panjiajie.cn

[R65] 查看端口占用
来源：http://ac.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pk.huixiangedu.cn

[R66] 定时任务
来源：http://hw.wgjwhj.cn

crontab -e;  crontab -l
来源：http://dy.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://kn.shxzskj.cn

openssl rand -hex 16
来源：http://ha.chemitech.net.cn

[R68] 计算文件校验值
来源：http://rj.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ft.muxihuayi.cn

[R69] 生成随机密码
来源：http://hv.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://st.gzmigu.cn

[R70] 时间戳与互转
来源：http://qf.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://hy.hahajie.cn

[R71] 日期格式化
来源：http://bh.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wj.lnxyls.cn

[R72] 等待端口就绪
来源：http://ul.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xb.lnxyls.cn

[R73] 分割大日志
来源：http://ol.muxihuayi.cn

split -l 1000 big.log part_
来源：http://kc.yuexingan06.cn

[R74] 批量重命名
来源：http://or.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lm.panjiajie.cn

[R75] 导出环境变量
来源：http://pg.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://kd.nszjky.cn

[R76] 使用临时文件
来源：http://gi.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eh.huixiangedu.cn

[R77] 读取用户输入
来源：http://wo.szxytkj.cn

read -rp "请输入: " ans
来源：http://jx.hnjuh.cn

[R78] 交互式菜单
来源：http://nw.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ft.9csxet.cn

[R79] 解析命令行选项
来源：http://xm.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vy.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://uv.chemitech.net.cn

time ./run.sh
来源：http://gr.hnjuh.cn

================================================================================
来源：http://lo.asd995.cn

S. C / C++ 专题
来源：http://ap.shxzukj.cn

================================================================================
来源：http://nc.szsharing.cn

[S01] C：Hello World
来源：http://fb.hnjuh.cn

#include <stdio.h>
来源：http://ag.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oo.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://kl.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://ma.yuexingan06.cn

[S03] C：读入整数
来源：http://ws.lnxyls.cn

int x; scanf("%d", &x);
来源：http://uq.shtwfgs.cn

[S04] C：字符串复制
来源：http://cu.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rb.hnjuh.cn

[S05] C：字符串长度
来源：http://wt.jianghongdianzi.cn

strlen(s)
来源：http://gq.hahajie.cn

[S06] C：字符串比较
来源：http://fk.hahajie.cn

strcmp(a, b) == 0
来源：http://le.shxzskj.cn

[S07] C：数组遍历求和
来源：http://hb.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ym.asd995.cn

[S08] C：动态内存分配与释放
来源：http://lq.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ty.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://vq.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lc.panjiajie.cn

[S10] C：指针与解引用
来源：http://ju.asd995.cn

int *p = &a;  *p = 5;
来源：http://ld.asd995.cn

[S11] C：逐行读文件
来源：http://no.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://pe.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://is.shtwfgs.cn

fclose(f);
来源：http://du.nicolike.cn

[S12] C：写文件
来源：http://ta.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nf.yuexingan06.cn

[S13] C：宏定义
来源：http://st.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tm.521024.cn

[S14] C：枚举
来源：http://yh.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://tp.nszjky.cn

[S15] C：类型转换
来源：http://hq.yuntaijiaju.cn

(double) a / b
来源：http://mb.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://bd.yuntaijiaju.cn

x |= (1 << 3);
来源：http://qn.521024.cn

[S17] C：安全拼接字符串
来源：http://dn.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lu.colortex.cn

[S18] C：命令行参数
来源：http://dv.hnjuh.cn

int main(int argc, char **argv)
来源：http://bu.nszjky.cn

[S19] C：快速排序
来源：http://iz.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ty.gzmigu.cn

[S20] C：二分查找
来源：http://wt.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mn.hnjuh.cn

[S21] C：字符类别判断
来源：http://wx.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://co.shxzskj.cn

[S22] C：字符串转数字
来源：http://qr.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fc.szxytkj.cn

[S23] C：随机数
来源：http://nj.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gh.panjiajie.cn

[S24] C：获取本地时间
来源：http://mk.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dv.huixiangedu.cn

[S25] C：内存拷贝
来源：http://fw.wgjwhj.cn

memcpy(dst, src, n);
来源：http://rx.shtwfgs.cn

[S26] C：内存清零
来源：http://sq.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://fn.colortex.cn

[S27] C：定义常量
来源：http://bo.colortex.cn

const double PI = 3.14159;
来源：http://cv.jctech888.com.cn

[S28] C：静态变量
来源：http://sa.lnxyls.cn

static int counter = 0;
来源：http://qc.shtwfgs.cn

[S29] C：变参函数
来源：http://xc.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cz.wgjwhj.cn

[S30] C：头文件保护
来源：http://aq.yuexingan06.cn

#ifndef X_H
来源：http://cm.yuntaijiaju.cn

#define X_H
来源：http://ip.shtwfgs.cn

#endif
来源：http://tg.lnxyls.cn

[S31] C++：Hello World
来源：http://zp.shxzskj.cn

#include <iostream>
来源：http://mv.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://wv.yuexingan06.cn

[S32] C++：字符串
来源：http://jx.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://gc.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://kt.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gw.gzmigu.cn

[S34] C++：遍历 vector
来源：http://zu.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://zt.shxzskj.cn

[S35] C++：map
来源：http://xf.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fs.gzmigu.cn

[S36] C++：unordered_map
来源：http://ka.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tf.szxytkj.cn

[S37] C++：set
来源：http://ef.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jy.bookmarksfly.cn

[S38] C++：排序
来源：http://gp.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://al.521024.cn

[S39] C++：自定义比较器排序
来源：http://gp.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bf.haigaiapp.cn

[S40] C++：查找元素
来源：http://az.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gw.bjjhwx.cn


<!-- 参考信息 -->