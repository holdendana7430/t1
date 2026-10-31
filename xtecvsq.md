代发 wailian999

ROLLBACK TO sp1;
来源：http://uw.wgjwhj.cn

[Q69] 查看执行计划
来源：http://ky.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://we.szsharing.cn

[Q70] 更新统计信息
来源：http://qe.shxzukj.cn

ANALYZE TABLE users;
来源：http://vd.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://yf.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vp.asd995.cn

[Q72] 查看索引
来源：http://ub.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://ha.newstarts.cn

[Q73] 查看表状态
来源：http://an.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pt.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://ae.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gh.colortex.cn

[Q75] 日期格式化
来源：http://an.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://os.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vf.shtwfgs.cn

[Q76] 按天统计
来源：http://no.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rp.521024.cn

[Q77] 时间加减
来源：http://wu.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ne.muxihuayi.cn

[Q78] 当前时间
来源：http://hv.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xd.shtwfgs.cn

[Q79] 字符串拼接
来源：http://ob.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fk.gzmigu.cn

[Q80] 字符串截取
来源：http://rg.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nj.lnxyls.cn

[Q81] 字符串替换
来源：http://lz.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gq.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://yj.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kn.haigaiapp.cn

[Q83] 大小写转换
来源：http://gr.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ae.521024.cn

[Q84] 去除首尾空格
来源：http://qj.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://pt.huixinmuqiang.cn

[Q85] 数值取整
来源：http://de.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yw.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://ts.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ko.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://yn.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ir.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://ey.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fl.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jh.szsharing.cn

[Q89] 判断表是否存在
来源：http://cm.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qg.shtwfgs.cn

[Q90] 生成序号列
来源：http://hk.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pv.chemitech.net.cn

================================================================================
来源：http://gi.yuexingan06.cn

R. Bash 专题
来源：http://pa.jianghongdianzi.cn

================================================================================
来源：http://fj.asd995.cn

[R01] shebang 与严格模式
来源：http://ou.colortex.cn

#!/usr/bin/env bash
来源：http://zz.szsharing.cn

set -euo pipefail
来源：http://yo.hahajie.cn

[R02] 变量赋值与使用
来源：http://du.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://fj.521024.cn

[R03] 只读变量
来源：http://if.gzmigu.cn

readonly PI=3.14
来源：http://ok.shxzskj.cn

[R04] 位置参数
来源：http://vo.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://da.521024.cn

[R05] 参数默认值
来源：http://hv.colortex.cn

name="${1:-default}"
来源：http://dy.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://fo.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qk.panjiajie.cn

[R07] if 判断文件
来源：http://lt.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lb.szxytkj.cn

[R08] 数值比较
来源：http://zu.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dx.muxihuayi.cn

[R09] 字符串比较
来源：http://mv.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://du.9csxet.cn

[R10] 正则匹配
来源：http://az.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lz.yuexingan06.cn

[R11] case 多分支
来源：http://rj.jianghongdianzi.cn

case "$1" in
来源：http://gm.gzmigu.cn

start) echo "启动" ;;
来源：http://co.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://nq.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://bq.521024.cn

esac
来源：http://yj.panjiajie.cn

[R12] for 遍历文件
来源：http://pa.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://fi.szxytkj.cn

[R13] for 计数循环
来源：http://kx.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://zc.wgjwhj.cn

[R14] C 风格 for
来源：http://lk.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://si.shtwfgs.cn

[R15] while 逐行读文件
来源：http://vc.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ys.newstarts.cn

[R16] until 等待条件
来源：http://vq.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uc.chemitech.net.cn

[R17] 数组定义与取值
来源：http://oj.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ru.huanxung.cn

[R18] 遍历数组
来源：http://dt.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://md.lnxyls.cn

[R19] 数组长度
来源：http://hi.huixiangedu.cn

echo "${#arr[@]}"
来源：http://mc.gzmigu.cn

[R20] 关联数组（字典）
来源：http://gr.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qf.9csxet.cn

[R21] 字符串长度
来源：http://qv.yuexingan06.cn

echo "${#s}"
来源：http://co.bjjhwx.cn

[R22] 截取子串
来源：http://nu.huanxung.cn

echo "${s:0:5}"
来源：http://nl.jctech888.com.cn

[R23] 字符串替换
来源：http://qd.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gf.hnjuh.cn

