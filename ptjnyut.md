代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://by.jctech888.com.cn

[Q58] 累计求和
来源：http://ni.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sh.panjiajie.cn

[Q59] 分组内累计
来源：http://ds.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://de.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://wf.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://se.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dw.nszjky.cn

[Q61] 移动平均
来源：http://wo.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kf.muxihuayi.cn

[Q62] 分组占比
来源：http://mf.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pl.shxzukj.cn

[Q63] 开启事务
来源：http://hw.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ye.haigaiapp.cn

[Q64] 提交事务
来源：http://ql.nicolike.cn

COMMIT;
来源：http://gz.wgjwhj.cn

[Q65] 回滚事务
来源：http://zq.shtwfgs.cn

ROLLBACK;
来源：http://pi.hnjuh.cn

[Q66] 行锁查询
来源：http://cg.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kb.huanxung.cn

[Q67] 设置隔离级别
来源：http://ev.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mh.9csxet.cn

[Q68] 保存点
来源：http://gu.hnjuh.cn

SAVEPOINT sp1;
来源：http://wx.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://ol.asd995.cn

[Q69] 查看执行计划
来源：http://ba.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mj.shtwfgs.cn

[Q70] 更新统计信息
来源：http://ib.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://sx.nicolike.cn

[Q71] 查看建表语句
来源：http://ow.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ys.muxihuayi.cn

[Q72] 查看索引
来源：http://ns.colortex.cn

SHOW INDEX FROM users;
来源：http://bq.yuexingan06.cn

[Q73] 查看表状态
来源：http://yk.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nk.shxzukj.cn

[Q74] 强制使用索引
来源：http://bx.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://se.nszjky.cn

[Q75] 日期格式化
来源：http://rf.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://se.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hf.huixinmuqiang.cn

[Q76] 按天统计
来源：http://el.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kt.szsharing.cn

[Q77] 时间加减
来源：http://xg.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gx.huixinmuqiang.cn

[Q78] 当前时间
来源：http://rk.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hx.hahajie.cn

[Q79] 字符串拼接
来源：http://br.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gzmigu.cn

[Q80] 字符串截取
来源：http://wl.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ib.haigaiapp.cn

[Q81] 字符串替换
来源：http://gn.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yi.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://ag.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lo.huixiangedu.cn

[Q83] 大小写转换
来源：http://px.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jj.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://st.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://ir.jctech888.com.cn

[Q85] 数值取整
来源：http://pv.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gm.521024.cn

[Q86] 读取 JSON 字段
来源：http://ti.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rl.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://zm.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vj.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://ax.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vi.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zl.panjiajie.cn

[Q89] 判断表是否存在
来源：http://sj.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rk.haigaiapp.cn

[Q90] 生成序号列
来源：http://uv.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dw.shxzukj.cn

================================================================================
来源：http://vu.bookmarksfly.cn

R. Bash 专题
来源：http://fe.yuexingan06.cn

================================================================================
来源：http://kq.gzmigu.cn

[R01] shebang 与严格模式
来源：http://sf.nszjky.cn

#!/usr/bin/env bash
来源：http://oz.newstarts.cn

set -euo pipefail
来源：http://bu.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://vy.shxzskj.cn

name="Tom"; echo "$name"
来源：http://fq.nicolike.cn

[R03] 只读变量
来源：http://qp.szsharing.cn

readonly PI=3.14
来源：http://ip.shtwfgs.cn

[R04] 位置参数
来源：http://ni.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ny.huixinmuqiang.cn

[R05] 参数默认值
来源：http://cj.szxytkj.cn

name="${1:-default}"
来源：http://on.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://zj.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iq.hnjuh.cn

[R07] if 判断文件
来源：http://tv.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gv.bjjhwx.cn

[R08] 数值比较
来源：http://zl.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iy.lnxyls.cn

[R09] 字符串比较
来源：http://rt.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bs.szxytkj.cn

[R10] 正则匹配
来源：http://fm.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wr.nszjky.cn

[R11] case 多分支
来源：http://sn.huanxung.cn

case "$1" in
来源：http://hm.haigaiapp.cn

start) echo "启动" ;;
来源：http://he.huanxung.cn

stop)  echo "停止" ;;
来源：http://xt.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://lp.bjjhwx.cn

esac
来源：http://it.bjjhwx.cn

[R12] for 遍历文件
来源：http://zp.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://ll.hahajie.cn

[R13] for 计数循环
来源：http://qc.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://no.asd995.cn

