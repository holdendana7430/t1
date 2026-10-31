代发 wailian999

[Q61] 移动平均
来源：http://dy.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vk.panjiajie.cn

[Q62] 分组占比
来源：http://ie.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dt.521024.cn

[Q63] 开启事务
来源：http://zu.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fq.shtwfgs.cn

[Q64] 提交事务
来源：http://mp.wgjwhj.cn

COMMIT;
来源：http://vz.nszjky.cn

[Q65] 回滚事务
来源：http://zg.szsharing.cn

ROLLBACK;
来源：http://pv.colortex.cn

[Q66] 行锁查询
来源：http://qd.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zl.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://nw.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gb.huanxung.cn

[Q68] 保存点
来源：http://dn.nicolike.cn

SAVEPOINT sp1;
来源：http://yk.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://sd.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://iv.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nh.gzmigu.cn

[Q70] 更新统计信息
来源：http://ae.shxzukj.cn

ANALYZE TABLE users;
来源：http://ix.huixiangedu.cn

[Q71] 查看建表语句
来源：http://vr.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cd.shxzukj.cn

[Q72] 查看索引
来源：http://pj.colortex.cn

SHOW INDEX FROM users;
来源：http://tj.hahajie.cn

[Q73] 查看表状态
来源：http://yv.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pg.nicolike.cn

[Q74] 强制使用索引
来源：http://dc.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://su.bjjhwx.cn

[Q75] 日期格式化
来源：http://ux.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uz.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oz.yuexingan06.cn

[Q76] 按天统计
来源：http://ik.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vq.9csxet.cn

[Q77] 时间加减
来源：http://ch.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qs.hnjuh.cn

[Q78] 当前时间
来源：http://rr.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qg.panjiajie.cn

[Q79] 字符串拼接
来源：http://mh.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hv.wgjwhj.cn

[Q80] 字符串截取
来源：http://xm.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dc.lnxyls.cn

[Q81] 字符串替换
来源：http://lt.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yf.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://cn.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qj.haigaiapp.cn

[Q83] 大小写转换
来源：http://ro.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hr.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://vs.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://th.yuntaijiaju.cn

[Q85] 数值取整
来源：http://je.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xx.colortex.cn

[Q86] 读取 JSON 字段
来源：http://as.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kh.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://ni.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qx.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://ty.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ko.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xv.szxytkj.cn

[Q89] 判断表是否存在
来源：http://ud.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qm.yuexingan06.cn

[Q90] 生成序号列
来源：http://rm.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bq.lnxyls.cn

================================================================================
来源：http://qs.wgjwhj.cn

R. Bash 专题
来源：http://op.shtwfgs.cn

================================================================================
来源：http://nu.newstarts.cn

[R01] shebang 与严格模式
来源：http://xu.lnxyls.cn

#!/usr/bin/env bash
来源：http://qu.chemitech.net.cn

set -euo pipefail
来源：http://sa.nszjky.cn

[R02] 变量赋值与使用
来源：http://qs.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://xo.huixiangedu.cn

[R03] 只读变量
来源：http://gv.newstarts.cn

readonly PI=3.14
来源：http://rn.huixinmuqiang.cn

[R04] 位置参数
来源：http://ni.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://as.521024.cn

[R05] 参数默认值
来源：http://bm.chemitech.net.cn

name="${1:-default}"
来源：http://ys.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://uc.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dk.panjiajie.cn

[R07] if 判断文件
来源：http://cv.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mm.yuntaijiaju.cn

[R08] 数值比较
来源：http://mr.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ik.chemitech.net.cn

[R09] 字符串比较
来源：http://tg.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qo.szxytkj.cn

[R10] 正则匹配
来源：http://tg.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ip.panjiajie.cn

[R11] case 多分支
来源：http://he.shxzskj.cn

case "$1" in
来源：http://gb.nicolike.cn

start) echo "启动" ;;
来源：http://ef.panjiajie.cn

stop)  echo "停止" ;;
来源：http://bi.521024.cn

*)     echo "未知命令" ;;
来源：http://te.521024.cn

esac
来源：http://za.bjjhwx.cn

[R12] for 遍历文件
来源：http://hx.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://fp.jctech888.com.cn

[R13] for 计数循环
来源：http://dk.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://uz.wgjwhj.cn

[R14] C 风格 for
来源：http://gx.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lp.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://lh.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rl.jianghongdianzi.cn

[R16] until 等待条件
来源：http://ey.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qq.muxihuayi.cn

[R17] 数组定义与取值
来源：http://kg.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ss.huixinmuqiang.cn

