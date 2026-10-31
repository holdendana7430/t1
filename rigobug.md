代发 wailian999

[Q65] 回滚事务
来源：http://ee.szsharing.cn

ROLLBACK;
来源：http://qw.hahajie.cn

[Q66] 行锁查询
来源：http://cb.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ps.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://tz.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vx.wgjwhj.cn

[Q68] 保存点
来源：http://sr.hahajie.cn

SAVEPOINT sp1;
来源：http://ga.521024.cn

ROLLBACK TO sp1;
来源：http://fw.hnjuh.cn

[Q69] 查看执行计划
来源：http://dr.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gc.521024.cn

[Q70] 更新统计信息
来源：http://xx.muxihuayi.cn

ANALYZE TABLE users;
来源：http://nd.yuexingan06.cn

[Q71] 查看建表语句
来源：http://ac.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mg.yuexingan06.cn

[Q72] 查看索引
来源：http://op.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://sd.shxzukj.cn

[Q73] 查看表状态
来源：http://kc.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bs.yuexingan06.cn

[Q74] 强制使用索引
来源：http://au.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://df.yuexingan06.cn

[Q75] 日期格式化
来源：http://xb.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yu.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ya.haigaiapp.cn

[Q76] 按天统计
来源：http://es.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lz.szxytkj.cn

[Q77] 时间加减
来源：http://at.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://au.jianghongdianzi.cn

[Q78] 当前时间
来源：http://nn.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wz.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://fe.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jk.shxzskj.cn

[Q80] 字符串截取
来源：http://ju.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uc.nicolike.cn

[Q81] 字符串替换
来源：http://tl.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mz.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://tq.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ti.panjiajie.cn

[Q83] 大小写转换
来源：http://oc.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vk.szxytkj.cn

[Q84] 去除首尾空格
来源：http://yc.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://on.521024.cn

[Q85] 数值取整
来源：http://ue.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jp.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://wa.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zu.asd995.cn

[Q87] JSON 字段做条件
来源：http://xg.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jv.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://gt.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gm.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qf.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://bs.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wr.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://ex.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://al.szsharing.cn

================================================================================
来源：http://hd.huanxung.cn

R. Bash 专题
来源：http://tn.yuntaijiaju.cn

================================================================================
来源：http://gn.nicolike.cn

[R01] shebang 与严格模式
来源：http://cy.wgjwhj.cn

#!/usr/bin/env bash
来源：http://dw.asd995.cn

set -euo pipefail
来源：http://kj.hnjuh.cn

[R02] 变量赋值与使用
来源：http://am.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://pl.asd995.cn

[R03] 只读变量
来源：http://xt.muxihuayi.cn

readonly PI=3.14
来源：http://tz.szsharing.cn

[R04] 位置参数
来源：http://sd.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://se.nszjky.cn

[R05] 参数默认值
来源：http://jz.jianghongdianzi.cn

name="${1:-default}"
来源：http://it.panjiajie.cn

[R06] 判断命令是否存在
来源：http://xs.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tf.9csxet.cn

[R07] if 判断文件
来源：http://ht.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vv.asd995.cn

[R08] 数值比较
来源：http://jn.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://va.asd995.cn

[R09] 字符串比较
来源：http://ir.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wm.lnxyls.cn

[R10] 正则匹配
来源：http://mc.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hb.9csxet.cn

[R11] case 多分支
来源：http://ms.bjjhwx.cn

case "$1" in
来源：http://wt.huixiangedu.cn

start) echo "启动" ;;
来源：http://zt.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://jr.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://ik.shtwfgs.cn

esac
来源：http://sx.panjiajie.cn

[R12] for 遍历文件
来源：http://kq.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://em.asd995.cn

[R13] for 计数循环
来源：http://ih.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://nl.hahajie.cn

[R14] C 风格 for
来源：http://uk.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://va.nszjky.cn

[R15] while 逐行读文件
来源：http://tl.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://as.muxihuayi.cn

[R16] until 等待条件
来源：http://os.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dl.lnxyls.cn

[R17] 数组定义与取值
来源：http://uc.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hr.shtwfgs.cn

[R18] 遍历数组
来源：http://as.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rf.szxytkj.cn

[R19] 数组长度
来源：http://ys.shtwfgs.cn

echo "${#arr[@]}"
来源：http://ln.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://gi.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tq.bookmarksfly.cn

[R21] 字符串长度
来源：http://jq.gzmigu.cn

echo "${#s}"
来源：http://ho.hahajie.cn

