代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lv.huixiangedu.cn

[Q58] 累计求和
来源：http://ae.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wh.huanxung.cn

[Q59] 分组内累计
来源：http://nv.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lz.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://jw.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://so.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://go.asd995.cn

[Q61] 移动平均
来源：http://rc.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xu.newstarts.cn

[Q62] 分组占比
来源：http://uf.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nu.huixiangedu.cn

[Q63] 开启事务
来源：http://cm.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wc.521024.cn

[Q64] 提交事务
来源：http://uk.shxzukj.cn

COMMIT;
来源：http://lb.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://hz.shxzskj.cn

ROLLBACK;
来源：http://nz.gzmigu.cn

[Q66] 行锁查询
来源：http://ff.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pv.asd995.cn

[Q67] 设置隔离级别
来源：http://yh.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vk.hnjuh.cn

[Q68] 保存点
来源：http://sm.hahajie.cn

SAVEPOINT sp1;
来源：http://rq.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://vh.521024.cn

[Q69] 查看执行计划
来源：http://jf.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vm.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://rf.wgjwhj.cn

ANALYZE TABLE users;
来源：http://mk.haigaiapp.cn

[Q71] 查看建表语句
来源：http://aa.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://to.szsharing.cn

[Q72] 查看索引
来源：http://qo.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://rr.haigaiapp.cn

[Q73] 查看表状态
来源：http://lc.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://je.521024.cn

[Q74] 强制使用索引
来源：http://sq.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ea.9csxet.cn

[Q75] 日期格式化
来源：http://ya.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lf.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cr.shxzukj.cn

[Q76] 按天统计
来源：http://hu.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ym.asd995.cn

[Q77] 时间加减
来源：http://ys.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://km.bookmarksfly.cn

[Q78] 当前时间
来源：http://bo.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ee.hahajie.cn

[Q79] 字符串拼接
来源：http://ff.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ql.szxytkj.cn

[Q80] 字符串截取
来源：http://sf.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lb.9csxet.cn

[Q81] 字符串替换
来源：http://yl.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lf.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://pc.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ed.hnjuh.cn

[Q83] 大小写转换
来源：http://rk.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pi.huanxung.cn

[Q84] 去除首尾空格
来源：http://fj.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://vv.huixiangedu.cn

[Q85] 数值取整
来源：http://gu.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dq.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://su.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hq.huanxung.cn

[Q87] JSON 字段做条件
来源：http://fk.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tn.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://ym.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yu.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ep.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://fq.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pj.nszjky.cn

[Q90] 生成序号列
来源：http://jx.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gm.jctech888.com.cn

================================================================================
来源：http://bo.muxihuayi.cn

R. Bash 专题
来源：http://ai.huixiangedu.cn

================================================================================
来源：http://qd.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://ry.huixiangedu.cn

#!/usr/bin/env bash
来源：http://xe.gzmigu.cn

set -euo pipefail
来源：http://gi.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://hq.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://kd.hnjuh.cn

[R03] 只读变量
来源：http://kt.bookmarksfly.cn

readonly PI=3.14
来源：http://uy.lnxyls.cn

[R04] 位置参数
来源：http://hz.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yk.colortex.cn

[R05] 参数默认值
来源：http://kk.521024.cn

name="${1:-default}"
来源：http://ln.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://fs.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xk.muxihuayi.cn

[R07] if 判断文件
来源：http://pp.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ne.huixinmuqiang.cn

[R08] 数值比较
来源：http://vx.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dv.yuntaijiaju.cn

[R09] 字符串比较
来源：http://di.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://st.shxzukj.cn

[R10] 正则匹配
来源：http://qn.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lw.colortex.cn

[R11] case 多分支
来源：http://rj.nszjky.cn

case "$1" in
来源：http://lm.nicolike.cn

start) echo "启动" ;;
来源：http://pm.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://yb.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://yn.jctech888.com.cn

esac
来源：http://fo.colortex.cn

[R12] for 遍历文件
来源：http://xj.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://ea.bjjhwx.cn

[R13] for 计数循环
来源：http://vd.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://fn.szsharing.cn

[R14] C 风格 for
来源：http://yg.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://st.wgjwhj.cn

[R15] while 逐行读文件
来源：http://ss.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xc.jianghongdianzi.cn

