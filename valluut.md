代发 wailian999

[Q67] 设置隔离级别
来源：http://oc.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ww.nszjky.cn

[Q68] 保存点
来源：http://hl.shtwfgs.cn

SAVEPOINT sp1;
来源：http://bu.szsharing.cn

ROLLBACK TO sp1;
来源：http://bw.asd995.cn

[Q69] 查看执行计划
来源：http://vc.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pj.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://ol.yuexingan06.cn

ANALYZE TABLE users;
来源：http://im.yuexingan06.cn

[Q71] 查看建表语句
来源：http://mn.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dh.yuntaijiaju.cn

[Q72] 查看索引
来源：http://ro.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://fx.shxzukj.cn

[Q73] 查看表状态
来源：http://fw.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://en.szsharing.cn

[Q74] 强制使用索引
来源：http://qn.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ud.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://ty.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ay.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wx.jctech888.com.cn

[Q76] 按天统计
来源：http://tt.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ls.asd995.cn

[Q77] 时间加减
来源：http://gy.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uq.muxihuayi.cn

[Q78] 当前时间
来源：http://oq.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yo.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://ug.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gi.gzmigu.cn

[Q80] 字符串截取
来源：http://hk.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://if.hahajie.cn

[Q81] 字符串替换
来源：http://ye.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cc.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://xj.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ro.9csxet.cn

[Q83] 大小写转换
来源：http://mb.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://he.nszjky.cn

[Q84] 去除首尾空格
来源：http://wz.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://nc.yuntaijiaju.cn

[Q85] 数值取整
来源：http://yq.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bi.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://qd.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nq.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://cq.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kj.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://sy.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wi.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nt.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://fp.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vt.nicolike.cn

[Q90] 生成序号列
来源：http://aw.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aj.shxzskj.cn

================================================================================
来源：http://da.yuexingan06.cn

R. Bash 专题
来源：http://ch.newstarts.cn

================================================================================
来源：http://ap.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://rv.newstarts.cn

#!/usr/bin/env bash
来源：http://fp.wgjwhj.cn

set -euo pipefail
来源：http://cy.panjiajie.cn

[R02] 变量赋值与使用
来源：http://sy.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://ou.lnxyls.cn

[R03] 只读变量
来源：http://bs.yuntaijiaju.cn

readonly PI=3.14
来源：http://zy.bjjhwx.cn

[R04] 位置参数
来源：http://ma.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bt.huixinmuqiang.cn

[R05] 参数默认值
来源：http://tk.huanxung.cn

name="${1:-default}"
来源：http://ss.nszjky.cn

[R06] 判断命令是否存在
来源：http://xw.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sa.panjiajie.cn

[R07] if 判断文件
来源：http://wj.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mg.chemitech.net.cn

[R08] 数值比较
来源：http://mv.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ui.lnxyls.cn

[R09] 字符串比较
来源：http://zu.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zk.shtwfgs.cn

[R10] 正则匹配
来源：http://fr.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oz.newstarts.cn

[R11] case 多分支
来源：http://yw.lnxyls.cn

case "$1" in
来源：http://hn.jctech888.com.cn

start) echo "启动" ;;
来源：http://oh.szxytkj.cn

stop)  echo "停止" ;;
来源：http://tp.newstarts.cn

*)     echo "未知命令" ;;
来源：http://kq.muxihuayi.cn

esac
来源：http://fh.gzmigu.cn

[R12] for 遍历文件
来源：http://fb.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://am.huixinmuqiang.cn

[R13] for 计数循环
来源：http://qh.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://hd.shxzukj.cn

[R14] C 风格 for
来源：http://fp.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kj.newstarts.cn

[R15] while 逐行读文件
来源：http://ms.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://un.bjjhwx.cn

[R16] until 等待条件
来源：http://ho.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jb.muxihuayi.cn

[R17] 数组定义与取值
来源：http://bs.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hm.9csxet.cn

[R18] 遍历数组
来源：http://tr.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dq.nicolike.cn

[R19] 数组长度
来源：http://nc.shtwfgs.cn

echo "${#arr[@]}"
来源：http://yy.huanxung.cn

[R20] 关联数组（字典）
来源：http://ue.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ar.jctech888.com.cn

[R21] 字符串长度
来源：http://jp.szsharing.cn

echo "${#s}"
来源：http://au.newstarts.cn

