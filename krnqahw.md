代发 wailian999

[Q63] 开启事务
来源：http://se.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vd.hahajie.cn

[Q64] 提交事务
来源：http://tv.chemitech.net.cn

COMMIT;
来源：http://dg.shtwfgs.cn

[Q65] 回滚事务
来源：http://sp.gzmigu.cn

ROLLBACK;
来源：http://uu.shxzukj.cn

[Q66] 行锁查询
来源：http://gm.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ev.huanxung.cn

[Q67] 设置隔离级别
来源：http://fl.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pr.shxzukj.cn

[Q68] 保存点
来源：http://pc.yuexingan06.cn

SAVEPOINT sp1;
来源：http://yl.nszjky.cn

ROLLBACK TO sp1;
来源：http://ba.9csxet.cn

[Q69] 查看执行计划
来源：http://bj.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jl.hnjuh.cn

[Q70] 更新统计信息
来源：http://tm.chemitech.net.cn

ANALYZE TABLE users;
来源：http://sy.haigaiapp.cn

[Q71] 查看建表语句
来源：http://de.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ck.bjjhwx.cn

[Q72] 查看索引
来源：http://ky.szsharing.cn

SHOW INDEX FROM users;
来源：http://fk.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://vi.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yk.nszjky.cn

[Q74] 强制使用索引
来源：http://jh.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ad.bookmarksfly.cn

[Q75] 日期格式化
来源：http://dn.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rr.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wy.bookmarksfly.cn

[Q76] 按天统计
来源：http://tv.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ja.521024.cn

[Q77] 时间加减
来源：http://ng.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mg.yuexingan06.cn

[Q78] 当前时间
来源：http://zf.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eu.shtwfgs.cn

[Q79] 字符串拼接
来源：http://cz.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pg.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://ik.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wf.haigaiapp.cn

[Q81] 字符串替换
来源：http://ye.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ux.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://ze.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vw.nszjky.cn

[Q83] 大小写转换
来源：http://gq.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fj.panjiajie.cn

[Q84] 去除首尾空格
来源：http://bl.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://wm.gzmigu.cn

[Q85] 数值取整
来源：http://wd.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yy.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://bf.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ip.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://yw.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oj.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://yb.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mw.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qb.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://uu.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pb.chemitech.net.cn

[Q90] 生成序号列
来源：http://ai.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://by.panjiajie.cn

================================================================================
来源：http://xr.haigaiapp.cn

R. Bash 专题
来源：http://qy.bookmarksfly.cn

================================================================================
来源：http://or.9csxet.cn

[R01] shebang 与严格模式
来源：http://uf.shxzskj.cn

#!/usr/bin/env bash
来源：http://wc.nszjky.cn

set -euo pipefail
来源：http://mn.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://rs.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://an.panjiajie.cn

[R03] 只读变量
来源：http://rx.colortex.cn

readonly PI=3.14
来源：http://rg.hahajie.cn

[R04] 位置参数
来源：http://jy.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lw.shxzskj.cn

[R05] 参数默认值
来源：http://ld.hahajie.cn

name="${1:-default}"
来源：http://ai.nicolike.cn

[R06] 判断命令是否存在
来源：http://st.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yb.jctech888.com.cn

[R07] if 判断文件
来源：http://zr.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dy.colortex.cn

[R08] 数值比较
来源：http://zf.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hy.shxzskj.cn

[R09] 字符串比较
来源：http://ax.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ax.nszjky.cn

[R10] 正则匹配
来源：http://ir.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fc.gzmigu.cn

[R11] case 多分支
来源：http://qg.9csxet.cn

case "$1" in
来源：http://tc.lnxyls.cn

start) echo "启动" ;;
来源：http://yx.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://rz.hahajie.cn

*)     echo "未知命令" ;;
来源：http://ay.muxihuayi.cn

esac
来源：http://sr.szxytkj.cn

[R12] for 遍历文件
来源：http://bd.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://pq.shtwfgs.cn

[R13] for 计数循环
来源：http://rb.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://cj.nicolike.cn

[R14] C 风格 for
来源：http://pp.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dh.521024.cn

[R15] while 逐行读文件
来源：http://hk.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yz.huixinmuqiang.cn

[R16] until 等待条件
来源：http://ck.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yo.haigaiapp.cn

[R17] 数组定义与取值
来源：http://sd.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ch.colortex.cn

[R18] 遍历数组
来源：http://wh.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hs.huixinmuqiang.cn

[R19] 数组长度
来源：http://rv.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://vq.lnxyls.cn

[R20] 关联数组（字典）
来源：http://xz.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xs.yuntaijiaju.cn