[R24] 大小写转换
来源：http://to.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kq.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://hj.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dc.9csxet.cn

[R26] 命令替换
来源：http://ib.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://iy.gzmigu.cn

[R27] 算术展开
来源：http://sa.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://gp.yuntaijiaju.cn

[R28] 浮点运算
来源：http://uc.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://fo.colortex.cn

[R29] 定义函数
来源：http://bi.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zk.9csxet.cn

[R30] 函数返回状态码
来源：http://ch.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://ip.shxzukj.cn

[R31] 局部变量
来源：http://dg.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://rz.jctech888.com.cn

[R32] 参数个数校验
来源：http://mc.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zu.asd995.cn

[R33] 捕获错误并提示行号
来源：http://iv.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oc.jianghongdianzi.cn

[R34] 退出时清理
来源：http://bi.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qo.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://qu.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dp.nszjky.cn

[R36] 并发执行多个任务
来源：http://wr.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://id.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://ve.szsharing.cn

files=$(ls -1)
来源：http://ns.hnjuh.cn

[R38] 管道串联
来源：http://cb.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://pe.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://np.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://px.jctech888.com.cn

[R40] 追加写日志
来源：http://yb.haigaiapp.cn

echo "log" >> out.log
来源：http://yq.nszjky.cn

[R41] 丢弃输出
来源：http://zm.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://wc.wgjwhj.cn

[R42] 输入重定向
来源：http://ao.jctech888.com.cn

wc -l < a.txt
来源：http://tz.nicolike.cn

[R43] 按名字查找文件
来源：http://ff.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://zy.bjjhwx.cn

[R44] 按修改时间查找
来源：http://gi.shtwfgs.cn

find . -mtime -7 -type f
来源：http://az.chemitech.net.cn

[R45] 批量删除
来源：http://pg.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://vm.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://hd.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://il.newstarts.cn

[R47] sed 单行替换
来源：http://de.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fi.muxihuayi.cn

[R48] awk 取指定列
来源：http://nt.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://pe.jctech888.com.cn

[R49] awk 带条件
来源：http://bv.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ig.nicolike.cn

[R50] awk 求和
来源：http://jf.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jt.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://rj.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ek.jianghongdianzi.cn

[R52] 统计行数
来源：http://lj.huixinmuqiang.cn

wc -l a.txt
来源：http://dy.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://ce.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vn.colortex.cn

[R54] 比较两个文件
来源：http://ju.panjiajie.cn

diff a.txt b.txt
来源：http://ta.haigaiapp.cn

[R55] 压缩与解压
来源：http://ti.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ax.huixiangedu.cn

[R56] 远程拷贝
来源：http://dn.521024.cn

scp file user@host:/path/
来源：http://dq.huixiangedu.cn

[R57] 远程执行命令
来源：http://sv.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://wd.521024.cn

[R58] 下载文件
来源：http://bf.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aa.asd995.cn

[R59] 发 POST JSON
来源：http://bc.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hp.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://lj.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qf.huanxung.cn

[R61] 磁盘占用
来源：http://lu.jianghongdianzi.cn

df -h;  du -sh *
来源：http://nv.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://aw.colortex.cn

du -ah . | sort -rh | head -10
来源：http://bd.jianghongdianzi.cn

[R63] 内存与进程
来源：http://pf.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://mh.hahajie.cn

[R64] 结束进程
来源：http://wr.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://iw.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://lq.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ke.colortex.cn

[R66] 定时任务
来源：http://hk.jctech888.com.cn

crontab -e;  crontab -l
来源：http://un.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://te.hnjuh.cn

openssl rand -hex 16
来源：http://ek.asd995.cn

[R68] 计算文件校验值
来源：http://uw.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xy.yuexingan06.cn

[R69] 生成随机密码
来源：http://tx.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://aa.wgjwhj.cn

[R70] 时间戳与互转
来源：http://az.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://jo.jctech888.com.cn

[R71] 日期格式化
来源：http://pg.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bo.colortex.cn

[R72] 等待端口就绪
来源：http://by.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://si.colortex.cn

[R73] 分割大日志
来源：http://ff.9csxet.cn

split -l 1000 big.log part_
来源：http://qc.colortex.cn

[R74] 批量重命名
来源：http://yo.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vs.shxzukj.cn