[R18] 遍历数组
来源：http://eo.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mb.9csxet.cn

[R19] 数组长度
来源：http://nu.lnxyls.cn

echo "${#arr[@]}"
来源：http://mg.szxytkj.cn

[R20] 关联数组（字典）
来源：http://by.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xd.huixinmuqiang.cn

[R21] 字符串长度
来源：http://jd.huixiangedu.cn

echo "${#s}"
来源：http://tg.huixinmuqiang.cn

[R22] 截取子串
来源：http://lv.hahajie.cn

echo "${s:0:5}"
来源：http://gq.9csxet.cn

[R23] 字符串替换
来源：http://ee.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lh.hnjuh.cn

[R24] 大小写转换
来源：http://cx.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vq.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://vi.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cn.9csxet.cn

[R26] 命令替换
来源：http://dd.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://bl.huixiangedu.cn

[R27] 算术展开
来源：http://qx.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ae.bookmarksfly.cn

[R28] 浮点运算
来源：http://jc.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://by.muxihuayi.cn

[R29] 定义函数
来源：http://pp.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tz.colortex.cn

[R30] 函数返回状态码
来源：http://pq.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://jv.asd995.cn

[R31] 局部变量
来源：http://tq.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://sx.nicolike.cn

[R32] 参数个数校验
来源：http://xa.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jy.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://cv.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pm.huixinmuqiang.cn

[R34] 退出时清理
来源：http://rw.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oh.yuexingan06.cn

[R35] 后台执行并等待
来源：http://gt.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iw.szxytkj.cn

[R36] 并发执行多个任务
来源：http://pp.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wf.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://yz.shtwfgs.cn

files=$(ls -1)
来源：http://mo.gzmigu.cn

[R38] 管道串联
来源：http://qk.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://wd.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://yb.bjjhwx.cn

cmd > out.log 2>&1
来源：http://sy.panjiajie.cn

[R40] 追加写日志
来源：http://ml.yuntaijiaju.cn

echo "log" >> out.log
来源：http://ye.muxihuayi.cn

[R41] 丢弃输出
来源：http://ta.colortex.cn

cmd >/dev/null 2>&1
来源：http://wh.shxzukj.cn

[R42] 输入重定向
来源：http://xs.nicolike.cn

wc -l < a.txt
来源：http://fq.lnxyls.cn

[R43] 按名字查找文件
来源：http://vd.szxytkj.cn

find . -name "*.log" -type f
来源：http://xr.colortex.cn

[R44] 按修改时间查找
来源：http://hn.lnxyls.cn

find . -mtime -7 -type f
来源：http://ju.nicolike.cn

[R45] 批量删除
来源：http://vl.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://mv.asd995.cn

[R46] 递归替换文件内容
来源：http://on.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ry.colortex.cn

[R47] sed 单行替换
来源：http://tz.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ey.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://kc.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://ad.shxzukj.cn

[R49] awk 带条件
来源：http://il.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tz.muxihuayi.cn

[R50] awk 求和
来源：http://an.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ra.yuexingan06.cn

[R51] 排序去重取前几
来源：http://qs.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pg.wgjwhj.cn

[R52] 统计行数
来源：http://db.asd995.cn

wc -l a.txt
来源：http://rg.colortex.cn

[R53] 查看文件头与实时尾
来源：http://ev.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jm.jctech888.com.cn

[R54] 比较两个文件
来源：http://dw.huixinmuqiang.cn

diff a.txt b.txt
来源：http://jz.9csxet.cn

[R55] 压缩与解压
来源：http://ze.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vf.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://sc.bookmarksfly.cn

scp file user@host:/path/
来源：http://qy.nicolike.cn

[R57] 远程执行命令
来源：http://ky.asd995.cn

ssh user@host 'uptime'
来源：http://cb.shxzskj.cn

[R58] 下载文件
来源：http://tn.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://re.lnxyls.cn

[R59] 发 POST JSON
来源：http://eq.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pt.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://nt.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ai.jctech888.com.cn

[R61] 磁盘占用
来源：http://ie.yuexingan06.cn

df -h;  du -sh *
来源：http://ln.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://jx.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://un.nicolike.cn

[R63] 内存与进程
来源：http://kz.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://ef.huanxung.cn

[R64] 结束进程
来源：http://oo.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://rl.huixiangedu.cn

[R65] 查看端口占用
来源：http://et.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gf.huanxung.cn

[R66] 定时任务
来源：http://zs.wgjwhj.cn

crontab -e;  crontab -l
来源：http://rm.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://xd.hnjuh.cn

openssl rand -hex 16
来源：http://yu.szxytkj.cn