[R22] 截取子串
来源：http://eg.bookmarksfly.cn

echo "${s:0:5}"
来源：http://hn.shtwfgs.cn

[R23] 字符串替换
来源：http://fi.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uz.hnjuh.cn

[R24] 大小写转换
来源：http://dp.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ou.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://ie.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://op.huixinmuqiang.cn

[R26] 命令替换
来源：http://md.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://ik.gzmigu.cn

[R27] 算术展开
来源：http://pu.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://ig.9csxet.cn

[R28] 浮点运算
来源：http://pd.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://uf.yuntaijiaju.cn

[R29] 定义函数
来源：http://cj.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ua.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://pk.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://hj.asd995.cn

[R31] 局部变量
来源：http://eh.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://ef.colortex.cn

[R32] 参数个数校验
来源：http://hg.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qo.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://nv.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wl.521024.cn

[R34] 退出时清理
来源：http://nj.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vq.huanxung.cn

[R35] 后台执行并等待
来源：http://ii.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rq.lnxyls.cn

[R36] 并发执行多个任务
来源：http://mk.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gw.szsharing.cn

[R37] 把输出赋给变量
来源：http://ve.szsharing.cn

files=$(ls -1)
来源：http://ll.hnjuh.cn

[R38] 管道串联
来源：http://wc.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://ln.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://zg.szxytkj.cn

cmd > out.log 2>&1
来源：http://hw.huanxung.cn

[R40] 追加写日志
来源：http://cg.colortex.cn

echo "log" >> out.log
来源：http://vf.yuexingan06.cn

[R41] 丢弃输出
来源：http://tx.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://yb.chemitech.net.cn

[R42] 输入重定向
来源：http://yl.521024.cn

wc -l < a.txt
来源：http://uy.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://xn.jctech888.com.cn

find . -name "*.log" -type f
来源：http://dk.huixiangedu.cn

[R44] 按修改时间查找
来源：http://qg.panjiajie.cn

find . -mtime -7 -type f
来源：http://pp.szsharing.cn

[R45] 批量删除
来源：http://ln.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://or.colortex.cn

[R46] 递归替换文件内容
来源：http://oy.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ea.colortex.cn

[R47] sed 单行替换
来源：http://md.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://as.bjjhwx.cn

[R48] awk 取指定列
来源：http://qy.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://fz.panjiajie.cn

[R49] awk 带条件
来源：http://sm.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lv.jctech888.com.cn

[R50] awk 求和
来源：http://ab.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wi.szsharing.cn

[R51] 排序去重取前几
来源：http://jg.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wl.jctech888.com.cn

[R52] 统计行数
来源：http://fe.colortex.cn

wc -l a.txt
来源：http://rd.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://kx.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oo.bjjhwx.cn

[R54] 比较两个文件
来源：http://ys.colortex.cn

diff a.txt b.txt
来源：http://qf.huanxung.cn

[R55] 压缩与解压
来源：http://rv.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gz.nszjky.cn

[R56] 远程拷贝
来源：http://fh.521024.cn

scp file user@host:/path/
来源：http://sv.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://rx.chemitech.net.cn

ssh user@host 'uptime'
来源：http://mz.bjjhwx.cn

[R58] 下载文件
来源：http://xr.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ep.hahajie.cn

[R59] 发 POST JSON
来源：http://hx.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fx.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://vj.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xi.shxzskj.cn

[R61] 磁盘占用
来源：http://zh.hnjuh.cn

df -h;  du -sh *
来源：http://ox.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://mn.521024.cn

du -ah . | sort -rh | head -10
来源：http://ma.newstarts.cn

[R63] 内存与进程
来源：http://vx.colortex.cn

free -h;  ps aux | grep nginx
来源：http://pq.9csxet.cn

[R64] 结束进程
来源：http://mp.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://dx.newstarts.cn

[R65] 查看端口占用
来源：http://ov.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fs.newstarts.cn

[R66] 定时任务
来源：http://vk.chemitech.net.cn

crontab -e;  crontab -l
来源：http://cz.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://mj.nszjky.cn

openssl rand -hex 16
来源：http://fw.szsharing.cn

[R68] 计算文件校验值
来源：http://uv.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://km.wgjwhj.cn

[R69] 生成随机密码
来源：http://cr.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://my.shtwfgs.cn

[R70] 时间戳与互转
来源：http://oe.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://ce.muxihuayi.cn

[R71] 日期格式化
来源：http://id.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nf.huanxung.cn

