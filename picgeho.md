代发 wailian999

[Q61] 移动平均
来源：http://eo.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ew.huixinmuqiang.cn

[Q62] 分组占比
来源：http://bq.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ao.asd995.cn

[Q63] 开启事务
来源：http://qp.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hw.muxihuayi.cn

[Q64] 提交事务
来源：http://ok.huixinmuqiang.cn

COMMIT;
来源：http://jl.shxzskj.cn

[Q65] 回滚事务
来源：http://mu.yuexingan06.cn

ROLLBACK;
来源：http://mb.hahajie.cn

[Q66] 行锁查询
来源：http://oo.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pk.huanxung.cn

[Q67] 设置隔离级别
来源：http://km.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sf.huixinmuqiang.cn

[Q68] 保存点
来源：http://gg.521024.cn

SAVEPOINT sp1;
来源：http://kv.521024.cn

ROLLBACK TO sp1;
来源：http://fn.newstarts.cn

[Q69] 查看执行计划
来源：http://ak.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://db.jctech888.com.cn

[Q70] 更新统计信息
来源：http://zk.chemitech.net.cn

ANALYZE TABLE users;
来源：http://qq.hahajie.cn

[Q71] 查看建表语句
来源：http://pb.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://up.haigaiapp.cn

[Q72] 查看索引
来源：http://sa.9csxet.cn

SHOW INDEX FROM users;
来源：http://mi.huixiangedu.cn

[Q73] 查看表状态
来源：http://rp.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xk.chemitech.net.cn

[Q74] 强制使用索引
来源：http://fa.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://da.colortex.cn

[Q75] 日期格式化
来源：http://lp.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qn.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ca.chemitech.net.cn

[Q76] 按天统计
来源：http://hg.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ff.asd995.cn

[Q77] 时间加减
来源：http://qo.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ok.asd995.cn

[Q78] 当前时间
来源：http://ma.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kj.newstarts.cn

[Q79] 字符串拼接
来源：http://gv.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jq.nszjky.cn

[Q80] 字符串截取
来源：http://dv.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jt.wgjwhj.cn

[Q81] 字符串替换
来源：http://rn.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xq.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://qq.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qk.hnjuh.cn

[Q83] 大小写转换
来源：http://ro.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://as.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://iy.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://mu.shxzukj.cn

[Q85] 数值取整
来源：http://yv.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hb.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://gg.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lt.asd995.cn

[Q87] JSON 字段做条件
来源：http://xt.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zu.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://jo.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ar.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zn.shxzukj.cn

[Q89] 判断表是否存在
来源：http://uu.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://th.szsharing.cn

[Q90] 生成序号列
来源：http://jk.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ga.nszjky.cn

================================================================================
来源：http://bv.shxzukj.cn

R. Bash 专题
来源：http://rd.huixiangedu.cn

================================================================================
来源：http://rh.nszjky.cn

[R01] shebang 与严格模式
来源：http://gv.gzmigu.cn

#!/usr/bin/env bash
来源：http://lv.huixinmuqiang.cn

set -euo pipefail
来源：http://id.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://go.nszjky.cn

name="Tom"; echo "$name"
来源：http://uw.bookmarksfly.cn

[R03] 只读变量
来源：http://xm.bookmarksfly.cn

readonly PI=3.14
来源：http://ki.shxzskj.cn

[R04] 位置参数
来源：http://lp.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hd.chemitech.net.cn

[R05] 参数默认值
来源：http://jq.hahajie.cn

name="${1:-default}"
来源：http://ag.nszjky.cn

[R06] 判断命令是否存在
来源：http://ri.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lu.szxytkj.cn

[R07] if 判断文件
来源：http://ir.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qk.jianghongdianzi.cn

[R08] 数值比较
来源：http://lz.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jo.huixinmuqiang.cn

[R09] 字符串比较
来源：http://xi.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zy.gzmigu.cn

[R10] 正则匹配
来源：http://uj.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bw.bjjhwx.cn

[R11] case 多分支
来源：http://tn.hnjuh.cn

case "$1" in
来源：http://dr.nicolike.cn

start) echo "启动" ;;
来源：http://kj.521024.cn

stop)  echo "停止" ;;
来源：http://ym.9csxet.cn

*)     echo "未知命令" ;;
来源：http://cr.yuntaijiaju.cn

esac
来源：http://xc.shxzukj.cn

[R12] for 遍历文件
来源：http://zh.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://pf.521024.cn

[R13] for 计数循环
来源：http://to.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ss.jianghongdianzi.cn