[R16] until 等待条件
来源：http://jc.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yi.szxytkj.cn

[R17] 数组定义与取值
来源：http://yg.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uo.szsharing.cn

[R18] 遍历数组
来源：http://sx.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hx.yuntaijiaju.cn

[R19] 数组长度
来源：http://xk.szxytkj.cn

echo "${#arr[@]}"
来源：http://tu.hnjuh.cn

[R20] 关联数组（字典）
来源：http://io.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fp.yuexingan06.cn

[R21] 字符串长度
来源：http://fd.521024.cn

echo "${#s}"
来源：http://xr.nicolike.cn

[R22] 截取子串
来源：http://xt.bookmarksfly.cn

echo "${s:0:5}"
来源：http://ui.hnjuh.cn

[R23] 字符串替换
来源：http://hy.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bw.hahajie.cn

[R24] 大小写转换
来源：http://tt.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sc.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://dz.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ds.jianghongdianzi.cn

[R26] 命令替换
来源：http://vg.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://fb.huixinmuqiang.cn

[R27] 算术展开
来源：http://ps.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://oz.nicolike.cn

[R28] 浮点运算
来源：http://ey.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://qt.szsharing.cn

[R29] 定义函数
来源：http://pp.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vw.hahajie.cn

[R30] 函数返回状态码
来源：http://ms.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://oe.wgjwhj.cn

[R31] 局部变量
来源：http://zi.521024.cn

f() { local x=1; echo "$x"; }
来源：http://vb.nszjky.cn

[R32] 参数个数校验
来源：http://pt.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vu.asd995.cn

[R33] 捕获错误并提示行号
来源：http://qx.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fr.chemitech.net.cn

[R34] 退出时清理
来源：http://uo.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pa.newstarts.cn

[R35] 后台执行并等待
来源：http://ms.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ei.szxytkj.cn

[R36] 并发执行多个任务
来源：http://du.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pt.colortex.cn

[R37] 把输出赋给变量
来源：http://nm.jianghongdianzi.cn

files=$(ls -1)
来源：http://ql.hahajie.cn

[R38] 管道串联
来源：http://yj.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://sm.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://fw.yuexingan06.cn

cmd > out.log 2>&1
来源：http://iq.huixinmuqiang.cn

[R40] 追加写日志
来源：http://kc.huixinmuqiang.cn

echo "log" >> out.log
来源：http://gt.huanxung.cn

[R41] 丢弃输出
来源：http://hz.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://cz.szxytkj.cn

[R42] 输入重定向
来源：http://pl.szsharing.cn

wc -l < a.txt
来源：http://qy.shxzukj.cn

[R43] 按名字查找文件
来源：http://va.szsharing.cn

find . -name "*.log" -type f
来源：http://qz.nszjky.cn

[R44] 按修改时间查找
来源：http://wq.newstarts.cn

find . -mtime -7 -type f
来源：http://dg.shxzukj.cn

[R45] 批量删除
来源：http://xq.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://mi.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://qg.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nr.chemitech.net.cn

[R47] sed 单行替换
来源：http://av.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wf.colortex.cn

[R48] awk 取指定列
来源：http://yj.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://gd.hnjuh.cn

[R49] awk 带条件
来源：http://fw.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gc.hnjuh.cn

[R50] awk 求和
来源：http://qx.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fk.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://yl.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gh.huanxung.cn

[R52] 统计行数
来源：http://fc.nicolike.cn

wc -l a.txt
来源：http://ta.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://ry.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sb.newstarts.cn

[R54] 比较两个文件
来源：http://id.hahajie.cn

diff a.txt b.txt
来源：http://jj.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://nq.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qk.bjjhwx.cn

[R56] 远程拷贝
来源：http://lk.hahajie.cn

scp file user@host:/path/
来源：http://zo.colortex.cn

[R57] 远程执行命令
来源：http://de.shxzskj.cn

ssh user@host 'uptime'
来源：http://gz.jianghongdianzi.cn

[R58] 下载文件
来源：http://zf.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://us.yuexingan06.cn

[R59] 发 POST JSON
来源：http://me.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rr.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://dt.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fi.shtwfgs.cn

[R61] 磁盘占用
来源：http://ck.shtwfgs.cn

