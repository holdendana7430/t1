代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dn.panjiajie.cn

[Q58] 累计求和
来源：http://xn.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://em.bookmarksfly.cn

[Q59] 分组内累计
来源：http://if.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bo.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://ev.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ye.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ix.jctech888.com.cn

[Q61] 移动平均
来源：http://el.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ef.bjjhwx.cn

[Q62] 分组占比
来源：http://uc.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wu.9csxet.cn

[Q63] 开启事务
来源：http://fv.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gf.nszjky.cn

[Q64] 提交事务
来源：http://pg.colortex.cn

COMMIT;
来源：http://hl.huanxung.cn

[Q65] 回滚事务
来源：http://ze.shxzukj.cn

ROLLBACK;
来源：http://px.asd995.cn

[Q66] 行锁查询
来源：http://fu.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uk.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://lw.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://av.haigaiapp.cn

[Q68] 保存点
来源：http://pw.wgjwhj.cn

SAVEPOINT sp1;
来源：http://kh.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://ft.szxytkj.cn

[Q69] 查看执行计划
来源：http://jo.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ls.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://lu.bjjhwx.cn

ANALYZE TABLE users;
来源：http://nk.newstarts.cn

[Q71] 查看建表语句
来源：http://lm.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sd.gzmigu.cn

[Q72] 查看索引
来源：http://wt.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://vw.lnxyls.cn

[Q73] 查看表状态
来源：http://ta.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ga.nszjky.cn

[Q74] 强制使用索引
来源：http://jm.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qn.lnxyls.cn

[Q75] 日期格式化
来源：http://kf.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://og.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ax.asd995.cn

[Q76] 按天统计
来源：http://wj.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fx.szxytkj.cn

[Q77] 时间加减
来源：http://js.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qw.asd995.cn

[Q78] 当前时间
来源：http://us.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ke.szsharing.cn

[Q79] 字符串拼接
来源：http://jy.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ac.haigaiapp.cn

[Q80] 字符串截取
来源：http://cp.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vw.bookmarksfly.cn

[Q81] 字符串替换
来源：http://ve.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wk.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://ot.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mm.newstarts.cn

[Q83] 大小写转换
来源：http://kx.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cg.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://rv.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://ai.bookmarksfly.cn

[Q85] 数值取整
来源：http://hs.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://js.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://qn.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vx.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://ad.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mv.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://ao.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xa.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wv.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://bc.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ga.nszjky.cn

[Q90] 生成序号列
来源：http://qo.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xj.shxzukj.cn

================================================================================
来源：http://uy.huixinmuqiang.cn

R. Bash 专题
来源：http://la.haigaiapp.cn

================================================================================
来源：http://no.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://fw.yuexingan06.cn

#!/usr/bin/env bash
来源：http://wm.yuntaijiaju.cn

set -euo pipefail
来源：http://ob.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://cx.szxytkj.cn

name="Tom"; echo "$name"
来源：http://vh.hahajie.cn

[R03] 只读变量
来源：http://ya.szxytkj.cn

readonly PI=3.14
来源：http://ju.newstarts.cn

[R04] 位置参数
来源：http://rv.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qf.nicolike.cn

[R05] 参数默认值
来源：http://gu.shxzukj.cn

name="${1:-default}"
来源：http://sy.hnjuh.cn

[R06] 判断命令是否存在
来源：http://lx.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ta.szxytkj.cn

[R07] if 判断文件
来源：http://dg.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bk.bookmarksfly.cn

[R08] 数值比较
来源：http://pp.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zo.521024.cn

[R09] 字符串比较
来源：http://lo.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dc.521024.cn

[R10] 正则匹配
来源：http://qw.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ko.521024.cn

[R11] case 多分支
来源：http://vs.huanxung.cn

case "$1" in
来源：http://is.haigaiapp.cn

start) echo "启动" ;;
来源：http://ho.lnxyls.cn

stop)  echo "停止" ;;
来源：http://nz.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://om.bookmarksfly.cn

esac
来源：http://sb.huanxung.cn

[R12] for 遍历文件
来源：http://us.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://mh.shxzskj.cn

[R13] for 计数循环
来源：http://bx.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://ts.muxihuayi.cn

[R14] C 风格 for
来源：http://si.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mc.hnjuh.cn