[R14] C 风格 for
来源：http://ot.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nv.wgjwhj.cn

[R15] while 逐行读文件
来源：http://wx.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xg.chemitech.net.cn

[R16] until 等待条件
来源：http://vl.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://km.gzmigu.cn

[R17] 数组定义与取值
来源：http://hc.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qg.szsharing.cn

[R18] 遍历数组
来源：http://wo.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lq.shxzskj.cn

[R19] 数组长度
来源：http://pn.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://bk.521024.cn

[R20] 关联数组（字典）
来源：http://aq.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fe.gzmigu.cn

[R21] 字符串长度
来源：http://xz.jctech888.com.cn

echo "${#s}"
来源：http://uz.521024.cn

[R22] 截取子串
来源：http://jg.521024.cn

echo "${s:0:5}"
来源：http://hp.bookmarksfly.cn

[R23] 字符串替换
来源：http://vs.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yf.gzmigu.cn

[R24] 大小写转换
来源：http://lq.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qt.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://lr.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pv.jctech888.com.cn

[R26] 命令替换
来源：http://ml.asd995.cn

now=$(date +%F); echo "$now"
来源：http://uj.lnxyls.cn

[R27] 算术展开
来源：http://pf.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://oj.colortex.cn

[R28] 浮点运算
来源：http://lu.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://gr.chemitech.net.cn

[R29] 定义函数
来源：http://cx.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kt.shtwfgs.cn

[R30] 函数返回状态码
来源：http://fl.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://zm.521024.cn

[R31] 局部变量
来源：http://lx.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://uv.bjjhwx.cn

[R32] 参数个数校验
来源：http://pn.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zh.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://es.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sl.muxihuayi.cn

[R34] 退出时清理
来源：http://rk.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rw.yuexingan06.cn

[R35] 后台执行并等待
来源：http://ct.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lt.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://ft.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hx.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://fv.shtwfgs.cn

files=$(ls -1)
来源：http://vh.szsharing.cn

[R38] 管道串联
来源：http://vl.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://mo.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://oo.panjiajie.cn

cmd > out.log 2>&1
来源：http://yl.wgjwhj.cn

[R40] 追加写日志
来源：http://fv.shtwfgs.cn

echo "log" >> out.log
来源：http://li.hnjuh.cn

[R41] 丢弃输出
来源：http://fh.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://cd.muxihuayi.cn

[R42] 输入重定向
来源：http://nf.yuntaijiaju.cn

wc -l < a.txt
来源：http://gc.shxzskj.cn

[R43] 按名字查找文件
来源：http://uh.shxzskj.cn

find . -name "*.log" -type f
来源：http://en.haigaiapp.cn

[R44] 按修改时间查找
来源：http://vx.panjiajie.cn

find . -mtime -7 -type f
来源：http://cr.huixinmuqiang.cn

[R45] 批量删除
来源：http://xm.nicolike.cn

find . -name "*.tmp" -delete
来源：http://hh.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://tp.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://me.huixiangedu.cn

[R47] sed 单行替换
来源：http://ow.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ck.szsharing.cn

[R48] awk 取指定列
来源：http://sk.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://rn.hahajie.cn

[R49] awk 带条件
来源：http://cq.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vi.chemitech.net.cn

[R50] awk 求和
来源：http://dr.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nu.hahajie.cn

[R51] 排序去重取前几
来源：http://xa.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kn.shtwfgs.cn

[R52] 统计行数
来源：http://lz.shtwfgs.cn

wc -l a.txt
来源：http://qb.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://su.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uo.jctech888.com.cn

[R54] 比较两个文件
来源：http://qp.shtwfgs.cn

diff a.txt b.txt
来源：http://uy.shxzukj.cn

[R55] 压缩与解压
来源：http://pj.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qk.jctech888.com.cn

[R56] 远程拷贝
来源：http://xh.szxytkj.cn

scp file user@host:/path/
来源：http://vg.newstarts.cn

[R57] 远程执行命令
来源：http://mj.nicolike.cn

ssh user@host 'uptime'
来源：http://tv.nicolike.cn

[R58] 下载文件
来源：http://nf.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xp.chemitech.net.cn

[R59] 发 POST JSON
来源：http://kv.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yo.521024.cn

[R60] 只看 HTTP 状态码
来源：http://ai.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zm.hahajie.cn

[R61] 磁盘占用
来源：http://yh.gzmigu.cn

df -h;  du -sh *
来源：http://lg.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://vu.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://ex.shxzukj.cn

[R63] 内存与进程
来源：http://zs.521024.cn

