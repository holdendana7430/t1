代发 wailian999

[Q61] 移动平均
来源：http://fk.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nd.chemitech.net.cn

[Q62] 分组占比
来源：http://fr.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://as.nszjky.cn

[Q63] 开启事务
来源：http://qh.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rx.huixinmuqiang.cn

[Q64] 提交事务
来源：http://ey.shtwfgs.cn

COMMIT;
来源：http://ba.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://wn.jianghongdianzi.cn

ROLLBACK;
来源：http://ax.szsharing.cn

[Q66] 行锁查询
来源：http://js.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ub.nicolike.cn

[Q67] 设置隔离级别
来源：http://fc.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cq.shxzskj.cn

[Q68] 保存点
来源：http://ie.colortex.cn

SAVEPOINT sp1;
来源：http://tq.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://jl.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://jj.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oj.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://qs.muxihuayi.cn

ANALYZE TABLE users;
来源：http://vj.yuexingan06.cn

[Q71] 查看建表语句
来源：http://xi.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://es.wgjwhj.cn

[Q72] 查看索引
来源：http://wr.521024.cn

SHOW INDEX FROM users;
来源：http://zy.chemitech.net.cn

[Q73] 查看表状态
来源：http://hm.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tr.huanxung.cn

[Q74] 强制使用索引
来源：http://zg.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://or.nicolike.cn

[Q75] 日期格式化
来源：http://tf.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nh.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yr.521024.cn

[Q76] 按天统计
来源：http://co.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ew.szsharing.cn

[Q77] 时间加减
来源：http://jp.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tq.hnjuh.cn

[Q78] 当前时间
来源：http://fh.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zl.bjjhwx.cn

[Q79] 字符串拼接
来源：http://ia.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vv.gzmigu.cn

[Q80] 字符串截取
来源：http://tk.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pu.huanxung.cn

[Q81] 字符串替换
来源：http://oy.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wy.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://sm.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://at.bookmarksfly.cn

[Q83] 大小写转换
来源：http://jg.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xr.gzmigu.cn

[Q84] 去除首尾空格
来源：http://ez.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://ut.muxihuayi.cn

[Q85] 数值取整
来源：http://mg.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uf.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://xq.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hl.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://gu.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mt.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://wp.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xs.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oi.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://jm.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yt.gzmigu.cn

[Q90] 生成序号列
来源：http://ns.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kk.yuntaijiaju.cn

================================================================================
来源：http://qe.haigaiapp.cn

R. Bash 专题
来源：http://ob.hnjuh.cn

================================================================================
来源：http://pg.lnxyls.cn

[R01] shebang 与严格模式
来源：http://mk.gzmigu.cn

#!/usr/bin/env bash
来源：http://vb.panjiajie.cn

set -euo pipefail
来源：http://wm.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://ae.lnxyls.cn

name="Tom"; echo "$name"
来源：http://af.nszjky.cn

[R03] 只读变量
来源：http://nq.haigaiapp.cn

readonly PI=3.14
来源：http://kl.521024.cn

[R04] 位置参数
来源：http://oh.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lt.asd995.cn

[R05] 参数默认值
来源：http://ps.nszjky.cn

name="${1:-default}"
来源：http://dw.panjiajie.cn

[R06] 判断命令是否存在
来源：http://ja.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fk.huanxung.cn

[R07] if 判断文件
来源：http://hn.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://se.asd995.cn

[R08] 数值比较
来源：http://fg.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uz.shtwfgs.cn

[R09] 字符串比较
来源：http://vo.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://by.muxihuayi.cn

[R10] 正则匹配
来源：http://ik.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ym.521024.cn

[R11] case 多分支
来源：http://iy.jianghongdianzi.cn

case "$1" in
来源：http://vs.shxzskj.cn

start) echo "启动" ;;
来源：http://zx.9csxet.cn

stop)  echo "停止" ;;
来源：http://fw.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://ll.chemitech.net.cn

esac
来源：http://px.hnjuh.cn

[R12] for 遍历文件
来源：http://gs.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://kr.bjjhwx.cn

[R13] for 计数循环
来源：http://vc.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://km.huixinmuqiang.cn

[R14] C 风格 for
来源：http://ne.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yn.521024.cn

[R15] while 逐行读文件
来源：http://wd.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dh.shxzukj.cn

[R16] until 等待条件
来源：http://ql.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dq.colortex.cn

[R17] 数组定义与取值
来源：http://zv.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gg.muxihuayi.cn