[R68] 计算文件校验值
来源：http://cv.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zn.gzmigu.cn

[R69] 生成随机密码
来源：http://rd.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://uc.muxihuayi.cn

[R70] 时间戳与互转
来源：http://ez.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://xp.nszjky.cn

[R71] 日期格式化
来源：http://uu.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uq.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://qz.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ev.521024.cn

[R73] 分割大日志
来源：http://fj.huanxung.cn

split -l 1000 big.log part_
来源：http://cd.521024.cn

[R74] 批量重命名
来源：http://mw.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ce.nszjky.cn

[R75] 导出环境变量
来源：http://hr.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://lc.hnjuh.cn

[R76] 使用临时文件
来源：http://ud.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ad.9csxet.cn

[R77] 读取用户输入
来源：http://us.hnjuh.cn

read -rp "请输入: " ans
来源：http://un.wgjwhj.cn

[R78] 交互式菜单
来源：http://bi.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gu.szsharing.cn

[R79] 解析命令行选项
来源：http://zh.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hd.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://be.yuntaijiaju.cn

time ./run.sh
来源：http://ih.521024.cn

================================================================================
来源：http://gr.panjiajie.cn

S. C / C++ 专题
来源：http://wz.gzmigu.cn

================================================================================
来源：http://sg.bookmarksfly.cn

[S01] C：Hello World
来源：http://ye.huixinmuqiang.cn

#include <stdio.h>
来源：http://np.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qw.521024.cn

[S02] C：变量与格式化输出
来源：http://to.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://su.panjiajie.cn

[S03] C：读入整数
来源：http://na.colortex.cn

int x; scanf("%d", &x);
来源：http://fj.gzmigu.cn

[S04] C：字符串复制
来源：http://pm.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jg.asd995.cn

[S05] C：字符串长度
来源：http://io.hahajie.cn

strlen(s)
来源：http://nr.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://np.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://lf.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://al.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dg.colortex.cn

[S08] C：动态内存分配与释放
来源：http://zo.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ts.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://df.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cy.wgjwhj.cn

[S10] C：指针与解引用
来源：http://dp.asd995.cn

int *p = &a;  *p = 5;
来源：http://gh.nszjky.cn

[S11] C：逐行读文件
来源：http://tv.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://dk.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ux.haigaiapp.cn

fclose(f);
来源：http://re.muxihuayi.cn

[S12] C：写文件
来源：http://px.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://za.chemitech.net.cn

[S13] C：宏定义
来源：http://gz.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wd.huixinmuqiang.cn

[S14] C：枚举
来源：http://lk.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://al.9csxet.cn

[S15] C：类型转换
来源：http://qj.colortex.cn

(double) a / b
来源：http://lb.wgjwhj.cn

[S16] C：位操作置位
来源：http://wc.jianghongdianzi.cn

x |= (1 << 3);
来源：http://ef.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://et.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xo.hnjuh.cn

[S18] C：命令行参数
来源：http://br.gzmigu.cn

int main(int argc, char **argv)
来源：http://ch.gzmigu.cn

[S19] C：快速排序
来源：http://uh.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kp.yuexingan06.cn

[S20] C：二分查找
来源：http://sj.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lk.shxzskj.cn

[S21] C：字符类别判断
来源：http://yr.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pp.huixiangedu.cn

[S22] C：字符串转数字
来源：http://qn.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vc.colortex.cn

[S23] C：随机数
来源：http://hj.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cq.jctech888.com.cn

[S24] C：获取本地时间
来源：http://hp.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mz.jctech888.com.cn

[S25] C：内存拷贝
来源：http://wd.wgjwhj.cn

memcpy(dst, src, n);
来源：http://hj.521024.cn

[S26] C：内存清零
来源：http://hn.nszjky.cn

memset(a, 0, sizeof a);
来源：http://jh.yuntaijiaju.cn

[S27] C：定义常量
来源：http://zr.nicolike.cn

const double PI = 3.14159;
来源：http://fe.haigaiapp.cn

[S28] C：静态变量
来源：http://tz.shtwfgs.cn

static int counter = 0;
来源：http://cr.lnxyls.cn

[S29] C：变参函数
来源：http://od.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ve.muxihuayi.cn

[S30] C：头文件保护
来源：http://gy.hnjuh.cn

#ifndef X_H
来源：http://ko.521024.cn

#define X_H
来源：http://gt.hahajie.cn

#endif
来源：http://it.shtwfgs.cn

[S31] C++：Hello World
来源：http://hb.wgjwhj.cn


<!-- 参考信息 -->