[R21] 字符串长度
来源：http://bn.huanxung.cn

echo "${#s}"
来源：http://qx.colortex.cn

[R22] 截取子串
来源：http://dy.bookmarksfly.cn

echo "${s:0:5}"
来源：http://vw.bjjhwx.cn

[R23] 字符串替换
来源：http://vz.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jv.shxzukj.cn

[R24] 大小写转换
来源：http://tt.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qa.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://vy.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eq.521024.cn

[R26] 命令替换
来源：http://yp.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://vk.colortex.cn

[R27] 算术展开
来源：http://go.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://nt.hahajie.cn

[R28] 浮点运算
来源：http://cu.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://xs.newstarts.cn

[R29] 定义函数
来源：http://ao.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://or.haigaiapp.cn

[R30] 函数返回状态码
来源：http://sg.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://un.nicolike.cn

[R31] 局部变量
来源：http://km.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://iw.bookmarksfly.cn

[R32] 参数个数校验
来源：http://pm.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ms.colortex.cn

[R33] 捕获错误并提示行号
来源：http://in.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fc.huixiangedu.cn

[R34] 退出时清理
来源：http://wu.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vf.chemitech.net.cn

[R35] 后台执行并等待
来源：http://jv.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fv.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://ny.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bv.szxytkj.cn

[R37] 把输出赋给变量
来源：http://jp.yuexingan06.cn

files=$(ls -1)
来源：http://qv.jctech888.com.cn

[R38] 管道串联
来源：http://lf.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://ef.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://dg.bjjhwx.cn

cmd > out.log 2>&1
来源：http://tf.chemitech.net.cn

[R40] 追加写日志
来源：http://ub.jctech888.com.cn

echo "log" >> out.log
来源：http://ap.muxihuayi.cn

[R41] 丢弃输出
来源：http://mw.colortex.cn

cmd >/dev/null 2>&1
来源：http://bp.newstarts.cn

[R42] 输入重定向
来源：http://mi.muxihuayi.cn

wc -l < a.txt
来源：http://db.shxzskj.cn

[R43] 按名字查找文件
来源：http://ow.9csxet.cn

find . -name "*.log" -type f
来源：http://ch.muxihuayi.cn

[R44] 按修改时间查找
来源：http://lk.bjjhwx.cn

find . -mtime -7 -type f
来源：http://zf.shxzskj.cn

[R45] 批量删除
来源：http://ew.huanxung.cn

find . -name "*.tmp" -delete
来源：http://dx.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://dp.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hk.jctech888.com.cn

[R47] sed 单行替换
来源：http://ve.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yu.lnxyls.cn

[R48] awk 取指定列
来源：http://li.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://pe.asd995.cn

[R49] awk 带条件
来源：http://io.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bw.hnjuh.cn

[R50] awk 求和
来源：http://fw.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vs.9csxet.cn

[R51] 排序去重取前几
来源：http://vr.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iv.hahajie.cn

[R52] 统计行数
来源：http://lo.521024.cn

wc -l a.txt
来源：http://tr.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://wg.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vo.huanxung.cn

[R54] 比较两个文件
来源：http://hh.9csxet.cn

diff a.txt b.txt
来源：http://oa.nicolike.cn

[R55] 压缩与解压
来源：http://ec.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ci.chemitech.net.cn

[R56] 远程拷贝
来源：http://qs.newstarts.cn

scp file user@host:/path/
来源：http://pw.521024.cn

[R57] 远程执行命令
来源：http://hu.haigaiapp.cn

ssh user@host 'uptime'
来源：http://ji.jianghongdianzi.cn

[R58] 下载文件
来源：http://mp.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rn.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://sf.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xm.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://rt.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xh.lnxyls.cn

[R61] 磁盘占用
来源：http://nd.jianghongdianzi.cn

df -h;  du -sh *
来源：http://ex.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://ld.521024.cn

du -ah . | sort -rh | head -10
来源：http://in.asd995.cn

[R63] 内存与进程
来源：http://kn.521024.cn

free -h;  ps aux | grep nginx
来源：http://gl.colortex.cn

[R64] 结束进程
来源：http://sm.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://py.lnxyls.cn

[R65] 查看端口占用
来源：http://xy.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pl.jctech888.com.cn

[R66] 定时任务
来源：http://zh.bjjhwx.cn

crontab -e;  crontab -l
来源：http://rs.asd995.cn

[R67] 生成随机十六进制串
来源：http://el.hnjuh.cn

openssl rand -hex 16
来源：http://zm.newstarts.cn

[R68] 计算文件校验值
来源：http://ao.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://th.huixiangedu.cn