[R18] 遍历数组
来源：http://yh.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ld.bjjhwx.cn

[R19] 数组长度
来源：http://oe.gzmigu.cn

echo "${#arr[@]}"
来源：http://vn.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://hl.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tz.asd995.cn

[R21] 字符串长度
来源：http://cz.muxihuayi.cn

echo "${#s}"
来源：http://mc.nicolike.cn

[R22] 截取子串
来源：http://jd.shxzukj.cn

echo "${s:0:5}"
来源：http://to.jianghongdianzi.cn

[R23] 字符串替换
来源：http://dt.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://so.521024.cn

[R24] 大小写转换
来源：http://rv.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dl.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://fl.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tq.newstarts.cn

[R26] 命令替换
来源：http://wi.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://vd.haigaiapp.cn

[R27] 算术展开
来源：http://lf.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://fb.9csxet.cn

[R28] 浮点运算
来源：http://bw.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://xb.chemitech.net.cn

[R29] 定义函数
来源：http://gw.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xt.nszjky.cn

[R30] 函数返回状态码
来源：http://ou.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://ro.shxzskj.cn

[R31] 局部变量
来源：http://tw.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://lb.muxihuayi.cn

[R32] 参数个数校验
来源：http://dz.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sb.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://vi.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jk.yuntaijiaju.cn

[R34] 退出时清理
来源：http://wh.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zn.newstarts.cn

[R35] 后台执行并等待
来源：http://an.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fx.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://va.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wz.shxzskj.cn

[R37] 把输出赋给变量
来源：http://hd.hahajie.cn

files=$(ls -1)
来源：http://hl.newstarts.cn

[R38] 管道串联
来源：http://cx.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://bj.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://eg.lnxyls.cn

cmd > out.log 2>&1
来源：http://zm.haigaiapp.cn

[R40] 追加写日志
来源：http://vw.521024.cn

echo "log" >> out.log
来源：http://im.muxihuayi.cn

[R41] 丢弃输出
来源：http://pi.nicolike.cn

cmd >/dev/null 2>&1
来源：http://ei.asd995.cn

[R42] 输入重定向
来源：http://vo.panjiajie.cn

wc -l < a.txt
来源：http://xt.panjiajie.cn

[R43] 按名字查找文件
来源：http://im.chemitech.net.cn

find . -name "*.log" -type f
来源：http://kj.nicolike.cn

[R44] 按修改时间查找
来源：http://ur.asd995.cn

find . -mtime -7 -type f
来源：http://zt.colortex.cn

[R45] 批量删除
来源：http://qx.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://ag.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://ta.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ox.wgjwhj.cn

[R47] sed 单行替换
来源：http://td.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vu.huixiangedu.cn

[R48] awk 取指定列
来源：http://ee.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://pr.lnxyls.cn

[R49] awk 带条件
来源：http://lt.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sn.newstarts.cn

[R50] awk 求和
来源：http://pi.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jk.9csxet.cn

[R51] 排序去重取前几
来源：http://jr.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qq.bjjhwx.cn

[R52] 统计行数
来源：http://xz.panjiajie.cn

wc -l a.txt
来源：http://hz.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://qq.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zu.huixiangedu.cn

[R54] 比较两个文件
来源：http://kn.asd995.cn

diff a.txt b.txt
来源：http://jh.shtwfgs.cn

[R55] 压缩与解压
来源：http://sq.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pv.colortex.cn

[R56] 远程拷贝
来源：http://dp.colortex.cn

scp file user@host:/path/
来源：http://fj.shxzukj.cn

[R57] 远程执行命令
来源：http://kd.szsharing.cn

ssh user@host 'uptime'
来源：http://ap.hnjuh.cn

[R58] 下载文件
来源：http://wl.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ad.nszjky.cn

[R59] 发 POST JSON
来源：http://gx.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zb.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://wd.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bw.bjjhwx.cn

[R61] 磁盘占用
来源：http://fv.hahajie.cn

df -h;  du -sh *
来源：http://at.lnxyls.cn

[R62] 找最占空间的文件
来源：http://wx.asd995.cn

du -ah . | sort -rh | head -10
来源：http://yn.bookmarksfly.cn

[R63] 内存与进程
来源：http://fo.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://lr.9csxet.cn

[R64] 结束进程
来源：http://yz.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://sa.shxzskj.cn

[R65] 查看端口占用
来源：http://iz.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ss.haigaiapp.cn

