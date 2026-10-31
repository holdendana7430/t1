代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ov.shxzskj.cn

[Q58] 累计求和
来源：http://wi.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lp.szxytkj.cn

[Q59] 分组内累计
来源：http://jq.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eq.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://id.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dj.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zi.shxzskj.cn

[Q61] 移动平均
来源：http://kn.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://el.shtwfgs.cn

[Q62] 分组占比
来源：http://tj.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hj.muxihuayi.cn

[Q63] 开启事务
来源：http://lu.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rx.huixiangedu.cn

[Q64] 提交事务
来源：http://qm.bookmarksfly.cn

COMMIT;
来源：http://rr.shxzukj.cn

[Q65] 回滚事务
来源：http://pr.wgjwhj.cn

ROLLBACK;
来源：http://jg.521024.cn

[Q66] 行锁查询
来源：http://ms.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uo.lnxyls.cn

[Q67] 设置隔离级别
来源：http://gl.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ax.hnjuh.cn

[Q68] 保存点
来源：http://dt.jctech888.com.cn

SAVEPOINT sp1;
来源：http://go.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://nv.gzmigu.cn

[Q69] 查看执行计划
来源：http://lt.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://us.jctech888.com.cn

[Q70] 更新统计信息
来源：http://pj.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://gs.shtwfgs.cn

[Q71] 查看建表语句
来源：http://mi.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://si.szsharing.cn

[Q72] 查看索引
来源：http://rv.lnxyls.cn

SHOW INDEX FROM users;
来源：http://zz.gzmigu.cn

[Q73] 查看表状态
来源：http://ww.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mc.yuexingan06.cn

[Q74] 强制使用索引
来源：http://yl.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bq.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://vl.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fj.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://me.bjjhwx.cn

[Q76] 按天统计
来源：http://hj.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ba.bjjhwx.cn

[Q77] 时间加减
来源：http://od.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lx.shtwfgs.cn

[Q78] 当前时间
来源：http://hi.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://on.hnjuh.cn

[Q79] 字符串拼接
来源：http://pf.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dd.shtwfgs.cn

[Q80] 字符串截取
来源：http://pm.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://km.gzmigu.cn

[Q81] 字符串替换
来源：http://ib.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mu.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://jy.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rl.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://pz.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ap.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://ut.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://ut.shtwfgs.cn

[Q85] 数值取整
来源：http://ey.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yv.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://zh.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nf.newstarts.cn

[Q87] JSON 字段做条件
来源：http://si.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fn.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://kf.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lm.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hd.521024.cn

[Q89] 判断表是否存在
来源：http://cq.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lq.szxytkj.cn

[Q90] 生成序号列
来源：http://rt.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fz.yuntaijiaju.cn

================================================================================
来源：http://fv.9csxet.cn

R. Bash 专题
来源：http://ad.jianghongdianzi.cn

================================================================================
来源：http://tj.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://gs.haigaiapp.cn

#!/usr/bin/env bash
来源：http://jm.lnxyls.cn

set -euo pipefail
来源：http://lg.hahajie.cn

[R02] 变量赋值与使用
来源：http://ut.521024.cn

name="Tom"; echo "$name"
来源：http://ti.szxytkj.cn

[R03] 只读变量
来源：http://lt.haigaiapp.cn

readonly PI=3.14
来源：http://ge.shxzskj.cn

[R04] 位置参数
来源：http://ot.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ql.huanxung.cn

[R05] 参数默认值
来源：http://xi.521024.cn

name="${1:-default}"
来源：http://ko.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://ip.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uq.hnjuh.cn

[R07] if 判断文件
来源：http://oj.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jo.bookmarksfly.cn

[R08] 数值比较
来源：http://fu.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lo.jctech888.com.cn

[R09] 字符串比较
来源：http://uu.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ff.9csxet.cn

[R10] 正则匹配
来源：http://pc.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gc.hahajie.cn

[R11] case 多分支
来源：http://dz.newstarts.cn

case "$1" in
来源：http://dn.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://dd.newstarts.cn

stop)  echo "停止" ;;
来源：http://yf.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://fz.colortex.cn

esac
来源：http://sg.muxihuayi.cn

[R12] for 遍历文件
来源：http://to.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://ry.huanxung.cn

[R13] for 计数循环
来源：http://az.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://hd.shtwfgs.cn

