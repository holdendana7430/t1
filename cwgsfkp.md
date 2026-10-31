代发 wailian999

[Q63] 开启事务
来源：http://kn.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fn.521024.cn

[Q64] 提交事务
来源：http://jp.gzmigu.cn

COMMIT;
来源：http://sc.szsharing.cn

[Q65] 回滚事务
来源：http://tu.hahajie.cn

ROLLBACK;
来源：http://fu.521024.cn

[Q66] 行锁查询
来源：http://pn.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tz.colortex.cn

[Q67] 设置隔离级别
来源：http://av.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zz.huixiangedu.cn

[Q68] 保存点
来源：http://fc.shxzukj.cn

SAVEPOINT sp1;
来源：http://vs.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://ga.newstarts.cn

[Q69] 查看执行计划
来源：http://pq.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cl.521024.cn

[Q70] 更新统计信息
来源：http://ve.hnjuh.cn

ANALYZE TABLE users;
来源：http://bp.panjiajie.cn

[Q71] 查看建表语句
来源：http://tk.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xf.muxihuayi.cn

[Q72] 查看索引
来源：http://nf.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://gi.szsharing.cn

[Q73] 查看表状态
来源：http://qs.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vf.shxzukj.cn

[Q74] 强制使用索引
来源：http://cn.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rz.jctech888.com.cn

[Q75] 日期格式化
来源：http://kc.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://on.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xd.jianghongdianzi.cn

[Q76] 按天统计
来源：http://iy.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wc.szxytkj.cn

[Q77] 时间加减
来源：http://ez.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eb.wgjwhj.cn

[Q78] 当前时间
来源：http://qq.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://on.hnjuh.cn

[Q79] 字符串拼接
来源：http://sb.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ti.haigaiapp.cn

[Q80] 字符串截取
来源：http://mb.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sd.gzmigu.cn

[Q81] 字符串替换
来源：http://xb.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qf.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://bt.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ed.gzmigu.cn

[Q83] 大小写转换
来源：http://hm.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vz.shxzukj.cn

[Q84] 去除首尾空格
来源：http://tt.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://gj.asd995.cn

[Q85] 数值取整
来源：http://cy.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cf.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://ct.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jd.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://wu.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ll.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://wh.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qy.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://up.hahajie.cn

[Q89] 判断表是否存在
来源：http://jj.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ej.nicolike.cn

[Q90] 生成序号列
来源：http://ng.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ko.colortex.cn

================================================================================
来源：http://tt.muxihuayi.cn

R. Bash 专题
来源：http://ox.chemitech.net.cn

================================================================================
来源：http://du.521024.cn

[R01] shebang 与严格模式
来源：http://fg.nicolike.cn

#!/usr/bin/env bash
来源：http://va.nicolike.cn

set -euo pipefail
来源：http://rh.newstarts.cn

[R02] 变量赋值与使用
来源：http://ck.panjiajie.cn

name="Tom"; echo "$name"
来源：http://yl.jctech888.com.cn

[R03] 只读变量
来源：http://vr.bjjhwx.cn

readonly PI=3.14
来源：http://kz.huanxung.cn

[R04] 位置参数
来源：http://za.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cy.nszjky.cn

[R05] 参数默认值
来源：http://dq.yuexingan06.cn

name="${1:-default}"
来源：http://tp.lnxyls.cn

[R06] 判断命令是否存在
来源：http://md.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cr.gzmigu.cn

[R07] if 判断文件
来源：http://ag.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rq.hahajie.cn

[R08] 数值比较
来源：http://nx.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ox.huixiangedu.cn

[R09] 字符串比较
来源：http://bi.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ii.huixinmuqiang.cn

[R10] 正则匹配
来源：http://pj.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bk.chemitech.net.cn

[R11] case 多分支
来源：http://rj.9csxet.cn

case "$1" in
来源：http://ly.shxzskj.cn

start) echo "启动" ;;
来源：http://fl.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://vy.colortex.cn

*)     echo "未知命令" ;;
来源：http://yc.haigaiapp.cn

esac
来源：http://sm.shxzskj.cn

[R12] for 遍历文件
来源：http://ap.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://vy.gzmigu.cn

[R13] for 计数循环
来源：http://sk.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://or.hnjuh.cn

[R14] C 风格 for
来源：http://nn.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shxzukj.cn

[R15] while 逐行读文件
来源：http://dr.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qw.shxzskj.cn

[R16] until 等待条件
来源：http://wh.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nc.nicolike.cn

[R17] 数组定义与取值
来源：http://zb.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lp.panjiajie.cn