[R72] 等待端口就绪
来源：http://lj.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eh.wgjwhj.cn

[R73] 分割大日志
来源：http://kl.9csxet.cn

split -l 1000 big.log part_
来源：http://it.asd995.cn

[R74] 批量重命名
来源：http://qc.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sf.521024.cn

[R75] 导出环境变量
来源：http://bg.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://bh.nszjky.cn

[R76] 使用临时文件
来源：http://nu.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://do.szxytkj.cn

[R77] 读取用户输入
来源：http://hv.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://dj.jctech888.com.cn

[R78] 交互式菜单
来源：http://vw.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rj.521024.cn

[R79] 解析命令行选项
来源：http://es.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tz.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://uz.yuntaijiaju.cn

time ./run.sh
来源：http://cb.szsharing.cn

================================================================================
来源：http://xf.wgjwhj.cn

S. C / C++ 专题
来源：http://oq.asd995.cn

================================================================================
来源：http://ec.szxytkj.cn

[S01] C：Hello World
来源：http://sn.haigaiapp.cn

#include <stdio.h>
来源：http://py.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tn.nszjky.cn

[S02] C：变量与格式化输出
来源：http://ho.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://tb.huanxung.cn

[S03] C：读入整数
来源：http://yw.asd995.cn

int x; scanf("%d", &x);
来源：http://dz.521024.cn

[S04] C：字符串复制
来源：http://kj.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://le.yuexingan06.cn

[S05] C：字符串长度
来源：http://xv.bookmarksfly.cn

strlen(s)
来源：http://lg.9csxet.cn

[S06] C：字符串比较
来源：http://oz.521024.cn

strcmp(a, b) == 0
来源：http://ua.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://hh.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ti.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://st.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://px.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://uy.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://st.chemitech.net.cn

[S10] C：指针与解引用
来源：http://gt.nicolike.cn

int *p = &a;  *p = 5;
来源：http://ig.szsharing.cn

[S11] C：逐行读文件
来源：http://lx.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://on.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dq.huixiangedu.cn

fclose(f);
来源：http://ni.521024.cn

[S12] C：写文件
来源：http://dc.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wn.huanxung.cn

[S13] C：宏定义
来源：http://cm.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xq.9csxet.cn

[S14] C：枚举
来源：http://df.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://le.jctech888.com.cn

[S15] C：类型转换
来源：http://kn.huixinmuqiang.cn

(double) a / b
来源：http://he.521024.cn

[S16] C：位操作置位
来源：http://qt.muxihuayi.cn

x |= (1 << 3);
来源：http://ad.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://wo.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qf.panjiajie.cn

[S18] C：命令行参数
来源：http://zg.shxzukj.cn

int main(int argc, char **argv)
来源：http://is.huanxung.cn

[S19] C：快速排序
来源：http://pq.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hm.shtwfgs.cn

[S20] C：二分查找
来源：http://vd.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cd.bjjhwx.cn

[S21] C：字符类别判断
来源：http://aa.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ub.9csxet.cn

[S22] C：字符串转数字
来源：http://xi.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gf.wgjwhj.cn

[S23] C：随机数
来源：http://oj.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jp.haigaiapp.cn

[S24] C：获取本地时间
来源：http://ua.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eb.gzmigu.cn

[S25] C：内存拷贝
来源：http://rk.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://sf.colortex.cn

[S26] C：内存清零
来源：http://fz.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://te.shxzskj.cn

[S27] C：定义常量
来源：http://gn.hahajie.cn

const double PI = 3.14159;
来源：http://tz.muxihuayi.cn

[S28] C：静态变量
来源：http://ku.wgjwhj.cn

static int counter = 0;
来源：http://is.9csxet.cn

[S29] C：变参函数
来源：http://yz.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ak.colortex.cn

[S30] C：头文件保护
来源：http://hp.yuntaijiaju.cn

#ifndef X_H
来源：http://pj.521024.cn

#define X_H
来源：http://km.jctech888.com.cn

#endif
来源：http://fg.colortex.cn

[S31] C++：Hello World
来源：http://oe.nicolike.cn

#include <iostream>
来源：http://dn.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://hs.haigaiapp.cn

[S32] C++：字符串
来源：http://am.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://lz.asd995.cn

[S33] C++：vector 增删
来源：http://lm.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ce.lnxyls.cn

[S34] C++：遍历 vector
来源：http://gc.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://yp.bookmarksfly.cn


<!-- 参考信息 -->