[R14] C 风格 for
来源：http://zp.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.muxihuayi.cn

[R15] while 逐行读文件
来源：http://nn.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rd.hahajie.cn

[R16] until 等待条件
来源：http://cm.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oh.gzmigu.cn

[R17] 数组定义与取值
来源：http://ao.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tf.nszjky.cn

[R18] 遍历数组
来源：http://vp.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rs.muxihuayi.cn

[R19] 数组长度
来源：http://xm.newstarts.cn

echo "${#arr[@]}"
来源：http://rn.nicolike.cn

[R20] 关联数组（字典）
来源：http://lo.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iz.szxytkj.cn

[R21] 字符串长度
来源：http://jq.nszjky.cn

echo "${#s}"
来源：http://en.bjjhwx.cn

[R22] 截取子串
来源：http://px.hahajie.cn

echo "${s:0:5}"
来源：http://xd.szxytkj.cn

[R23] 字符串替换
来源：http://um.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hi.bjjhwx.cn

[R24] 大小写转换
来源：http://uz.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rc.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://nn.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ho.huanxung.cn

[R26] 命令替换
来源：http://vy.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://ja.shxzukj.cn

[R27] 算术展开
来源：http://gp.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://jg.haigaiapp.cn

[R28] 浮点运算
来源：http://xe.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://tn.bookmarksfly.cn

[R29] 定义函数
来源：http://zz.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ci.shxzukj.cn

[R30] 函数返回状态码
来源：http://ay.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://ik.huixiangedu.cn

[R31] 局部变量
来源：http://hy.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://ps.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://yt.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://la.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://yf.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mn.shtwfgs.cn

[R34] 退出时清理
来源：http://gj.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://br.colortex.cn

[R35] 后台执行并等待
来源：http://js.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vf.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://me.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qh.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://tq.lnxyls.cn

files=$(ls -1)
来源：http://hm.szsharing.cn

[R38] 管道串联
来源：http://zu.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://ea.asd995.cn

[R39] 重定向标准输出与错误
来源：http://ll.asd995.cn

cmd > out.log 2>&1
来源：http://bh.huanxung.cn

[R40] 追加写日志
来源：http://hs.chemitech.net.cn

echo "log" >> out.log
来源：http://qm.gzmigu.cn

[R41] 丢弃输出
来源：http://ej.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://fh.shtwfgs.cn

[R42] 输入重定向
来源：http://tv.nszjky.cn

wc -l < a.txt
来源：http://cx.panjiajie.cn

[R43] 按名字查找文件
来源：http://jk.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://cs.haigaiapp.cn

[R44] 按修改时间查找
来源：http://eu.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://dk.yuexingan06.cn

[R45] 批量删除
来源：http://pm.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://hi.shxzskj.cn

[R46] 递归替换文件内容
来源：http://ca.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zv.shtwfgs.cn

[R47] sed 单行替换
来源：http://oh.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zz.muxihuayi.cn

[R48] awk 取指定列
来源：http://qj.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://re.asd995.cn

[R49] awk 带条件
来源：http://yx.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sn.muxihuayi.cn

[R50] awk 求和
来源：http://ti.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://da.shxzukj.cn

[R51] 排序去重取前几
来源：http://pg.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nn.szxytkj.cn

[R52] 统计行数
来源：http://uy.colortex.cn

wc -l a.txt
来源：http://mw.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://dx.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rv.bookmarksfly.cn

[R54] 比较两个文件
来源：http://hv.gzmigu.cn

diff a.txt b.txt
来源：http://ju.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://tf.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nv.jctech888.com.cn

[R56] 远程拷贝
来源：http://gp.shtwfgs.cn

scp file user@host:/path/
来源：http://me.gzmigu.cn

[R57] 远程执行命令
来源：http://xf.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://xc.huixiangedu.cn

[R58] 下载文件
来源：http://up.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cl.gzmigu.cn

[R59] 发 POST JSON
来源：http://tm.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nf.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ru.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ln.newstarts.cn

[R61] 磁盘占用
来源：http://rd.panjiajie.cn

df -h;  du -sh *
来源：http://nr.hahajie.cn

[R62] 找最占空间的文件
来源：http://ng.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://py.muxihuayi.cn

[R63] 内存与进程
来源：http://oe.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://na.szsharing.cn