[R14] C 风格 for
来源：http://kq.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ae.jctech888.com.cn

[R15] while 逐行读文件
来源：http://ao.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hq.gzmigu.cn

[R16] until 等待条件
来源：http://tm.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kq.huanxung.cn

[R17] 数组定义与取值
来源：http://pj.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zx.yuexingan06.cn

[R18] 遍历数组
来源：http://oi.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://se.nicolike.cn

[R19] 数组长度
来源：http://tj.521024.cn

echo "${#arr[@]}"
来源：http://ht.521024.cn

[R20] 关联数组（字典）
来源：http://um.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://co.wgjwhj.cn

[R21] 字符串长度
来源：http://sh.colortex.cn

echo "${#s}"
来源：http://ot.nszjky.cn

[R22] 截取子串
来源：http://wq.hnjuh.cn

echo "${s:0:5}"
来源：http://io.wgjwhj.cn

[R23] 字符串替换
来源：http://tw.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jr.huanxung.cn

[R24] 大小写转换
来源：http://er.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xa.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://hr.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ug.muxihuayi.cn

[R26] 命令替换
来源：http://gb.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://iw.chemitech.net.cn

[R27] 算术展开
来源：http://tt.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://ay.huanxung.cn

[R28] 浮点运算
来源：http://fk.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://wq.9csxet.cn

[R29] 定义函数
来源：http://wv.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wa.huanxung.cn

[R30] 函数返回状态码
来源：http://pm.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://oy.gzmigu.cn

[R31] 局部变量
来源：http://fc.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://kb.asd995.cn

[R32] 参数个数校验
来源：http://vb.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qx.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://fe.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ws.521024.cn

[R34] 退出时清理
来源：http://uq.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ec.nszjky.cn

[R35] 后台执行并等待
来源：http://oh.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ew.szsharing.cn

[R36] 并发执行多个任务
来源：http://zo.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xn.gzmigu.cn

[R37] 把输出赋给变量
来源：http://zm.shtwfgs.cn

files=$(ls -1)
来源：http://ps.wgjwhj.cn

[R38] 管道串联
来源：http://fj.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://nk.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://cg.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://ro.shxzukj.cn

[R40] 追加写日志
来源：http://fi.hahajie.cn

echo "log" >> out.log
来源：http://nf.521024.cn

[R41] 丢弃输出
来源：http://qj.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://ov.asd995.cn

[R42] 输入重定向
来源：http://fw.shxzskj.cn

wc -l < a.txt
来源：http://wd.colortex.cn

[R43] 按名字查找文件
来源：http://tk.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ms.shxzskj.cn

[R44] 按修改时间查找
来源：http://fy.asd995.cn

find . -mtime -7 -type f
来源：http://lp.bookmarksfly.cn

[R45] 批量删除
来源：http://ah.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://nw.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://wm.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ii.chemitech.net.cn

[R47] sed 单行替换
来源：http://af.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lo.huanxung.cn

[R48] awk 取指定列
来源：http://ja.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://vo.nicolike.cn

[R49] awk 带条件
来源：http://po.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ji.panjiajie.cn

[R50] awk 求和
来源：http://qj.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qi.szsharing.cn

[R51] 排序去重取前几
来源：http://jj.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://od.colortex.cn

[R52] 统计行数
来源：http://mr.haigaiapp.cn

wc -l a.txt
来源：http://db.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://en.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bh.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://gp.9csxet.cn

diff a.txt b.txt
来源：http://fm.shxzukj.cn

[R55] 压缩与解压
来源：http://rs.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pq.jctech888.com.cn

[R56] 远程拷贝
来源：http://wq.huanxung.cn

scp file user@host:/path/
来源：http://zx.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://eg.nszjky.cn

ssh user@host 'uptime'
来源：http://sj.gzmigu.cn

[R58] 下载文件
来源：http://op.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ww.shxzskj.cn

[R59] 发 POST JSON
来源：http://ew.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wv.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://we.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zz.shtwfgs.cn

[R61] 磁盘占用
来源：http://ab.hahajie.cn

df -h;  du -sh *
来源：http://yo.newstarts.cn

[R62] 找最占空间的文件
来源：http://hq.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://sn.nszjky.cn

[R63] 内存与进程
来源：http://rd.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://ox.huixiangedu.cn

[R64] 结束进程
来源：http://vg.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://hf.muxihuayi.cn

[R65] 查看端口占用
来源：http://hy.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vo.yuexingan06.cn

[R66] 定时任务
来源：http://ku.szxytkj.cn

crontab -e;  crontab -l
来源：http://qu.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://gp.jctech888.com.cn