[R22] 截取子串
来源：http://sw.nszjky.cn

echo "${s:0:5}"
来源：http://pb.lnxyls.cn

[R23] 字符串替换
来源：http://bn.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mu.muxihuayi.cn

[R24] 大小写转换
来源：http://vr.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jg.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://wk.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tc.jctech888.com.cn

[R26] 命令替换
来源：http://rp.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://pt.nszjky.cn

[R27] 算术展开
来源：http://wm.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://lr.521024.cn

[R28] 浮点运算
来源：http://in.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://tu.bjjhwx.cn

[R29] 定义函数
来源：http://in.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ow.shxzukj.cn

[R30] 函数返回状态码
来源：http://wd.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://cf.nicolike.cn

[R31] 局部变量
来源：http://ez.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://cl.panjiajie.cn

[R32] 参数个数校验
来源：http://et.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cs.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://cn.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yy.nszjky.cn

[R34] 退出时清理
来源：http://fp.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cc.shtwfgs.cn

[R35] 后台执行并等待
来源：http://rk.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tn.gzmigu.cn

[R36] 并发执行多个任务
来源：http://yl.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xa.nszjky.cn

[R37] 把输出赋给变量
来源：http://lz.lnxyls.cn

files=$(ls -1)
来源：http://wh.panjiajie.cn

[R38] 管道串联
来源：http://ba.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://vi.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://ra.jctech888.com.cn

cmd > out.log 2>&1
来源：http://ik.szxytkj.cn

[R40] 追加写日志
来源：http://oi.521024.cn

echo "log" >> out.log
来源：http://kd.lnxyls.cn

[R41] 丢弃输出
来源：http://uu.nicolike.cn

cmd >/dev/null 2>&1
来源：http://aw.chemitech.net.cn

[R42] 输入重定向
来源：http://qd.lnxyls.cn

wc -l < a.txt
来源：http://tc.huixiangedu.cn

[R43] 按名字查找文件
来源：http://vd.haigaiapp.cn

find . -name "*.log" -type f
来源：http://pa.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://qf.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://vr.bookmarksfly.cn

[R45] 批量删除
来源：http://it.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://tq.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://mq.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ez.newstarts.cn

[R47] sed 单行替换
来源：http://wq.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pa.colortex.cn

[R48] awk 取指定列
来源：http://ku.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://gh.yuexingan06.cn

[R49] awk 带条件
来源：http://xt.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lo.jctech888.com.cn

[R50] awk 求和
来源：http://en.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ci.lnxyls.cn

[R51] 排序去重取前几
来源：http://on.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gi.shxzskj.cn

[R52] 统计行数
来源：http://tm.gzmigu.cn

wc -l a.txt
来源：http://nb.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://ph.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zn.szsharing.cn

[R54] 比较两个文件
来源：http://il.shxzukj.cn

diff a.txt b.txt
来源：http://xp.hnjuh.cn

[R55] 压缩与解压
来源：http://hx.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sb.asd995.cn

[R56] 远程拷贝
来源：http://vl.szsharing.cn

scp file user@host:/path/
来源：http://oi.chemitech.net.cn

[R57] 远程执行命令
来源：http://fi.yuexingan06.cn

ssh user@host 'uptime'
来源：http://zq.lnxyls.cn

[R58] 下载文件
来源：http://qg.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nc.521024.cn

[R59] 发 POST JSON
来源：http://ml.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ie.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://eb.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rm.yuexingan06.cn

[R61] 磁盘占用
来源：http://kh.shxzskj.cn

df -h;  du -sh *
来源：http://zr.colortex.cn

[R62] 找最占空间的文件
来源：http://yo.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://rh.hahajie.cn

[R63] 内存与进程
来源：http://bq.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://rs.szxytkj.cn

[R64] 结束进程
来源：http://cl.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://lq.jctech888.com.cn

[R65] 查看端口占用
来源：http://av.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fi.521024.cn

[R66] 定时任务
来源：http://uf.panjiajie.cn

crontab -e;  crontab -l
来源：http://on.hahajie.cn

[R67] 生成随机十六进制串
来源：http://so.jctech888.com.cn

openssl rand -hex 16
来源：http://zz.hahajie.cn

[R68] 计算文件校验值
来源：http://br.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wl.bjjhwx.cn

[R69] 生成随机密码
来源：http://lr.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://pl.hnjuh.cn