[R66] 定时任务
来源：http://df.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://ch.hahajie.cn

[R67] 生成随机十六进制串
来源：http://bn.hahajie.cn

openssl rand -hex 16
来源：http://zv.asd995.cn

[R68] 计算文件校验值
来源：http://dz.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hf.nszjky.cn

[R69] 生成随机密码
来源：http://pd.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://nt.huanxung.cn

[R70] 时间戳与互转
来源：http://oz.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://kq.nszjky.cn

[R71] 日期格式化
来源：http://op.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ej.asd995.cn

[R72] 等待端口就绪
来源：http://gj.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ks.huanxung.cn

[R73] 分割大日志
来源：http://uj.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://tu.nszjky.cn

[R74] 批量重命名
来源：http://dr.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ee.jctech888.com.cn

[R75] 导出环境变量
来源：http://rv.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ur.jctech888.com.cn

[R76] 使用临时文件
来源：http://ed.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rt.huanxung.cn

[R77] 读取用户输入
来源：http://zx.gzmigu.cn

read -rp "请输入: " ans
来源：http://ad.haigaiapp.cn

[R78] 交互式菜单
来源：http://kw.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tf.newstarts.cn

[R79] 解析命令行选项
来源：http://xi.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fu.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://nm.asd995.cn

time ./run.sh
来源：http://fp.shtwfgs.cn

================================================================================
来源：http://tk.haigaiapp.cn

S. C / C++ 专题
来源：http://cy.huixiangedu.cn

================================================================================
来源：http://qe.lnxyls.cn

[S01] C：Hello World
来源：http://gb.nszjky.cn

#include <stdio.h>
来源：http://px.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mo.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://ml.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://qc.asd995.cn

[S03] C：读入整数
来源：http://td.521024.cn

int x; scanf("%d", &x);
来源：http://vq.yuexingan06.cn

[S04] C：字符串复制
来源：http://ke.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ub.szsharing.cn

[S05] C：字符串长度
来源：http://ho.lnxyls.cn

strlen(s)
来源：http://uj.newstarts.cn

[S06] C：字符串比较
来源：http://wh.huixiangedu.cn

strcmp(a, b) == 0
来源：http://nm.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://ps.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://os.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://cz.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vf.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://md.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ik.huanxung.cn

[S10] C：指针与解引用
来源：http://db.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://qp.wgjwhj.cn

[S11] C：逐行读文件
来源：http://wz.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://ne.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gi.asd995.cn

fclose(f);
来源：http://rk.9csxet.cn

[S12] C：写文件
来源：http://pb.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bb.shtwfgs.cn

[S13] C：宏定义
来源：http://zr.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jd.9csxet.cn

[S14] C：枚举
来源：http://tn.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://ld.jctech888.com.cn

[S15] C：类型转换
来源：http://vw.huanxung.cn

(double) a / b
来源：http://zw.huixiangedu.cn

[S16] C：位操作置位
来源：http://gd.huanxung.cn

x |= (1 << 3);
来源：http://ga.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://ip.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://du.gzmigu.cn

[S18] C：命令行参数
来源：http://xb.lnxyls.cn

int main(int argc, char **argv)
来源：http://cr.haigaiapp.cn

[S19] C：快速排序
来源：http://sc.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kx.shxzskj.cn

[S20] C：二分查找
来源：http://ag.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://do.asd995.cn

[S21] C：字符类别判断
来源：http://eh.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lk.asd995.cn

[S22] C：字符串转数字
来源：http://rl.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ye.panjiajie.cn

[S23] C：随机数
来源：http://oh.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hg.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://qr.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tr.9csxet.cn

[S25] C：内存拷贝
来源：http://yi.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://gy.haigaiapp.cn

[S26] C：内存清零
来源：http://hx.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://zg.muxihuayi.cn

[S27] C：定义常量
来源：http://sq.colortex.cn

const double PI = 3.14159;
来源：http://ug.colortex.cn

[S28] C：静态变量
来源：http://vm.jianghongdianzi.cn

static int counter = 0;
来源：http://wl.bjjhwx.cn

[S29] C：变参函数
来源：http://mp.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ry.haigaiapp.cn

[S30] C：头文件保护
来源：http://jj.newstarts.cn

#ifndef X_H
来源：http://aw.lnxyls.cn

#define X_H
来源：http://ub.newstarts.cn

#endif
来源：http://dx.hnjuh.cn

[S31] C++：Hello World
来源：http://mu.asd995.cn


<!-- 参考信息 -->