df -h;  du -sh *
来源：http://uo.szsharing.cn

[R62] 找最占空间的文件
来源：http://ux.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://pz.newstarts.cn

[R63] 内存与进程
来源：http://xo.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://eb.szsharing.cn

[R64] 结束进程
来源：http://pq.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://pu.wgjwhj.cn

[R65] 查看端口占用
来源：http://rl.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oa.colortex.cn

[R66] 定时任务
来源：http://to.szxytkj.cn

crontab -e;  crontab -l
来源：http://no.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://hn.haigaiapp.cn

openssl rand -hex 16
来源：http://jr.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://an.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ow.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://vr.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://vo.szsharing.cn

[R70] 时间戳与互转
来源：http://yr.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://ag.huanxung.cn

[R71] 日期格式化
来源：http://mk.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hy.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://ig.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jz.shxzskj.cn

[R73] 分割大日志
来源：http://gt.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://og.yuntaijiaju.cn

[R74] 批量重命名
来源：http://el.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://it.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://to.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://ta.shtwfgs.cn

[R76] 使用临时文件
来源：http://tp.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ei.jctech888.com.cn

[R77] 读取用户输入
来源：http://vf.hahajie.cn

read -rp "请输入: " ans
来源：http://mp.szsharing.cn

[R78] 交互式菜单
来源：http://bp.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ys.huanxung.cn

[R79] 解析命令行选项
来源：http://so.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yz.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://je.newstarts.cn

time ./run.sh
来源：http://zw.wgjwhj.cn

================================================================================
来源：http://vl.huixiangedu.cn

S. C / C++ 专题
来源：http://qi.huixinmuqiang.cn

================================================================================
来源：http://sc.shxzukj.cn

[S01] C：Hello World
来源：http://rh.lnxyls.cn

#include <stdio.h>
来源：http://ui.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ls.colortex.cn

[S02] C：变量与格式化输出
来源：http://nc.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://cv.szxytkj.cn

[S03] C：读入整数
来源：http://zx.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://hp.nicolike.cn

[S04] C：字符串复制
来源：http://pe.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cz.hnjuh.cn

[S05] C：字符串长度
来源：http://iy.shtwfgs.cn

strlen(s)
来源：http://dy.9csxet.cn

[S06] C：字符串比较
来源：http://yh.gzmigu.cn

strcmp(a, b) == 0
来源：http://zt.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://gu.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rq.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://to.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rh.521024.cn

[S09] C：结构体定义与初始化
来源：http://no.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qx.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://hj.hahajie.cn

int *p = &a;  *p = 5;
来源：http://fo.szxytkj.cn

[S11] C：逐行读文件
来源：http://gh.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://mp.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ky.nszjky.cn

fclose(f);
来源：http://sc.hahajie.cn

[S12] C：写文件
来源：http://jb.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jv.nszjky.cn

[S13] C：宏定义
来源：http://sd.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ev.hnjuh.cn

[S14] C：枚举
来源：http://yi.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://ml.bjjhwx.cn

[S15] C：类型转换
来源：http://xm.asd995.cn

(double) a / b
来源：http://ud.bjjhwx.cn

[S16] C：位操作置位
来源：http://jz.chemitech.net.cn

x |= (1 << 3);
来源：http://ma.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://th.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ei.shxzukj.cn

[S18] C：命令行参数
来源：http://xb.hahajie.cn

int main(int argc, char **argv)
来源：http://ob.jctech888.com.cn

[S19] C：快速排序
来源：http://pd.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sw.panjiajie.cn

[S20] C：二分查找
来源：http://ic.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fc.gzmigu.cn

[S21] C：字符类别判断
来源：http://ib.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ok.521024.cn

[S22] C：字符串转数字
来源：http://st.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qs.yuexingan06.cn

[S23] C：随机数
来源：http://th.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nc.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://ob.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cr.nszjky.cn

[S25] C：内存拷贝
来源：http://fg.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://up.huanxung.cn

[S26] C：内存清零
来源：http://bg.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://er.shxzukj.cn

[S27] C：定义常量
来源：http://nk.nicolike.cn

const double PI = 3.14159;
来源：http://zs.shxzukj.cn

[S28] C：静态变量
来源：http://aj.nicolike.cn


<!-- 参考信息 -->