[R18] 遍历数组
来源：http://rv.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rk.huixiangedu.cn

[R19] 数组长度
来源：http://lw.huixiangedu.cn

echo "${#arr[@]}"
来源：http://hg.newstarts.cn

[R20] 关联数组（字典）
来源：http://bq.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pz.huixinmuqiang.cn

[R21] 字符串长度
来源：http://cp.jianghongdianzi.cn

echo "${#s}"
来源：http://hy.muxihuayi.cn

[R22] 截取子串
来源：http://xs.521024.cn

echo "${s:0:5}"
来源：http://df.wgjwhj.cn

[R23] 字符串替换
来源：http://bz.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nz.shxzukj.cn

[R24] 大小写转换
来源：http://tk.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ny.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://bm.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wp.haigaiapp.cn

[R26] 命令替换
来源：http://xc.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://ry.asd995.cn

[R27] 算术展开
来源：http://oc.asd995.cn

echo $((1 + 2 * 3))
来源：http://nx.shxzukj.cn

[R28] 浮点运算
来源：http://pb.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://zx.huixiangedu.cn

[R29] 定义函数
来源：http://xh.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pk.yuexingan06.cn

[R30] 函数返回状态码
来源：http://rn.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://dd.shtwfgs.cn

[R31] 局部变量
来源：http://qk.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://yc.lnxyls.cn

[R32] 参数个数校验
来源：http://af.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ai.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://ga.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nr.shxzskj.cn

[R34] 退出时清理
来源：http://nh.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pe.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://pa.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wl.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://pq.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lw.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://ti.lnxyls.cn

files=$(ls -1)
来源：http://cx.muxihuayi.cn

[R38] 管道串联
来源：http://fd.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://ds.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://em.szxytkj.cn

cmd > out.log 2>&1
来源：http://zo.gzmigu.cn

[R40] 追加写日志
来源：http://yl.gzmigu.cn

echo "log" >> out.log
来源：http://ca.bjjhwx.cn

[R41] 丢弃输出
来源：http://na.newstarts.cn

cmd >/dev/null 2>&1
来源：http://wx.nicolike.cn

[R42] 输入重定向
来源：http://jk.muxihuayi.cn

wc -l < a.txt
来源：http://wy.chemitech.net.cn

[R43] 按名字查找文件
来源：http://ht.shxzskj.cn

find . -name "*.log" -type f
来源：http://pi.shxzukj.cn

[R44] 按修改时间查找
来源：http://xr.wgjwhj.cn

find . -mtime -7 -type f
来源：http://et.asd995.cn

[R45] 批量删除
来源：http://bn.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://wf.hnjuh.cn

[R46] 递归替换文件内容
来源：http://ej.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pc.newstarts.cn

[R47] sed 单行替换
来源：http://kg.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lq.nicolike.cn

[R48] awk 取指定列
来源：http://ut.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://jk.shxzskj.cn

[R49] awk 带条件
来源：http://jc.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kk.shtwfgs.cn

[R50] awk 求和
来源：http://ck.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yv.hnjuh.cn

[R51] 排序去重取前几
来源：http://ex.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://as.jctech888.com.cn

[R52] 统计行数
来源：http://xb.shtwfgs.cn

wc -l a.txt
来源：http://hg.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://oa.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fo.521024.cn

[R54] 比较两个文件
来源：http://sa.huixinmuqiang.cn

diff a.txt b.txt
来源：http://lq.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://eb.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pf.wgjwhj.cn

[R56] 远程拷贝
来源：http://kd.hahajie.cn

scp file user@host:/path/
来源：http://lm.yuexingan06.cn

[R57] 远程执行命令
来源：http://fh.bjjhwx.cn

ssh user@host 'uptime'
来源：http://et.huixiangedu.cn

[R58] 下载文件
来源：http://ri.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cc.bjjhwx.cn

[R59] 发 POST JSON
来源：http://xi.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dp.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://it.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://it.lnxyls.cn

[R61] 磁盘占用
来源：http://ki.muxihuayi.cn

df -h;  du -sh *
来源：http://lt.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://ay.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://xx.lnxyls.cn

[R63] 内存与进程
来源：http://bf.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://fh.huixiangedu.cn

[R64] 结束进程
来源：http://sf.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://ty.bookmarksfly.cn

[R65] 查看端口占用
来源：http://zm.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ff.muxihuayi.cn

[R66] 定时任务
来源：http://zw.nicolike.cn

crontab -e;  crontab -l
来源：http://fl.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://qo.521024.cn