[R15] while 逐行读文件
来源：http://vi.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://of.huixiangedu.cn

[R16] until 等待条件
来源：http://iv.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fz.asd995.cn

[R17] 数组定义与取值
来源：http://gz.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qf.hnjuh.cn

[R18] 遍历数组
来源：http://mw.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ay.yuexingan06.cn

[R19] 数组长度
来源：http://zz.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://ko.gzmigu.cn

[R20] 关联数组（字典）
来源：http://hn.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xg.jctech888.com.cn

[R21] 字符串长度
来源：http://at.haigaiapp.cn

echo "${#s}"
来源：http://em.yuexingan06.cn

[R22] 截取子串
来源：http://ep.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://pt.huixinmuqiang.cn

[R23] 字符串替换
来源：http://bh.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cm.jianghongdianzi.cn

[R24] 大小写转换
来源：http://nk.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uy.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://fn.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wr.nicolike.cn

[R26] 命令替换
来源：http://lz.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://pv.yuntaijiaju.cn

[R27] 算术展开
来源：http://ff.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://rg.yuexingan06.cn

[R28] 浮点运算
来源：http://sv.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://tf.lnxyls.cn

[R29] 定义函数
来源：http://cx.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kx.huixiangedu.cn

[R30] 函数返回状态码
来源：http://pf.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://js.newstarts.cn

[R31] 局部变量
来源：http://ot.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://sj.colortex.cn

[R32] 参数个数校验
来源：http://yx.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oa.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://ud.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pv.521024.cn

[R34] 退出时清理
来源：http://uo.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ns.jctech888.com.cn

[R35] 后台执行并等待
来源：http://qf.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qf.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://xa.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ok.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://kt.huanxung.cn

files=$(ls -1)
来源：http://cw.panjiajie.cn

[R38] 管道串联
来源：http://il.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://rf.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://bt.9csxet.cn

cmd > out.log 2>&1
来源：http://sj.9csxet.cn

[R40] 追加写日志
来源：http://du.muxihuayi.cn

echo "log" >> out.log
来源：http://va.nszjky.cn

[R41] 丢弃输出
来源：http://pz.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://hm.bookmarksfly.cn

[R42] 输入重定向
来源：http://qo.huixinmuqiang.cn

wc -l < a.txt
来源：http://de.hnjuh.cn

[R43] 按名字查找文件
来源：http://zo.haigaiapp.cn

find . -name "*.log" -type f
来源：http://or.jctech888.com.cn

[R44] 按修改时间查找
来源：http://tw.jctech888.com.cn

find . -mtime -7 -type f
来源：http://oi.yuexingan06.cn

[R45] 批量删除
来源：http://gc.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://wv.panjiajie.cn

[R46] 递归替换文件内容
来源：http://er.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lh.haigaiapp.cn

[R47] sed 单行替换
来源：http://df.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qc.colortex.cn

[R48] awk 取指定列
来源：http://ez.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://hd.colortex.cn

[R49] awk 带条件
来源：http://ej.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rp.9csxet.cn

[R50] awk 求和
来源：http://od.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ug.muxihuayi.cn

[R51] 排序去重取前几
来源：http://lp.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://el.hnjuh.cn

[R52] 统计行数
来源：http://cq.szxytkj.cn

wc -l a.txt
来源：http://cw.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://zp.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://at.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://hb.huixiangedu.cn

diff a.txt b.txt
来源：http://lb.nicolike.cn

[R55] 压缩与解压
来源：http://yj.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tk.muxihuayi.cn

[R56] 远程拷贝
来源：http://wt.9csxet.cn

scp file user@host:/path/
来源：http://rm.yuexingan06.cn

[R57] 远程执行命令
来源：http://tf.nicolike.cn

ssh user@host 'uptime'
来源：http://gi.shtwfgs.cn

[R58] 下载文件
来源：http://xb.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qe.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://js.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ui.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://gp.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nj.shxzukj.cn

[R61] 磁盘占用
来源：http://co.szxytkj.cn

df -h;  du -sh *
来源：http://uw.asd995.cn

[R62] 找最占空间的文件
来源：http://aj.colortex.cn

du -ah . | sort -rh | head -10
来源：http://vg.asd995.cn

[R63] 内存与进程
来源：http://ac.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://uq.521024.cn

[R64] 结束进程
来源：http://qf.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://xy.yuexingan06.cn

