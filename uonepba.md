代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ch.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://hn.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xc.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tb.chemitech.net.cn

[Q61] 移动平均
来源：http://ib.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rc.jianghongdianzi.cn

[Q62] 分组占比
来源：http://at.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ol.yuntaijiaju.cn

[Q63] 开启事务
来源：http://pz.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yi.hahajie.cn

[Q64] 提交事务
来源：http://uu.huixiangedu.cn

COMMIT;
来源：http://wd.bjjhwx.cn

[Q65] 回滚事务
来源：http://vo.shxzukj.cn

ROLLBACK;
来源：http://yp.haigaiapp.cn

[Q66] 行锁查询
来源：http://jk.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gr.nicolike.cn

[Q67] 设置隔离级别
来源：http://xs.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oa.chemitech.net.cn

[Q68] 保存点
来源：http://im.hnjuh.cn

SAVEPOINT sp1;
来源：http://ux.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://ik.wgjwhj.cn

[Q69] 查看执行计划
来源：http://qy.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://id.newstarts.cn

[Q70] 更新统计信息
来源：http://ou.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://rn.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://le.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ts.bookmarksfly.cn

[Q72] 查看索引
来源：http://ol.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://ah.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://ov.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wd.wgjwhj.cn

[Q74] 强制使用索引
来源：http://bt.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hy.asd995.cn

[Q75] 日期格式化
来源：http://bg.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://th.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lv.jctech888.com.cn

[Q76] 按天统计
来源：http://vi.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lq.jianghongdianzi.cn

[Q77] 时间加减
来源：http://oi.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pf.hahajie.cn

[Q78] 当前时间
来源：http://bm.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fn.gzmigu.cn

[Q79] 字符串拼接
来源：http://jy.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ng.nicolike.cn

[Q80] 字符串截取
来源：http://hy.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pv.haigaiapp.cn

[Q81] 字符串替换
来源：http://or.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xi.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://zo.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qx.9csxet.cn

[Q83] 大小写转换
来源：http://be.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wm.nszjky.cn

[Q84] 去除首尾空格
来源：http://ax.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://fs.shxzukj.cn

[Q85] 数值取整
来源：http://ax.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aj.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://qt.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cq.newstarts.cn

[Q87] JSON 字段做条件
来源：http://ym.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yj.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://cs.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dg.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://we.hnjuh.cn

[Q89] 判断表是否存在
来源：http://za.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gt.lnxyls.cn

[Q90] 生成序号列
来源：http://rk.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cv.szsharing.cn

================================================================================
来源：http://qe.jianghongdianzi.cn

R. Bash 专题
来源：http://rv.gzmigu.cn

================================================================================
来源：http://gc.colortex.cn

[R01] shebang 与严格模式
来源：http://jr.lnxyls.cn

#!/usr/bin/env bash
来源：http://qu.jianghongdianzi.cn

set -euo pipefail
来源：http://fc.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://aa.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://vp.hnjuh.cn

[R03] 只读变量
来源：http://zh.bjjhwx.cn

readonly PI=3.14
来源：http://mu.haigaiapp.cn

[R04] 位置参数
来源：http://sf.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xh.wgjwhj.cn

[R05] 参数默认值
来源：http://km.huixiangedu.cn

name="${1:-default}"
来源：http://wg.hnjuh.cn

[R06] 判断命令是否存在
来源：http://qi.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yk.huixiangedu.cn

[R07] if 判断文件
来源：http://px.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hs.newstarts.cn

[R08] 数值比较
来源：http://fz.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mg.szxytkj.cn

[R09] 字符串比较
来源：http://fd.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bt.yuntaijiaju.cn

[R10] 正则匹配
来源：http://sn.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sz.asd995.cn

[R11] case 多分支
来源：http://zb.yuexingan06.cn

case "$1" in
来源：http://un.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://xa.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://la.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://uz.lnxyls.cn

esac
来源：http://cu.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://oy.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://cx.szsharing.cn

[R13] for 计数循环
来源：http://ad.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://no.szxytkj.cn

[R14] C 风格 for
来源：http://po.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cy.newstarts.cn

[R15] while 逐行读文件
来源：http://sl.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ur.jianghongdianzi.cn

[R16] until 等待条件
来源：http://qx.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fl.huixiangedu.cn

[R17] 数组定义与取值
来源：http://tl.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gc.nicolike.cn