[R75] 导出环境变量
来源：http://va.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ve.nszjky.cn

[R76] 使用临时文件
来源：http://mj.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ed.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://av.nicolike.cn

read -rp "请输入: " ans
来源：http://cl.szsharing.cn

[R78] 交互式菜单
来源：http://qc.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tq.9csxet.cn

[R79] 解析命令行选项
来源：http://ln.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ld.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://pe.huixiangedu.cn

time ./run.sh
来源：http://wy.huixinmuqiang.cn

================================================================================
来源：http://ey.nicolike.cn

S. C / C++ 专题
来源：http://ce.shxzskj.cn

================================================================================
来源：http://ui.yuntaijiaju.cn

[S01] C：Hello World
来源：http://pt.nszjky.cn

#include <stdio.h>
来源：http://qn.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uj.hahajie.cn

[S02] C：变量与格式化输出
来源：http://lw.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://od.lnxyls.cn

[S03] C：读入整数
来源：http://pu.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://rt.huanxung.cn

[S04] C：字符串复制
来源：http://zm.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dl.asd995.cn

[S05] C：字符串长度
来源：http://jl.newstarts.cn

strlen(s)
来源：http://hv.nicolike.cn

[S06] C：字符串比较
来源：http://at.lnxyls.cn

strcmp(a, b) == 0
来源：http://vn.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://nv.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jc.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://kl.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wd.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://sa.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://np.hnjuh.cn

[S10] C：指针与解引用
来源：http://ai.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://ud.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://ud.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://eh.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sw.lnxyls.cn

fclose(f);
来源：http://vg.9csxet.cn

[S12] C：写文件
来源：http://cu.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xb.huixinmuqiang.cn

[S13] C：宏定义
来源：http://mx.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ul.colortex.cn

[S14] C：枚举
来源：http://am.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://rt.yuexingan06.cn

[S15] C：类型转换
来源：http://un.nszjky.cn

(double) a / b
来源：http://vz.521024.cn

[S16] C：位操作置位
来源：http://uq.huanxung.cn

x |= (1 << 3);
来源：http://av.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://us.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wv.jctech888.com.cn

[S18] C：命令行参数
来源：http://jw.lnxyls.cn

int main(int argc, char **argv)
来源：http://wo.newstarts.cn

[S19] C：快速排序
来源：http://fh.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kd.huanxung.cn

[S20] C：二分查找
来源：http://nb.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jz.nszjky.cn

[S21] C：字符类别判断
来源：http://qr.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xh.hnjuh.cn

[S22] C：字符串转数字
来源：http://zt.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://na.nszjky.cn

[S23] C：随机数
来源：http://rw.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ns.nicolike.cn

[S24] C：获取本地时间
来源：http://wz.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pr.lnxyls.cn

[S25] C：内存拷贝
来源：http://zw.nicolike.cn

memcpy(dst, src, n);
来源：http://hs.huanxung.cn

[S26] C：内存清零
来源：http://rs.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://bw.muxihuayi.cn

[S27] C：定义常量
来源：http://jh.colortex.cn

const double PI = 3.14159;
来源：http://fh.yuexingan06.cn

[S28] C：静态变量
来源：http://fn.panjiajie.cn

static int counter = 0;
来源：http://ym.panjiajie.cn

[S29] C：变参函数
来源：http://ua.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kk.chemitech.net.cn

[S30] C：头文件保护
来源：http://za.huanxung.cn

#ifndef X_H
来源：http://ly.jianghongdianzi.cn

#define X_H
来源：http://al.shxzukj.cn

#endif
来源：http://mz.nszjky.cn

[S31] C++：Hello World
来源：http://zt.bjjhwx.cn

#include <iostream>
来源：http://gi.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://cv.haigaiapp.cn

[S32] C++：字符串
来源：http://ae.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://aq.shxzskj.cn

[S33] C++：vector 增删
来源：http://yu.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gd.newstarts.cn

[S34] C++：遍历 vector
来源：http://ey.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://je.shxzukj.cn

[S35] C++：map
来源：http://zt.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nc.521024.cn

[S36] C++：unordered_map
来源：http://em.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vv.shxzskj.cn

[S37] C++：set
来源：http://ph.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://no.shxzukj.cn

[S38] C++：排序
来源：http://at.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://am.yuntaijiaju.cn


<!-- 参考信息 -->