[R65] 查看端口占用
来源：http://dc.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sd.9csxet.cn

[R66] 定时任务
来源：http://hb.gzmigu.cn

crontab -e;  crontab -l
来源：http://zd.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://nu.szxytkj.cn

openssl rand -hex 16
来源：http://fy.hahajie.cn

[R68] 计算文件校验值
来源：http://wf.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qo.shxzskj.cn

[R69] 生成随机密码
来源：http://mk.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://hj.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://yx.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://hf.newstarts.cn

[R71] 日期格式化
来源：http://cy.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://if.chemitech.net.cn

[R72] 等待端口就绪
来源：http://hn.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://br.huixinmuqiang.cn

[R73] 分割大日志
来源：http://fx.yuexingan06.cn

split -l 1000 big.log part_
来源：http://cf.szsharing.cn

[R74] 批量重命名
来源：http://gf.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wq.wgjwhj.cn

[R75] 导出环境变量
来源：http://eg.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://lz.huanxung.cn

[R76] 使用临时文件
来源：http://ia.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tm.hnjuh.cn

[R77] 读取用户输入
来源：http://ur.hnjuh.cn

read -rp "请输入: " ans
来源：http://fq.yuexingan06.cn

[R78] 交互式菜单
来源：http://ju.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vx.bjjhwx.cn

[R79] 解析命令行选项
来源：http://ha.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ws.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://ev.colortex.cn

time ./run.sh
来源：http://ld.hahajie.cn

================================================================================
来源：http://ni.shxzukj.cn

S. C / C++ 专题
来源：http://vv.shxzukj.cn

================================================================================
来源：http://lv.panjiajie.cn

[S01] C：Hello World
来源：http://hc.nicolike.cn

#include <stdio.h>
来源：http://kt.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eb.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://cy.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://qq.jianghongdianzi.cn

[S03] C：读入整数
来源：http://sx.newstarts.cn

int x; scanf("%d", &x);
来源：http://da.colortex.cn

[S04] C：字符串复制
来源：http://qe.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ng.muxihuayi.cn

[S05] C：字符串长度
来源：http://it.hnjuh.cn

strlen(s)
来源：http://ua.huixiangedu.cn

[S06] C：字符串比较
来源：http://ov.shtwfgs.cn

strcmp(a, b) == 0
来源：http://he.szxytkj.cn

[S07] C：数组遍历求和
来源：http://ki.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xn.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://fz.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kq.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://xq.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eu.newstarts.cn

[S10] C：指针与解引用
来源：http://ep.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://kg.szsharing.cn

[S11] C：逐行读文件
来源：http://zd.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://cv.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ip.gzmigu.cn

fclose(f);
来源：http://xr.wgjwhj.cn

[S12] C：写文件
来源：http://ir.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fp.yuntaijiaju.cn

[S13] C：宏定义
来源：http://pd.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pr.9csxet.cn

[S14] C：枚举
来源：http://fl.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://yt.hnjuh.cn

[S15] C：类型转换
来源：http://an.panjiajie.cn

(double) a / b
来源：http://tc.szsharing.cn

[S16] C：位操作置位
来源：http://cw.jctech888.com.cn

x |= (1 << 3);
来源：http://oj.asd995.cn

[S17] C：安全拼接字符串
来源：http://vi.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dm.nszjky.cn

[S18] C：命令行参数
来源：http://pa.shxzskj.cn

int main(int argc, char **argv)
来源：http://kl.521024.cn

[S19] C：快速排序
来源：http://hr.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hb.gzmigu.cn

[S20] C：二分查找
来源：http://sz.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://si.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://sk.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qn.huixiangedu.cn

[S22] C：字符串转数字
来源：http://ur.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tx.nicolike.cn

[S23] C：随机数
来源：http://qt.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hh.lnxyls.cn

[S24] C：获取本地时间
来源：http://ca.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uq.muxihuayi.cn

[S25] C：内存拷贝
来源：http://yg.521024.cn

memcpy(dst, src, n);
来源：http://iy.jianghongdianzi.cn

[S26] C：内存清零
来源：http://nz.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://ch.lnxyls.cn

[S27] C：定义常量
来源：http://fq.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://ti.lnxyls.cn

[S28] C：静态变量
来源：http://hr.newstarts.cn


<!-- 参考信息 -->