openssl rand -hex 16
来源：http://do.hnjuh.cn

[R68] 计算文件校验值
来源：http://wh.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rp.huanxung.cn

[R69] 生成随机密码
来源：http://vg.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://ic.colortex.cn

[R70] 时间戳与互转
来源：http://lz.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://kw.9csxet.cn

[R71] 日期格式化
来源：http://wm.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rj.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://ov.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cb.521024.cn

[R73] 分割大日志
来源：http://vw.9csxet.cn

split -l 1000 big.log part_
来源：http://zz.yuntaijiaju.cn

[R74] 批量重命名
来源：http://uz.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dt.bjjhwx.cn

[R75] 导出环境变量
来源：http://lz.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://no.wgjwhj.cn

[R76] 使用临时文件
来源：http://hx.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yf.szsharing.cn

[R77] 读取用户输入
来源：http://bc.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://om.huanxung.cn

[R78] 交互式菜单
来源：http://li.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kc.chemitech.net.cn

[R79] 解析命令行选项
来源：http://sn.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jx.colortex.cn

[R80] 查看脚本执行耗时
来源：http://ha.bookmarksfly.cn

time ./run.sh
来源：http://zb.yuntaijiaju.cn

================================================================================
来源：http://aq.panjiajie.cn

S. C / C++ 专题
来源：http://sz.nszjky.cn

================================================================================
来源：http://ll.wgjwhj.cn

[S01] C：Hello World
来源：http://jt.huixinmuqiang.cn

#include <stdio.h>
来源：http://aw.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lo.colortex.cn

[S02] C：变量与格式化输出
来源：http://ou.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://bi.jianghongdianzi.cn

[S03] C：读入整数
来源：http://sa.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://ub.shtwfgs.cn

[S04] C：字符串复制
来源：http://ce.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fw.bookmarksfly.cn

[S05] C：字符串长度
来源：http://mb.gzmigu.cn

strlen(s)
来源：http://gh.huanxung.cn

[S06] C：字符串比较
来源：http://qf.newstarts.cn

strcmp(a, b) == 0
来源：http://hw.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://cm.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zl.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://lp.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uw.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://ld.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ay.shtwfgs.cn

[S10] C：指针与解引用
来源：http://ou.nicolike.cn

int *p = &a;  *p = 5;
来源：http://gs.chemitech.net.cn

[S11] C：逐行读文件
来源：http://ik.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://ab.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ij.huixiangedu.cn

fclose(f);
来源：http://dp.yuexingan06.cn

[S12] C：写文件
来源：http://za.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zv.jctech888.com.cn

[S13] C：宏定义
来源：http://gp.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zn.jianghongdianzi.cn

[S14] C：枚举
来源：http://dh.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://dg.gzmigu.cn

[S15] C：类型转换
来源：http://gl.shtwfgs.cn

(double) a / b
来源：http://es.panjiajie.cn

[S16] C：位操作置位
来源：http://ax.shxzskj.cn

x |= (1 << 3);
来源：http://tm.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ia.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bv.huixiangedu.cn

[S18] C：命令行参数
来源：http://nc.shtwfgs.cn

int main(int argc, char **argv)
来源：http://ux.szsharing.cn

[S19] C：快速排序
来源：http://sd.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jd.panjiajie.cn

[S20] C：二分查找
来源：http://bi.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ct.huanxung.cn

[S21] C：字符类别判断
来源：http://kb.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ba.hnjuh.cn

[S22] C：字符串转数字
来源：http://ks.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ts.szsharing.cn

[S23] C：随机数
来源：http://ax.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://di.nicolike.cn

[S24] C：获取本地时间
来源：http://wr.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nr.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://gq.jctech888.com.cn

memcpy(dst, src, n);
来源：http://mj.nicolike.cn

[S26] C：内存清零
来源：http://yd.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://cb.asd995.cn

[S27] C：定义常量
来源：http://ll.newstarts.cn

const double PI = 3.14159;
来源：http://xp.muxihuayi.cn

[S28] C：静态变量
来源：http://zi.bookmarksfly.cn

static int counter = 0;
来源：http://ep.szxytkj.cn

[S29] C：变参函数
来源：http://gt.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vj.bjjhwx.cn

[S30] C：头文件保护
来源：http://be.huixiangedu.cn

#ifndef X_H
来源：http://ni.szsharing.cn

#define X_H
来源：http://fp.yuntaijiaju.cn

#endif
来源：http://rr.shxzukj.cn

[S31] C++：Hello World
来源：http://gg.521024.cn


<!-- 参考信息 -->