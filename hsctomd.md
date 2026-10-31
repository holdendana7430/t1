代发 wailian999

[Q63] 开启事务
来源：http://ox.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ew.lnxyls.cn

[Q64] 提交事务
来源：http://ta.lnxyls.cn

COMMIT;
来源：http://nh.wgjwhj.cn

[Q65] 回滚事务
来源：http://xp.wgjwhj.cn

ROLLBACK;
来源：http://es.521024.cn

[Q66] 行锁查询
来源：http://dp.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qr.newstarts.cn

[Q67] 设置隔离级别
来源：http://oy.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qp.shxzukj.cn

[Q68] 保存点
来源：http://hs.wgjwhj.cn

SAVEPOINT sp1;
来源：http://aa.lnxyls.cn

ROLLBACK TO sp1;
来源：http://qx.521024.cn

[Q69] 查看执行计划
来源：http://du.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kf.bjjhwx.cn

[Q70] 更新统计信息
来源：http://rc.bjjhwx.cn

ANALYZE TABLE users;
来源：http://ti.shxzskj.cn

[Q71] 查看建表语句
来源：http://yn.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ar.jctech888.com.cn

[Q72] 查看索引
来源：http://bh.521024.cn

SHOW INDEX FROM users;
来源：http://zt.wgjwhj.cn

[Q73] 查看表状态
来源：http://js.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qs.shxzskj.cn

[Q74] 强制使用索引
来源：http://ia.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zo.newstarts.cn

[Q75] 日期格式化
来源：http://nt.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://td.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vq.huixiangedu.cn

[Q76] 按天统计
来源：http://nr.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lv.asd995.cn

[Q77] 时间加减
来源：http://kr.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cq.hahajie.cn

[Q78] 当前时间
来源：http://gt.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rp.newstarts.cn

[Q79] 字符串拼接
来源：http://yf.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://em.colortex.cn

[Q80] 字符串截取
来源：http://it.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://in.shtwfgs.cn

[Q81] 字符串替换
来源：http://qj.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kh.521024.cn

[Q82] 字符长度与字节长度
来源：http://ys.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qs.wgjwhj.cn

[Q83] 大小写转换
来源：http://lj.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://km.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://cn.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://kn.newstarts.cn

[Q85] 数值取整
来源：http://rc.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ff.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://mo.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fp.hahajie.cn

[Q87] JSON 字段做条件
来源：http://wh.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://am.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://bl.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zq.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qo.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://kt.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yh.muxihuayi.cn

[Q90] 生成序号列
来源：http://uo.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xr.nszjky.cn

================================================================================
来源：http://hc.nicolike.cn

R. Bash 专题
来源：http://qg.gzmigu.cn

================================================================================
来源：http://fa.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://ls.huixiangedu.cn

#!/usr/bin/env bash
来源：http://az.muxihuayi.cn

set -euo pipefail
来源：http://np.shxzukj.cn

[R02] 变量赋值与使用
来源：http://ot.shxzskj.cn

name="Tom"; echo "$name"
来源：http://rz.colortex.cn

[R03] 只读变量
来源：http://xb.szsharing.cn

readonly PI=3.14
来源：http://sw.haigaiapp.cn

[R04] 位置参数
来源：http://lq.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rh.huanxung.cn

[R05] 参数默认值
来源：http://yc.hnjuh.cn

name="${1:-default}"
来源：http://ar.shxzskj.cn

[R06] 判断命令是否存在
来源：http://ny.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://df.muxihuayi.cn

[R07] if 判断文件
来源：http://bw.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oo.lnxyls.cn

[R08] 数值比较
来源：http://dq.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qn.jctech888.com.cn

[R09] 字符串比较
来源：http://cm.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bk.haigaiapp.cn

[R10] 正则匹配
来源：http://rn.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kx.muxihuayi.cn

[R11] case 多分支
来源：http://ud.huixinmuqiang.cn

case "$1" in
来源：http://aw.muxihuayi.cn

start) echo "启动" ;;
来源：http://pb.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://dg.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://mq.hahajie.cn

esac
来源：http://or.szxytkj.cn

[R12] for 遍历文件
来源：http://sv.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://ft.jianghongdianzi.cn

[R13] for 计数循环
来源：http://fo.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://la.521024.cn

[R14] C 风格 for
来源：http://fx.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qa.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://fc.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zw.huixiangedu.cn

[R16] until 等待条件
来源：http://hd.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ky.huanxung.cn

[R17] 数组定义与取值
来源：http://xu.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zs.hnjuh.cn

[R18] 遍历数组
来源：http://gy.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fu.huixinmuqiang.cn

[R19] 数组长度
来源：http://ie.asd995.cn

echo "${#arr[@]}"
来源：http://cg.huanxung.cn