[R70] 时间戳与互转
来源：http://wo.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://mn.9csxet.cn

[R71] 日期格式化
来源：http://su.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://na.shxzskj.cn

[R72] 等待端口就绪
来源：http://jh.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ea.colortex.cn

[R73] 分割大日志
来源：http://pf.muxihuayi.cn

split -l 1000 big.log part_
来源：http://sf.huixinmuqiang.cn

[R74] 批量重命名
来源：http://th.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ld.jctech888.com.cn

[R75] 导出环境变量
来源：http://xx.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://nc.9csxet.cn

[R76] 使用临时文件
来源：http://ac.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ja.szsharing.cn

[R77] 读取用户输入
来源：http://vh.nszjky.cn

read -rp "请输入: " ans
来源：http://pf.haigaiapp.cn

[R78] 交互式菜单
来源：http://sw.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://er.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://xk.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zl.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://fy.jctech888.com.cn

time ./run.sh
来源：http://vh.nszjky.cn

================================================================================
来源：http://uo.hahajie.cn

S. C / C++ 专题
来源：http://mt.muxihuayi.cn

================================================================================
来源：http://wr.huixinmuqiang.cn

[S01] C：Hello World
来源：http://nh.shxzukj.cn

#include <stdio.h>
来源：http://az.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xw.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://pd.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://eb.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ex.9csxet.cn

int x; scanf("%d", &x);
来源：http://xq.chemitech.net.cn

[S04] C：字符串复制
来源：http://tv.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://at.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://di.newstarts.cn

strlen(s)
来源：http://bw.yuexingan06.cn

[S06] C：字符串比较
来源：http://fj.bjjhwx.cn

strcmp(a, b) == 0
来源：http://jx.lnxyls.cn

[S07] C：数组遍历求和
来源：http://qu.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ry.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://ym.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ce.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://dp.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ps.hnjuh.cn

[S10] C：指针与解引用
来源：http://tk.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://ow.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://hh.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://la.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nq.szsharing.cn

fclose(f);
来源：http://ok.huixiangedu.cn

[S12] C：写文件
来源：http://de.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cw.huanxung.cn

[S13] C：宏定义
来源：http://ft.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ri.9csxet.cn

[S14] C：枚举
来源：http://rm.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://dp.jctech888.com.cn

[S15] C：类型转换
来源：http://pq.huanxung.cn

(double) a / b
来源：http://oj.bjjhwx.cn

[S16] C：位操作置位
来源：http://ki.chemitech.net.cn

x |= (1 << 3);
来源：http://ni.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://ha.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kd.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://iu.gzmigu.cn

int main(int argc, char **argv)
来源：http://dc.521024.cn

[S19] C：快速排序
来源：http://wd.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zs.jctech888.com.cn

[S20] C：二分查找
来源：http://sd.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gx.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://yf.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lw.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://jo.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cp.nszjky.cn

[S23] C：随机数
来源：http://nu.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qq.gzmigu.cn

[S24] C：获取本地时间
来源：http://qc.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cg.nicolike.cn

[S25] C：内存拷贝
来源：http://tj.huanxung.cn

memcpy(dst, src, n);
来源：http://mn.shxzukj.cn

[S26] C：内存清零
来源：http://fq.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://uc.shxzskj.cn

[S27] C：定义常量
来源：http://pf.nszjky.cn

const double PI = 3.14159;
来源：http://ke.newstarts.cn

[S28] C：静态变量
来源：http://xu.shtwfgs.cn

static int counter = 0;
来源：http://bo.shxzukj.cn

[S29] C：变参函数
来源：http://pk.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ws.hnjuh.cn

[S30] C：头文件保护
来源：http://ov.panjiajie.cn

#ifndef X_H
来源：http://ct.hahajie.cn

#define X_H
来源：http://hu.huanxung.cn

#endif
来源：http://zg.haigaiapp.cn

[S31] C++：Hello World
来源：http://pr.hnjuh.cn

#include <iostream>
来源：http://lb.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://jd.nicolike.cn

[S32] C++：字符串
来源：http://yp.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://mt.chemitech.net.cn

[S33] C++：vector 增删
来源：http://ns.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tu.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ie.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://gm.asd995.cn

[S35] C++：map
来源：http://xm.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ew.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://xp.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nk.haigaiapp.cn


<!-- 参考信息 -->