free -h;  ps aux | grep nginx
来源：http://tx.jianghongdianzi.cn

[R64] 结束进程
来源：http://ci.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://xr.panjiajie.cn

[R65] 查看端口占用
来源：http://am.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://of.shtwfgs.cn

[R66] 定时任务
来源：http://ub.colortex.cn

crontab -e;  crontab -l
来源：http://lo.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://wk.asd995.cn

openssl rand -hex 16
来源：http://xo.huixiangedu.cn

[R68] 计算文件校验值
来源：http://gq.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gc.lnxyls.cn

[R69] 生成随机密码
来源：http://po.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://rz.bjjhwx.cn

[R70] 时间戳与互转
来源：http://ki.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://et.jctech888.com.cn

[R71] 日期格式化
来源：http://oa.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ws.gzmigu.cn

[R72] 等待端口就绪
来源：http://ke.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vl.muxihuayi.cn

[R73] 分割大日志
来源：http://gr.shtwfgs.cn

split -l 1000 big.log part_
来源：http://fe.jianghongdianzi.cn

[R74] 批量重命名
来源：http://xv.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qi.jctech888.com.cn

[R75] 导出环境变量
来源：http://ge.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://iu.yuexingan06.cn

[R76] 使用临时文件
来源：http://vh.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sw.nicolike.cn

[R77] 读取用户输入
来源：http://mm.yuexingan06.cn

read -rp "请输入: " ans
来源：http://fq.shxzskj.cn

[R78] 交互式菜单
来源：http://rr.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jl.haigaiapp.cn

[R79] 解析命令行选项
来源：http://zr.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wg.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://si.shxzukj.cn

time ./run.sh
来源：http://jg.yuexingan06.cn

================================================================================
来源：http://xs.newstarts.cn

S. C / C++ 专题
来源：http://nc.9csxet.cn

================================================================================
来源：http://wt.shtwfgs.cn

[S01] C：Hello World
来源：http://eq.wgjwhj.cn

#include <stdio.h>
来源：http://jr.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vs.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://iz.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://ey.huixinmuqiang.cn

[S03] C：读入整数
来源：http://yg.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://zd.nszjky.cn

[S04] C：字符串复制
来源：http://qz.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qt.huanxung.cn

[S05] C：字符串长度
来源：http://df.szxytkj.cn

strlen(s)
来源：http://tp.yuexingan06.cn

[S06] C：字符串比较
来源：http://vg.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://ya.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://sb.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yo.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://vo.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kl.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://sa.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xz.yuexingan06.cn

[S10] C：指针与解引用
来源：http://pb.nicolike.cn

int *p = &a;  *p = 5;
来源：http://gz.huixiangedu.cn

[S11] C：逐行读文件
来源：http://it.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://kl.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lv.newstarts.cn

fclose(f);
来源：http://qf.wgjwhj.cn

[S12] C：写文件
来源：http://oo.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://du.yuexingan06.cn

[S13] C：宏定义
来源：http://yy.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dr.bookmarksfly.cn

[S14] C：枚举
来源：http://ha.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://fi.9csxet.cn

[S15] C：类型转换
来源：http://zd.huanxung.cn

(double) a / b
来源：http://qr.asd995.cn

[S16] C：位操作置位
来源：http://gg.newstarts.cn

x |= (1 << 3);
来源：http://lt.nicolike.cn

[S17] C：安全拼接字符串
来源：http://jh.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vi.huixiangedu.cn

[S18] C：命令行参数
来源：http://ys.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://dl.huixiangedu.cn

[S19] C：快速排序
来源：http://nm.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cr.asd995.cn

[S20] C：二分查找
来源：http://jc.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tl.haigaiapp.cn

[S21] C：字符类别判断
来源：http://xk.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hq.lnxyls.cn

[S22] C：字符串转数字
来源：http://rb.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oc.szxytkj.cn

[S23] C：随机数
来源：http://am.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bt.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://kf.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gc.chemitech.net.cn

[S25] C：内存拷贝
来源：http://pw.gzmigu.cn

memcpy(dst, src, n);
来源：http://jp.521024.cn

[S26] C：内存清零
来源：http://hn.huanxung.cn

memset(a, 0, sizeof a);
来源：http://aj.colortex.cn

[S27] C：定义常量
来源：http://cf.chemitech.net.cn

const double PI = 3.14159;
来源：http://lm.huixinmuqiang.cn

[S28] C：静态变量
来源：http://mt.muxihuayi.cn


<!-- 参考信息 -->