[R20] 关联数组（字典）
来源：http://fk.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yl.hahajie.cn

[R21] 字符串长度
来源：http://bz.shtwfgs.cn

echo "${#s}"
来源：http://jv.colortex.cn

[R22] 截取子串
来源：http://vq.gzmigu.cn

echo "${s:0:5}"
来源：http://ac.521024.cn

[R23] 字符串替换
来源：http://zr.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fk.jianghongdianzi.cn

[R24] 大小写转换
来源：http://bw.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oa.521024.cn

[R25] 去后缀 / 去前缀
来源：http://fy.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vh.huixiangedu.cn

[R26] 命令替换
来源：http://ry.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://zg.yuntaijiaju.cn

[R27] 算术展开
来源：http://xx.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://ch.szsharing.cn

[R28] 浮点运算
来源：http://cb.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://vr.jctech888.com.cn

[R29] 定义函数
来源：http://rn.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ut.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://ts.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://qw.9csxet.cn

[R31] 局部变量
来源：http://sz.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://my.nszjky.cn

[R32] 参数个数校验
来源：http://na.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rd.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://hg.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yt.panjiajie.cn

[R34] 退出时清理
来源：http://fe.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wl.haigaiapp.cn

[R35] 后台执行并等待
来源：http://xw.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lu.hahajie.cn

[R36] 并发执行多个任务
来源：http://rz.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cv.9csxet.cn

[R37] 把输出赋给变量
来源：http://jl.szxytkj.cn

files=$(ls -1)
来源：http://oj.chemitech.net.cn

[R38] 管道串联
来源：http://ah.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://is.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://rj.muxihuayi.cn

cmd > out.log 2>&1
来源：http://kp.nszjky.cn

[R40] 追加写日志
来源：http://pa.huixinmuqiang.cn

echo "log" >> out.log
来源：http://vh.huixiangedu.cn

[R41] 丢弃输出
来源：http://dn.9csxet.cn

cmd >/dev/null 2>&1
来源：http://zf.shtwfgs.cn

[R42] 输入重定向
来源：http://lf.nicolike.cn

wc -l < a.txt
来源：http://iw.shxzukj.cn

[R43] 按名字查找文件
来源：http://xx.gzmigu.cn

find . -name "*.log" -type f
来源：http://wc.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://qa.521024.cn

find . -mtime -7 -type f
来源：http://jy.521024.cn

[R45] 批量删除
来源：http://xw.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://fm.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://ii.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ws.colortex.cn

[R47] sed 单行替换
来源：http://hs.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ck.521024.cn

[R48] awk 取指定列
来源：http://pr.521024.cn

awk '{print $1, $3}' a.txt
来源：http://wl.huixinmuqiang.cn

[R49] awk 带条件
来源：http://mh.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jr.yuntaijiaju.cn

[R50] awk 求和
来源：http://sy.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lj.9csxet.cn

[R51] 排序去重取前几
来源：http://cx.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zq.huixinmuqiang.cn

[R52] 统计行数
来源：http://ew.huanxung.cn

wc -l a.txt
来源：http://yr.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://cb.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nj.haigaiapp.cn

[R54] 比较两个文件
来源：http://aw.hahajie.cn

diff a.txt b.txt
来源：http://qc.szsharing.cn

[R55] 压缩与解压
来源：http://yz.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mb.bookmarksfly.cn

[R56] 远程拷贝
来源：http://vj.szsharing.cn

scp file user@host:/path/
来源：http://xh.bjjhwx.cn

[R57] 远程执行命令
来源：http://ax.newstarts.cn

ssh user@host 'uptime'
来源：http://hu.nszjky.cn

[R58] 下载文件
来源：http://do.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hs.gzmigu.cn

[R59] 发 POST JSON
来源：http://se.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://su.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://ui.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lj.muxihuayi.cn

[R61] 磁盘占用
来源：http://np.jianghongdianzi.cn

df -h;  du -sh *
来源：http://kl.szxytkj.cn

[R62] 找最占空间的文件
来源：http://fi.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://ny.shxzukj.cn

[R63] 内存与进程
来源：http://pr.521024.cn

free -h;  ps aux | grep nginx
来源：http://zb.shxzskj.cn

[R64] 结束进程
来源：http://el.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://sl.panjiajie.cn

[R65] 查看端口占用
来源：http://vh.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eg.hnjuh.cn

[R66] 定时任务
来源：http://ev.shxzukj.cn

crontab -e;  crontab -l
来源：http://jy.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://hz.chemitech.net.cn

openssl rand -hex 16
来源：http://lx.szsharing.cn

[R68] 计算文件校验值
来源：http://ft.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yq.hnjuh.cn

[R69] 生成随机密码
来源：http://cx.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://he.wgjwhj.cn