[R18] 遍历数组
来源：http://qw.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yf.hahajie.cn

[R19] 数组长度
来源：http://jg.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://ik.szxytkj.cn

[R20] 关联数组（字典）
来源：http://vc.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hs.newstarts.cn

[R21] 字符串长度
来源：http://uw.hahajie.cn

echo "${#s}"
来源：http://st.huixinmuqiang.cn

[R22] 截取子串
来源：http://jb.panjiajie.cn

echo "${s:0:5}"
来源：http://er.hahajie.cn

[R23] 字符串替换
来源：http://dl.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kz.nszjky.cn

[R24] 大小写转换
来源：http://cf.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kr.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://ex.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sq.wgjwhj.cn

[R26] 命令替换
来源：http://lj.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://ax.panjiajie.cn

[R27] 算术展开
来源：http://pq.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://zw.hahajie.cn

[R28] 浮点运算
来源：http://hv.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://ho.jianghongdianzi.cn

[R29] 定义函数
来源：http://uu.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cp.muxihuayi.cn

[R30] 函数返回状态码
来源：http://cc.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://bz.521024.cn

[R31] 局部变量
来源：http://gb.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://fu.bjjhwx.cn

[R32] 参数个数校验
来源：http://gu.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wg.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://vu.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kj.panjiajie.cn

[R34] 退出时清理
来源：http://py.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eu.muxihuayi.cn

[R35] 后台执行并等待
来源：http://ts.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fw.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://pc.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bo.shxzskj.cn

[R37] 把输出赋给变量
来源：http://sq.huixinmuqiang.cn

files=$(ls -1)
来源：http://kc.bookmarksfly.cn

[R38] 管道串联
来源：http://zj.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://et.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://dn.haigaiapp.cn

cmd > out.log 2>&1
来源：http://rr.lnxyls.cn

[R40] 追加写日志
来源：http://dm.muxihuayi.cn

echo "log" >> out.log
来源：http://qt.gzmigu.cn

[R41] 丢弃输出
来源：http://yw.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://hx.huixiangedu.cn

[R42] 输入重定向
来源：http://wr.bookmarksfly.cn

wc -l < a.txt
来源：http://ev.hahajie.cn

[R43] 按名字查找文件
来源：http://pf.521024.cn

find . -name "*.log" -type f
来源：http://na.panjiajie.cn

[R44] 按修改时间查找
来源：http://ut.muxihuayi.cn

find . -mtime -7 -type f
来源：http://xu.huixinmuqiang.cn

[R45] 批量删除
来源：http://ra.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://gh.huanxung.cn

[R46] 递归替换文件内容
来源：http://jd.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vn.jctech888.com.cn

[R47] sed 单行替换
来源：http://dc.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tf.colortex.cn

[R48] awk 取指定列
来源：http://gt.521024.cn

awk '{print $1, $3}' a.txt
来源：http://wq.colortex.cn

[R49] awk 带条件
来源：http://cv.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aw.shxzskj.cn

[R50] awk 求和
来源：http://dm.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ra.newstarts.cn

[R51] 排序去重取前几
来源：http://ik.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dx.bookmarksfly.cn

[R52] 统计行数
来源：http://mo.lnxyls.cn

wc -l a.txt
来源：http://xy.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://jp.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://al.hahajie.cn

[R54] 比较两个文件
来源：http://wt.shxzukj.cn

diff a.txt b.txt
来源：http://ak.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://fp.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bz.shtwfgs.cn

[R56] 远程拷贝
来源：http://ks.asd995.cn

scp file user@host:/path/
来源：http://sd.colortex.cn

[R57] 远程执行命令
来源：http://op.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://zt.muxihuayi.cn

[R58] 下载文件
来源：http://yd.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lq.nszjky.cn

[R59] 发 POST JSON
来源：http://lx.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oh.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://we.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fz.asd995.cn

[R61] 磁盘占用
来源：http://cj.chemitech.net.cn

df -h;  du -sh *
来源：http://vz.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://bu.521024.cn

du -ah . | sort -rh | head -10
来源：http://rl.wgjwhj.cn

[R63] 内存与进程
来源：http://vy.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://jw.haigaiapp.cn

[R64] 结束进程
来源：http://cr.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://ka.newstarts.cn

[R65] 查看端口占用
来源：http://vu.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gm.shxzukj.cn