openssl rand -hex 16
来源：http://th.lnxyls.cn

[R68] 计算文件校验值
来源：http://zv.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pu.muxihuayi.cn

[R69] 生成随机密码
来源：http://bs.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://gx.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://rs.asd995.cn

date +%s;  date -d @1700000000
来源：http://sn.chemitech.net.cn

[R71] 日期格式化
来源：http://gd.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cs.huixiangedu.cn

[R72] 等待端口就绪
来源：http://fi.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qv.muxihuayi.cn

[R73] 分割大日志
来源：http://qi.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://rw.hahajie.cn

[R74] 批量重命名
来源：http://wm.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://el.huixiangedu.cn

[R75] 导出环境变量
来源：http://mw.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://zl.newstarts.cn

[R76] 使用临时文件
来源：http://kh.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ec.yuexingan06.cn

[R77] 读取用户输入
来源：http://hs.panjiajie.cn

read -rp "请输入: " ans
来源：http://xg.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://dm.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nm.yuexingan06.cn

[R79] 解析命令行选项
来源：http://pu.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://md.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://kj.hahajie.cn

time ./run.sh
来源：http://yh.huanxung.cn

================================================================================
来源：http://lt.shxzukj.cn

S. C / C++ 专题
来源：http://vf.muxihuayi.cn

================================================================================
来源：http://jx.nicolike.cn

[S01] C：Hello World
来源：http://gp.shxzskj.cn

#include <stdio.h>
来源：http://cx.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ea.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://gv.521024.cn

int a = 10; printf("%d\n", a);
来源：http://xx.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ty.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://ib.huanxung.cn

[S04] C：字符串复制
来源：http://ux.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lz.huixiangedu.cn

[S05] C：字符串长度
来源：http://og.gzmigu.cn

strlen(s)
来源：http://hn.yuexingan06.cn

[S06] C：字符串比较
来源：http://de.huanxung.cn

strcmp(a, b) == 0
来源：http://kg.panjiajie.cn

[S07] C：数组遍历求和
来源：http://fb.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://us.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://bm.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bf.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://en.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://me.muxihuayi.cn

[S10] C：指针与解引用
来源：http://sk.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://ce.szsharing.cn

[S11] C：逐行读文件
来源：http://fp.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://pb.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://db.colortex.cn

fclose(f);
来源：http://dq.hahajie.cn

[S12] C：写文件
来源：http://qa.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pz.bookmarksfly.cn

[S13] C：宏定义
来源：http://bk.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ez.9csxet.cn

[S14] C：枚举
来源：http://ry.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://fg.shxzskj.cn

[S15] C：类型转换
来源：http://bt.hnjuh.cn

(double) a / b
来源：http://jw.shxzukj.cn

[S16] C：位操作置位
来源：http://uo.newstarts.cn

x |= (1 << 3);
来源：http://fk.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://lv.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rm.lnxyls.cn

[S18] C：命令行参数
来源：http://ax.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://aj.huixinmuqiang.cn

[S19] C：快速排序
来源：http://er.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://le.9csxet.cn

[S20] C：二分查找
来源：http://nf.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cs.yuexingan06.cn

[S21] C：字符类别判断
来源：http://ya.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rl.huanxung.cn

[S22] C：字符串转数字
来源：http://dz.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://av.yuntaijiaju.cn

[S23] C：随机数
来源：http://gs.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xo.chemitech.net.cn

[S24] C：获取本地时间
来源：http://eo.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kk.chemitech.net.cn

[S25] C：内存拷贝
来源：http://em.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://eb.lnxyls.cn

[S26] C：内存清零
来源：http://tk.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://ar.yuexingan06.cn

[S27] C：定义常量
来源：http://pk.521024.cn

const double PI = 3.14159;
来源：http://db.haigaiapp.cn

[S28] C：静态变量
来源：http://lh.shtwfgs.cn

static int counter = 0;
来源：http://nh.huanxung.cn

[S29] C：变参函数
来源：http://lk.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://om.szxytkj.cn

[S30] C：头文件保护
来源：http://pb.szsharing.cn

#ifndef X_H
来源：http://cr.nszjky.cn

#define X_H
来源：http://wd.yuexingan06.cn

#endif
来源：http://hn.lnxyls.cn

[S31] C++：Hello World
来源：http://ue.huixinmuqiang.cn

#include <iostream>
来源：http://js.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://mt.9csxet.cn

[S32] C++：字符串
来源：http://xw.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://ij.nicolike.cn


<!-- 参考信息 -->