[R70] 时间戳与互转
来源：http://fe.nicolike.cn

date +%s;  date -d @1700000000
来源：http://br.jianghongdianzi.cn

[R71] 日期格式化
来源：http://rg.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ya.shxzskj.cn

[R72] 等待端口就绪
来源：http://zb.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://do.colortex.cn

[R73] 分割大日志
来源：http://cv.szsharing.cn

split -l 1000 big.log part_
来源：http://fr.shxzukj.cn

[R74] 批量重命名
来源：http://nv.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yd.jctech888.com.cn

[R75] 导出环境变量
来源：http://wg.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://fp.haigaiapp.cn

[R76] 使用临时文件
来源：http://hs.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kv.shxzukj.cn

[R77] 读取用户输入
来源：http://or.colortex.cn

read -rp "请输入: " ans
来源：http://sz.huixiangedu.cn

[R78] 交互式菜单
来源：http://vi.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uh.newstarts.cn

[R79] 解析命令行选项
来源：http://ng.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pk.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://fd.muxihuayi.cn

time ./run.sh
来源：http://cu.szsharing.cn

================================================================================
来源：http://ja.hahajie.cn

S. C / C++ 专题
来源：http://fy.jctech888.com.cn

================================================================================
来源：http://nc.huanxung.cn

[S01] C：Hello World
来源：http://vy.bjjhwx.cn

#include <stdio.h>
来源：http://ji.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oe.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://qy.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://al.huixinmuqiang.cn

[S03] C：读入整数
来源：http://ix.9csxet.cn

int x; scanf("%d", &x);
来源：http://sa.9csxet.cn

[S04] C：字符串复制
来源：http://yr.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ly.muxihuayi.cn

[S05] C：字符串长度
来源：http://eu.bookmarksfly.cn

strlen(s)
来源：http://ek.huanxung.cn

[S06] C：字符串比较
来源：http://my.asd995.cn

strcmp(a, b) == 0
来源：http://kx.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://fs.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ee.colortex.cn

[S08] C：动态内存分配与释放
来源：http://lc.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ui.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://qc.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rh.nszjky.cn

[S10] C：指针与解引用
来源：http://od.szsharing.cn

int *p = &a;  *p = 5;
来源：http://lb.colortex.cn

[S11] C：逐行读文件
来源：http://cg.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://dx.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lt.nicolike.cn

fclose(f);
来源：http://eg.gzmigu.cn

[S12] C：写文件
来源：http://bc.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fp.nicolike.cn

[S13] C：宏定义
来源：http://ry.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rk.bookmarksfly.cn

[S14] C：枚举
来源：http://zd.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://zv.asd995.cn

[S15] C：类型转换
来源：http://jj.yuntaijiaju.cn

(double) a / b
来源：http://vp.bookmarksfly.cn

[S16] C：位操作置位
来源：http://fl.asd995.cn

x |= (1 << 3);
来源：http://ow.nicolike.cn

[S17] C：安全拼接字符串
来源：http://cj.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oi.lnxyls.cn

[S18] C：命令行参数
来源：http://tc.bjjhwx.cn

int main(int argc, char **argv)
来源：http://gg.haigaiapp.cn

[S19] C：快速排序
来源：http://hs.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://za.jctech888.com.cn

[S20] C：二分查找
来源：http://ru.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nc.muxihuayi.cn

[S21] C：字符类别判断
来源：http://rr.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gt.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://st.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fv.hahajie.cn

[S23] C：随机数
来源：http://qy.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xh.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://bu.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wx.hahajie.cn

[S25] C：内存拷贝
来源：http://ef.asd995.cn

memcpy(dst, src, n);
来源：http://gq.wgjwhj.cn

[S26] C：内存清零
来源：http://nf.nszjky.cn

memset(a, 0, sizeof a);
来源：http://oz.jctech888.com.cn

[S27] C：定义常量
来源：http://wo.shtwfgs.cn

const double PI = 3.14159;
来源：http://fi.shxzskj.cn

[S28] C：静态变量
来源：http://zw.jianghongdianzi.cn

static int counter = 0;
来源：http://tk.gzmigu.cn

[S29] C：变参函数
来源：http://dx.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cy.gzmigu.cn

[S30] C：头文件保护
来源：http://yj.huixinmuqiang.cn

#ifndef X_H
来源：http://js.huixinmuqiang.cn

#define X_H
来源：http://cn.shxzukj.cn

#endif
来源：http://vi.muxihuayi.cn

[S31] C++：Hello World
来源：http://ot.lnxyls.cn

#include <iostream>
来源：http://jp.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://kj.chemitech.net.cn

[S32] C++：字符串
来源：http://cm.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://se.shtwfgs.cn


<!-- 参考信息 -->