[R64] 结束进程
来源：http://ku.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://ow.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://sm.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oo.hnjuh.cn

[R66] 定时任务
来源：http://oe.hahajie.cn

crontab -e;  crontab -l
来源：http://ko.hahajie.cn

[R67] 生成随机十六进制串
来源：http://qw.hnjuh.cn

openssl rand -hex 16
来源：http://qc.521024.cn

[R68] 计算文件校验值
来源：http://yi.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bc.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://nt.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://bs.bjjhwx.cn

[R70] 时间戳与互转
来源：http://cv.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://hg.huixinmuqiang.cn

[R71] 日期格式化
来源：http://qy.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wj.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://cw.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sq.haigaiapp.cn

[R73] 分割大日志
来源：http://ne.bjjhwx.cn

split -l 1000 big.log part_
来源：http://pl.shtwfgs.cn

[R74] 批量重命名
来源：http://wp.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nl.yuexingan06.cn

[R75] 导出环境变量
来源：http://iz.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ki.asd995.cn

[R76] 使用临时文件
来源：http://tm.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oq.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://ad.bjjhwx.cn

read -rp "请输入: " ans
来源：http://tl.newstarts.cn

[R78] 交互式菜单
来源：http://pm.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yk.muxihuayi.cn

[R79] 解析命令行选项
来源：http://ow.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dh.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://ct.yuexingan06.cn

time ./run.sh
来源：http://bm.nicolike.cn

================================================================================
来源：http://ce.szsharing.cn

S. C / C++ 专题
来源：http://mp.shxzskj.cn

================================================================================
来源：http://vg.yuexingan06.cn

[S01] C：Hello World
来源：http://yo.muxihuayi.cn

#include <stdio.h>
来源：http://oq.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://et.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://mg.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://zi.shxzukj.cn

[S03] C：读入整数
来源：http://oa.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://dg.huixiangedu.cn

[S04] C：字符串复制
来源：http://xk.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://om.newstarts.cn

[S05] C：字符串长度
来源：http://gl.wgjwhj.cn

strlen(s)
来源：http://av.nszjky.cn

[S06] C：字符串比较
来源：http://rc.hnjuh.cn

strcmp(a, b) == 0
来源：http://jg.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://lg.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cx.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://kl.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cn.colortex.cn

[S09] C：结构体定义与初始化
来源：http://vn.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wc.bjjhwx.cn

[S10] C：指针与解引用
来源：http://ty.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://jk.jctech888.com.cn

[S11] C：逐行读文件
来源：http://qs.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://wu.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xf.huanxung.cn

fclose(f);
来源：http://fb.szsharing.cn

[S12] C：写文件
来源：http://om.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ub.haigaiapp.cn

[S13] C：宏定义
来源：http://vs.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jb.colortex.cn

[S14] C：枚举
来源：http://fu.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://sb.jianghongdianzi.cn

[S15] C：类型转换
来源：http://jj.nszjky.cn

(double) a / b
来源：http://yg.huanxung.cn

[S16] C：位操作置位
来源：http://gb.lnxyls.cn

x |= (1 << 3);
来源：http://up.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://mx.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bm.huixiangedu.cn

[S18] C：命令行参数
来源：http://za.huanxung.cn

int main(int argc, char **argv)
来源：http://os.hnjuh.cn

[S19] C：快速排序
来源：http://cx.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sd.szsharing.cn

[S20] C：二分查找
来源：http://zy.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wv.wgjwhj.cn

[S21] C：字符类别判断
来源：http://yf.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yo.hnjuh.cn

[S22] C：字符串转数字
来源：http://od.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qy.hahajie.cn

[S23] C：随机数
来源：http://np.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mx.9csxet.cn

[S24] C：获取本地时间
来源：http://pw.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mv.shxzukj.cn

[S25] C：内存拷贝
来源：http://bx.bjjhwx.cn

memcpy(dst, src, n);
来源：http://tc.wgjwhj.cn

[S26] C：内存清零
来源：http://rc.huanxung.cn

memset(a, 0, sizeof a);
来源：http://ph.gzmigu.cn

[S27] C：定义常量
来源：http://au.521024.cn

const double PI = 3.14159;
来源：http://tb.szsharing.cn

[S28] C：静态变量
来源：http://pn.newstarts.cn


<!-- 参考信息 -->