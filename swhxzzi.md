代发 wailian999

[Q63] 开启事务
来源：http://qs.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nr.yuexingan06.cn

[Q64] 提交事务
来源：http://zo.asd995.cn

COMMIT;
来源：http://dp.shxzskj.cn

[Q65] 回滚事务
来源：http://wd.nicolike.cn

ROLLBACK;
来源：http://ic.521024.cn

[Q66] 行锁查询
来源：http://uq.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ci.gzmigu.cn

[Q67] 设置隔离级别
来源：http://ly.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ti.9csxet.cn

[Q68] 保存点
来源：http://vm.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://sd.shxzukj.cn

ROLLBACK TO sp1;
来源：http://db.9csxet.cn

[Q69] 查看执行计划
来源：http://co.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ph.asd995.cn

[Q70] 更新统计信息
来源：http://wj.chemitech.net.cn

ANALYZE TABLE users;
来源：http://dv.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://wd.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cx.szxytkj.cn

[Q72] 查看索引
来源：http://qy.colortex.cn

SHOW INDEX FROM users;
来源：http://gh.hahajie.cn

[Q73] 查看表状态
来源：http://ad.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hs.521024.cn

[Q74] 强制使用索引
来源：http://oq.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gk.chemitech.net.cn

[Q75] 日期格式化
来源：http://yo.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cd.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jb.shtwfgs.cn

[Q76] 按天统计
来源：http://wl.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oi.9csxet.cn

[Q77] 时间加减
来源：http://ei.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nu.haigaiapp.cn

[Q78] 当前时间
来源：http://cv.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://if.colortex.cn

[Q79] 字符串拼接
来源：http://kk.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pm.hahajie.cn

[Q80] 字符串截取
来源：http://fc.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iw.9csxet.cn

[Q81] 字符串替换
来源：http://lw.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sd.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://kv.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ri.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://ff.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iu.szxytkj.cn

[Q84] 去除首尾空格
来源：http://vf.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://jy.panjiajie.cn

[Q85] 数值取整
来源：http://ms.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fh.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://vu.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gh.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://ya.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tc.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://uh.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pl.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ph.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://im.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qr.hahajie.cn

[Q90] 生成序号列
来源：http://wm.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ny.wgjwhj.cn

================================================================================
来源：http://yg.bookmarksfly.cn

R. Bash 专题
来源：http://yy.newstarts.cn

================================================================================
来源：http://qa.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://yu.shtwfgs.cn

#!/usr/bin/env bash
来源：http://qw.521024.cn

set -euo pipefail
来源：http://uz.gzmigu.cn

[R02] 变量赋值与使用
来源：http://bq.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://lz.shxzukj.cn

[R03] 只读变量
来源：http://fg.huixiangedu.cn

readonly PI=3.14
来源：http://ok.lnxyls.cn

[R04] 位置参数
来源：http://lc.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fl.szxytkj.cn

[R05] 参数默认值
来源：http://gi.yuntaijiaju.cn

name="${1:-default}"
来源：http://ns.newstarts.cn

[R06] 判断命令是否存在
来源：http://la.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jn.panjiajie.cn

[R07] if 判断文件
来源：http://cn.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://np.gzmigu.cn

[R08] 数值比较
来源：http://aw.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cz.lnxyls.cn

[R09] 字符串比较
来源：http://ff.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ro.yuntaijiaju.cn

[R10] 正则匹配
来源：http://ve.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pe.hahajie.cn

[R11] case 多分支
来源：http://qi.yuntaijiaju.cn

case "$1" in
来源：http://ad.shxzskj.cn

start) echo "启动" ;;
来源：http://bi.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://yg.asd995.cn

*)     echo "未知命令" ;;
来源：http://xv.nicolike.cn

esac
来源：http://tp.huixiangedu.cn

[R12] for 遍历文件
来源：http://kk.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://dh.bjjhwx.cn

[R13] for 计数循环
来源：http://eo.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ud.colortex.cn

[R14] C 风格 for
来源：http://dg.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fc.nicolike.cn

[R15] while 逐行读文件
来源：http://ns.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pz.gzmigu.cn

[R16] until 等待条件
来源：http://se.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wq.szxytkj.cn

[R17] 数组定义与取值
来源：http://om.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bg.nicolike.cn

[R18] 遍历数组
来源：http://uf.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cm.jianghongdianzi.cn

[R19] 数组长度
来源：http://pg.szsharing.cn