[R69] 生成随机密码
来源：http://qo.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://xt.lnxyls.cn

[R70] 时间戳与互转
来源：http://mf.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://cm.panjiajie.cn

[R71] 日期格式化
来源：http://vl.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yp.wgjwhj.cn

[R72] 等待端口就绪
来源：http://al.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cb.jctech888.com.cn

[R73] 分割大日志
来源：http://me.newstarts.cn

split -l 1000 big.log part_
来源：http://ry.panjiajie.cn

[R74] 批量重命名
来源：http://to.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://im.szxytkj.cn

[R75] 导出环境变量
来源：http://bj.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://ui.hahajie.cn

[R76] 使用临时文件
来源：http://qr.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nc.szsharing.cn

[R77] 读取用户输入
来源：http://lb.huanxung.cn

read -rp "请输入: " ans
来源：http://mv.hnjuh.cn

[R78] 交互式菜单
来源：http://sp.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ir.newstarts.cn

[R79] 解析命令行选项
来源：http://oi.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wn.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://vv.gzmigu.cn

time ./run.sh
来源：http://zk.chemitech.net.cn

================================================================================
来源：http://iq.huixinmuqiang.cn

S. C / C++ 专题
来源：http://or.wgjwhj.cn

================================================================================
来源：http://qu.shtwfgs.cn

[S01] C：Hello World
来源：http://mu.jctech888.com.cn

#include <stdio.h>
来源：http://bb.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nm.colortex.cn

[S02] C：变量与格式化输出
来源：http://qv.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://om.9csxet.cn

[S03] C：读入整数
来源：http://yc.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://uu.gzmigu.cn

[S04] C：字符串复制
来源：http://mm.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gf.gzmigu.cn

[S05] C：字符串长度
来源：http://di.521024.cn

strlen(s)
来源：http://ty.muxihuayi.cn

[S06] C：字符串比较
来源：http://iz.9csxet.cn

strcmp(a, b) == 0
来源：http://tk.panjiajie.cn

[S07] C：数组遍历求和
来源：http://gl.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://il.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://nt.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ke.asd995.cn

[S09] C：结构体定义与初始化
来源：http://wg.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gz.shxzukj.cn

[S10] C：指针与解引用
来源：http://ko.521024.cn

int *p = &a;  *p = 5;
来源：http://px.panjiajie.cn

[S11] C：逐行读文件
来源：http://ht.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://hm.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jl.nszjky.cn

fclose(f);
来源：http://nu.9csxet.cn

[S12] C：写文件
来源：http://hs.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vq.yuexingan06.cn

[S13] C：宏定义
来源：http://yq.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://to.jianghongdianzi.cn

[S14] C：枚举
来源：http://mk.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://kj.hahajie.cn

[S15] C：类型转换
来源：http://tr.shtwfgs.cn

(double) a / b
来源：http://td.hnjuh.cn

[S16] C：位操作置位
来源：http://au.nicolike.cn

x |= (1 << 3);
来源：http://zw.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://xd.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ao.521024.cn

[S18] C：命令行参数
来源：http://tn.jctech888.com.cn

int main(int argc, char **argv)
来源：http://ox.szxytkj.cn

[S19] C：快速排序
来源：http://rb.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ti.shxzskj.cn

[S20] C：二分查找
来源：http://bi.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sl.nicolike.cn

[S21] C：字符类别判断
来源：http://fs.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fu.bjjhwx.cn

[S22] C：字符串转数字
来源：http://iu.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pl.hahajie.cn

[S23] C：随机数
来源：http://dx.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kh.lnxyls.cn

[S24] C：获取本地时间
来源：http://kf.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xc.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://wv.asd995.cn

memcpy(dst, src, n);
来源：http://rg.colortex.cn

[S26] C：内存清零
来源：http://vz.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://up.panjiajie.cn

[S27] C：定义常量
来源：http://mk.9csxet.cn

const double PI = 3.14159;
来源：http://lu.wgjwhj.cn

[S28] C：静态变量
来源：http://un.yuexingan06.cn

static int counter = 0;
来源：http://pd.gzmigu.cn

[S29] C：变参函数
来源：http://qo.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zl.huixiangedu.cn

[S30] C：头文件保护
来源：http://pz.szxytkj.cn

#ifndef X_H
来源：http://tr.shxzskj.cn

#define X_H
来源：http://qw.bjjhwx.cn

#endif
来源：http://mp.gzmigu.cn

[S31] C++：Hello World
来源：http://ij.asd995.cn

#include <iostream>
来源：http://ay.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ww.yuexingan06.cn

[S32] C++：字符串
来源：http://go.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://rq.panjiajie.cn


<!-- 参考信息 -->