[R66] 定时任务
来源：http://td.gzmigu.cn

crontab -e;  crontab -l
来源：http://it.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://zj.szxytkj.cn

openssl rand -hex 16
来源：http://pc.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://ms.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pi.huanxung.cn

[R69] 生成随机密码
来源：http://qg.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://su.lnxyls.cn

[R70] 时间戳与互转
来源：http://qp.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://mr.panjiajie.cn

[R71] 日期格式化
来源：http://ww.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qi.yuexingan06.cn

[R72] 等待端口就绪
来源：http://qk.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fo.haigaiapp.cn

[R73] 分割大日志
来源：http://gb.hahajie.cn

split -l 1000 big.log part_
来源：http://wt.muxihuayi.cn

[R74] 批量重命名
来源：http://xv.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eq.shtwfgs.cn

[R75] 导出环境变量
来源：http://um.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://nm.asd995.cn

[R76] 使用临时文件
来源：http://kb.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pt.chemitech.net.cn

[R77] 读取用户输入
来源：http://xt.szxytkj.cn

read -rp "请输入: " ans
来源：http://ia.shxzskj.cn

[R78] 交互式菜单
来源：http://cg.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ot.muxihuayi.cn

[R79] 解析命令行选项
来源：http://cq.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://if.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://td.haigaiapp.cn

time ./run.sh
来源：http://wf.521024.cn

================================================================================
来源：http://ob.521024.cn

S. C / C++ 专题
来源：http://qz.9csxet.cn

================================================================================
来源：http://kk.huixinmuqiang.cn

[S01] C：Hello World
来源：http://hz.asd995.cn

#include <stdio.h>
来源：http://ot.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wh.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://ab.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://hf.nszjky.cn

[S03] C：读入整数
来源：http://pj.hnjuh.cn

int x; scanf("%d", &x);
来源：http://ni.yuexingan06.cn

[S04] C：字符串复制
来源：http://eo.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cj.colortex.cn

[S05] C：字符串长度
来源：http://xh.szxytkj.cn

strlen(s)
来源：http://mp.szxytkj.cn

[S06] C：字符串比较
来源：http://ek.521024.cn

strcmp(a, b) == 0
来源：http://xp.hahajie.cn

[S07] C：数组遍历求和
来源：http://df.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ps.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://ry.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tj.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://nk.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ab.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://br.asd995.cn

int *p = &a;  *p = 5;
来源：http://qq.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://em.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://sk.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zi.9csxet.cn

fclose(f);
来源：http://lw.jctech888.com.cn

[S12] C：写文件
来源：http://xi.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nu.szxytkj.cn

[S13] C：宏定义
来源：http://rz.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ey.yuexingan06.cn

[S14] C：枚举
来源：http://wj.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://pj.nszjky.cn

[S15] C：类型转换
来源：http://xn.nszjky.cn

(double) a / b
来源：http://ix.huixiangedu.cn

[S16] C：位操作置位
来源：http://nk.bookmarksfly.cn

x |= (1 << 3);
来源：http://wq.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://ti.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dd.chemitech.net.cn

[S18] C：命令行参数
来源：http://tg.szxytkj.cn

int main(int argc, char **argv)
来源：http://jl.9csxet.cn

[S19] C：快速排序
来源：http://fu.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zb.nszjky.cn

[S20] C：二分查找
来源：http://ww.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jz.szsharing.cn

[S21] C：字符类别判断
来源：http://bv.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yc.panjiajie.cn

[S22] C：字符串转数字
来源：http://vf.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ox.colortex.cn

[S23] C：随机数
来源：http://te.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fe.newstarts.cn

[S24] C：获取本地时间
来源：http://yh.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ma.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://gu.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://pn.jianghongdianzi.cn

[S26] C：内存清零
来源：http://kx.newstarts.cn

memset(a, 0, sizeof a);
来源：http://as.newstarts.cn

[S27] C：定义常量
来源：http://vu.szsharing.cn

const double PI = 3.14159;
来源：http://mc.hnjuh.cn

[S28] C：静态变量
来源：http://ko.colortex.cn

static int counter = 0;
来源：http://fv.szxytkj.cn

[S29] C：变参函数
来源：http://xn.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fm.wgjwhj.cn

[S30] C：头文件保护
来源：http://vg.colortex.cn


<!-- 参考信息 -->