echo "${#arr[@]}"
来源：http://om.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://kg.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tm.bjjhwx.cn

[R21] 字符串长度
来源：http://lu.szsharing.cn

echo "${#s}"
来源：http://on.huixinmuqiang.cn

[R22] 截取子串
来源：http://jc.newstarts.cn

echo "${s:0:5}"
来源：http://le.panjiajie.cn

[R23] 字符串替换
来源：http://jf.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eq.shxzukj.cn

[R24] 大小写转换
来源：http://yn.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bl.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://sd.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zf.shxzskj.cn

[R26] 命令替换
来源：http://gw.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://dl.jctech888.com.cn

[R27] 算术展开
来源：http://wh.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://xb.yuexingan06.cn

[R28] 浮点运算
来源：http://rt.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://qg.huixiangedu.cn

[R29] 定义函数
来源：http://zk.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hj.shxzukj.cn

[R30] 函数返回状态码
来源：http://ga.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://ur.colortex.cn

[R31] 局部变量
来源：http://so.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://cs.szsharing.cn

[R32] 参数个数校验
来源：http://xm.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iy.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://ag.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fn.521024.cn

[R34] 退出时清理
来源：http://bv.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hj.chemitech.net.cn

[R35] 后台执行并等待
来源：http://sh.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oc.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://bm.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://df.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://vz.bookmarksfly.cn

files=$(ls -1)
来源：http://ez.asd995.cn

[R38] 管道串联
来源：http://ge.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://le.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://xj.asd995.cn

cmd > out.log 2>&1
来源：http://zz.9csxet.cn

[R40] 追加写日志
来源：http://lx.shxzukj.cn

echo "log" >> out.log
来源：http://uf.panjiajie.cn

[R41] 丢弃输出
来源：http://qf.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://wv.yuexingan06.cn

[R42] 输入重定向
来源：http://fd.huixiangedu.cn

wc -l < a.txt
来源：http://fi.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://oe.yuexingan06.cn

find . -name "*.log" -type f
来源：http://sx.panjiajie.cn

[R44] 按修改时间查找
来源：http://xb.lnxyls.cn

find . -mtime -7 -type f
来源：http://nb.haigaiapp.cn

[R45] 批量删除
来源：http://hl.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://fj.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://th.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mu.huanxung.cn

[R47] sed 单行替换
来源：http://cg.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hb.haigaiapp.cn

[R48] awk 取指定列
来源：http://ni.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://rb.nszjky.cn

[R49] awk 带条件
来源：http://aq.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zu.panjiajie.cn

[R50] awk 求和
来源：http://lf.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pe.bjjhwx.cn

[R51] 排序去重取前几
来源：http://iu.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gq.asd995.cn

[R52] 统计行数
来源：http://uk.jianghongdianzi.cn

wc -l a.txt
来源：http://up.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://pa.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://by.huixiangedu.cn

[R54] 比较两个文件
来源：http://qn.521024.cn

diff a.txt b.txt
来源：http://rk.newstarts.cn

[R55] 压缩与解压
来源：http://zu.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rj.shxzukj.cn

[R56] 远程拷贝
来源：http://qv.panjiajie.cn

scp file user@host:/path/
来源：http://hb.gzmigu.cn

[R57] 远程执行命令
来源：http://si.bjjhwx.cn

ssh user@host 'uptime'
来源：http://hp.szxytkj.cn

[R58] 下载文件
来源：http://gh.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gb.9csxet.cn

[R59] 发 POST JSON
来源：http://ya.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ga.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://ug.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://if.lnxyls.cn

[R61] 磁盘占用
来源：http://lg.nicolike.cn

df -h;  du -sh *
来源：http://uv.szsharing.cn

[R62] 找最占空间的文件
来源：http://qj.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://gv.nicolike.cn

[R63] 内存与进程
来源：http://nk.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://fu.9csxet.cn

[R64] 结束进程
来源：http://di.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://fl.huixiangedu.cn

[R65] 查看端口占用
来源：http://ex.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://od.9csxet.cn

[R66] 定时任务
来源：http://nv.panjiajie.cn

crontab -e;  crontab -l
来源：http://xk.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://ck.521024.cn

openssl rand -hex 16
来源：http://oy.gzmigu.cn

[R68] 计算文件校验值
来源：http://be.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kr.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://tg.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://of.szsharing.cn

[R70] 时间戳与互转
来源：http://sc.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://ks.newstarts.cn

[R71] 日期格式化
来源：http://cb.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gi.newstarts.cn

[R72] 等待端口就绪
来源：http://dw.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rh.shtwfgs.cn

[R73] 分割大日志
来源：http://ki.muxihuayi.cn

split -l 1000 big.log part_
来源：http://fu.jianghongdianzi.cn

[R74] 批量重命名
来源：http://db.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ad.shxzskj.cn

[R75] 导出环境变量
来源：http://zc.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://jz.muxihuayi.cn

[R76] 使用临时文件
来源：http://lo.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yh.shtwfgs.cn

[R77] 读取用户输入
来源：http://fb.lnxyls.cn

read -rp "请输入: " ans
来源：http://ox.bookmarksfly.cn

[R78] 交互式菜单
来源：http://wb.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fg.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://wc.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fb.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://iv.asd995.cn

time ./run.sh
来源：http://nm.szxytkj.cn

================================================================================
来源：http://af.yuntaijiaju.cn

S. C / C++ 专题
来源：http://by.newstarts.cn

================================================================================
来源：http://pw.yuntaijiaju.cn

[S01] C：Hello World
来源：http://sf.9csxet.cn

#include <stdio.h>
来源：http://bg.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nk.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://ug.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://nw.szxytkj.cn

[S03] C：读入整数
来源：http://ou.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://xg.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://je.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qk.nszjky.cn

[S05] C：字符串长度
来源：http://wn.gzmigu.cn

strlen(s)
来源：http://tc.szsharing.cn

[S06] C：字符串比较
来源：http://am.shtwfgs.cn

strcmp(a, b) == 0
来源：http://ki.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://sy.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qj.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://gk.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uq.521024.cn

[S09] C：结构体定义与初始化
来源：http://cr.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rp.huanxung.cn

[S10] C：指针与解引用
来源：http://mg.9csxet.cn

int *p = &a;  *p = 5;
来源：http://gv.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://ly.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://bj.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yu.hnjuh.cn

fclose(f);
来源：http://ay.nicolike.cn

[S12] C：写文件
来源：http://uu.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vk.jctech888.com.cn

[S13] C：宏定义
来源：http://pv.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://am.hahajie.cn

[S14] C：枚举
来源：http://tg.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://wv.nicolike.cn

[S15] C：类型转换
来源：http://jg.wgjwhj.cn

(double) a / b
来源：http://mr.colortex.cn

[S16] C：位操作置位
来源：http://pd.muxihuayi.cn

x |= (1 << 3);
来源：http://bw.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://nn.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://um.huanxung.cn

[S18] C：命令行参数
来源：http://ie.panjiajie.cn

int main(int argc, char **argv)
来源：http://ca.jctech888.com.cn

[S19] C：快速排序
来源：http://ge.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ne.asd995.cn

[S20] C：二分查找
来源：http://ql.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xq.muxihuayi.cn

[S21] C：字符类别判断
来源：http://rr.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ok.hnjuh.cn

[S22] C：字符串转数字
来源：http://za.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vd.nicolike.cn

[S23] C：随机数
来源：http://nr.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://am.521024.cn

[S24] C：获取本地时间
来源：http://mk.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://es.szsharing.cn

[S25] C：内存拷贝
来源：http://in.yuexingan06.cn

memcpy(dst, src, n);
来源：http://wr.yuntaijiaju.cn

[S26] C：内存清零
来源：http://wc.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://oy.haigaiapp.cn

[S27] C：定义常量
来源：http://pj.szsharing.cn

const double PI = 3.14159;
来源：http://em.shxzskj.cn

[S28] C：静态变量
来源：http://iy.yuexingan06.cn

static int counter = 0;
来源：http://qn.huixiangedu.cn

[S29] C：变参函数
来源：http://tx.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mm.bookmarksfly.cn

[S30] C：头文件保护
来源：http://do.jctech888.com.cn

#ifndef X_H
来源：http://ji.colortex.cn

#define X_H
来源：http://on.szxytkj.cn

#endif
来源：http://hm.wgjwhj.cn

[S31] C++：Hello World
来源：http://bb.yuexingan06.cn

#include <iostream>
来源：http://cr.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://yc.shxzukj.cn

[S32] C++：字符串
来源：http://ya.asd995.cn

std::string s = "hi";  s += "!";
来源：http://wk.huanxung.cn


<!-- 参考信息 -->