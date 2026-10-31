代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zg.shtwfgs.cn

[Q52] 删除指定行
来源：http://zl.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://rq.wgjwhj.cn

[Q53] 按条件删除
来源：http://rh.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rj.muxihuayi.cn

[Q54] 清空表
来源：http://kw.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://ci.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://nk.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jj.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://cs.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nd.521024.cn

[Q57] 行号
来源：http://wp.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nu.gzmigu.cn

[Q58] 累计求和
来源：http://ne.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qu.gzmigu.cn

[Q59] 分组内累计
来源：http://so.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qi.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://nx.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zd.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lx.bjjhwx.cn

[Q61] 移动平均
来源：http://bo.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wl.huixinmuqiang.cn

[Q62] 分组占比
来源：http://kx.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tp.wgjwhj.cn

[Q63] 开启事务
来源：http://in.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bu.jctech888.com.cn

[Q64] 提交事务
来源：http://lt.szsharing.cn

COMMIT;
来源：http://pj.lnxyls.cn

[Q65] 回滚事务
来源：http://ox.huixinmuqiang.cn

ROLLBACK;
来源：http://aj.jctech888.com.cn

[Q66] 行锁查询
来源：http://ar.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://il.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://xo.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sv.huanxung.cn

[Q68] 保存点
来源：http://fc.muxihuayi.cn

SAVEPOINT sp1;
来源：http://nb.shxzskj.cn

ROLLBACK TO sp1;
来源：http://ls.asd995.cn

[Q69] 查看执行计划
来源：http://wl.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ro.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://ak.9csxet.cn

ANALYZE TABLE users;
来源：http://oq.newstarts.cn

[Q71] 查看建表语句
来源：http://kn.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ni.shxzukj.cn

[Q72] 查看索引
来源：http://pe.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://sm.bookmarksfly.cn

[Q73] 查看表状态
来源：http://sq.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uy.lnxyls.cn

[Q74] 强制使用索引
来源：http://rm.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mt.huanxung.cn

[Q75] 日期格式化
来源：http://av.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sk.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vk.521024.cn

[Q76] 按天统计
来源：http://mg.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ko.9csxet.cn

[Q77] 时间加减
来源：http://pz.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aj.jianghongdianzi.cn

[Q78] 当前时间
来源：http://cm.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nz.colortex.cn

[Q79] 字符串拼接
来源：http://ph.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cx.szxytkj.cn

[Q80] 字符串截取
来源：http://hq.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jy.lnxyls.cn

[Q81] 字符串替换
来源：http://ea.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xb.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://hi.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ql.wgjwhj.cn

[Q83] 大小写转换
来源：http://go.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ks.gzmigu.cn

[Q84] 去除首尾空格
来源：http://vk.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://vy.yuntaijiaju.cn

[Q85] 数值取整
来源：http://mg.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mo.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://fe.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jb.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://yb.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wk.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://bc.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://il.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qy.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://ic.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ul.colortex.cn

[Q90] 生成序号列
来源：http://dl.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zz.bjjhwx.cn

================================================================================
来源：http://kk.bjjhwx.cn

R. Bash 专题
来源：http://bl.jianghongdianzi.cn

================================================================================
来源：http://uu.huanxung.cn

[R01] shebang 与严格模式
来源：http://sr.521024.cn

#!/usr/bin/env bash
来源：http://sq.nszjky.cn

set -euo pipefail
来源：http://dj.521024.cn

[R02] 变量赋值与使用
来源：http://ow.panjiajie.cn

name="Tom"; echo "$name"
来源：http://zo.newstarts.cn

[R03] 只读变量
来源：http://zk.wgjwhj.cn

readonly PI=3.14
来源：http://mf.huixiangedu.cn

[R04] 位置参数
来源：http://fm.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nv.lnxyls.cn

[R05] 参数默认值
来源：http://fg.nicolike.cn

name="${1:-default}"
来源：http://ll.gzmigu.cn

[R06] 判断命令是否存在
来源：http://qe.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nx.yuntaijiaju.cn

[R07] if 判断文件
来源：http://xn.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ls.huixinmuqiang.cn

[R08] 数值比较
来源：http://fq.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vn.yuntaijiaju.cn

[R09] 字符串比较
来源：http://sy.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fs.nicolike.cn

[R10] 正则匹配
来源：http://oj.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bv.9csxet.cn

[R11] case 多分支
来源：http://jb.nicolike.cn

case "$1" in
来源：http://ko.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://ro.nszjky.cn

stop)  echo "停止" ;;
来源：http://ey.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://cn.bjjhwx.cn

esac
来源：http://io.yuexingan06.cn

[R12] for 遍历文件
来源：http://uw.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://uf.panjiajie.cn

[R13] for 计数循环
来源：http://lm.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://ip.jctech888.com.cn

[R14] C 风格 for
来源：http://iu.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wc.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://ob.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nx.asd995.cn

[R16] until 等待条件
来源：http://vy.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fu.gzmigu.cn

[R17] 数组定义与取值
来源：http://cl.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bw.521024.cn

[R18] 遍历数组
来源：http://hl.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hm.lnxyls.cn

[R19] 数组长度
来源：http://eq.nicolike.cn

echo "${#arr[@]}"
来源：http://ln.colortex.cn

[R20] 关联数组（字典）
来源：http://bn.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hi.newstarts.cn

[R21] 字符串长度
来源：http://go.chemitech.net.cn

echo "${#s}"
来源：http://lh.nszjky.cn

[R22] 截取子串
来源：http://ex.haigaiapp.cn

echo "${s:0:5}"
来源：http://lp.huixiangedu.cn

[R23] 字符串替换
来源：http://qo.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zv.muxihuayi.cn

[R24] 大小写转换
来源：http://cu.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ro.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://ov.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eq.wgjwhj.cn

[R26] 命令替换
来源：http://io.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://si.szxytkj.cn

[R27] 算术展开
来源：http://yn.colortex.cn

echo $((1 + 2 * 3))
来源：http://vl.lnxyls.cn

[R28] 浮点运算
来源：http://ux.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://gy.jctech888.com.cn

[R29] 定义函数
来源：http://co.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fb.gzmigu.cn

[R30] 函数返回状态码
来源：http://kl.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://eo.nszjky.cn

[R31] 局部变量
来源：http://qu.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://cq.asd995.cn

[R32] 参数个数校验
来源：http://rp.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zw.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://zx.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mq.jianghongdianzi.cn

[R34] 退出时清理
来源：http://yw.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kr.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://lk.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wn.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://kj.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ts.hahajie.cn

[R37] 把输出赋给变量
来源：http://cq.9csxet.cn

files=$(ls -1)
来源：http://hh.newstarts.cn

[R38] 管道串联
来源：http://yh.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://ua.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://ul.521024.cn

cmd > out.log 2>&1
来源：http://nw.chemitech.net.cn

[R40] 追加写日志
来源：http://oo.jctech888.com.cn

echo "log" >> out.log
来源：http://lo.gzmigu.cn

[R41] 丢弃输出
来源：http://ko.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://hu.shtwfgs.cn

[R42] 输入重定向
来源：http://oo.panjiajie.cn

wc -l < a.txt
来源：http://dx.shtwfgs.cn

[R43] 按名字查找文件
来源：http://ps.521024.cn

find . -name "*.log" -type f
来源：http://bu.shtwfgs.cn

[R44] 按修改时间查找
来源：http://dp.chemitech.net.cn

find . -mtime -7 -type f
来源：http://qk.szxytkj.cn

[R45] 批量删除
来源：http://ay.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://ag.colortex.cn

[R46] 递归替换文件内容
来源：http://pa.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://je.521024.cn

[R47] sed 单行替换
来源：http://yr.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lf.hahajie.cn

[R48] awk 取指定列
来源：http://ll.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://ix.asd995.cn

[R49] awk 带条件
来源：http://ah.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lo.yuexingan06.cn

[R50] awk 求和
来源：http://qk.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bt.shtwfgs.cn

[R51] 排序去重取前几
来源：http://fd.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qe.bjjhwx.cn

[R52] 统计行数
来源：http://xt.chemitech.net.cn

wc -l a.txt
来源：http://ui.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://fq.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ay.bjjhwx.cn

[R54] 比较两个文件
来源：http://yw.newstarts.cn

diff a.txt b.txt
来源：http://xp.hnjuh.cn

[R55] 压缩与解压
来源：http://mk.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zj.muxihuayi.cn

[R56] 远程拷贝
来源：http://oj.nicolike.cn

scp file user@host:/path/
来源：http://aa.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://yf.haigaiapp.cn

ssh user@host 'uptime'
来源：http://dx.yuexingan06.cn

[R58] 下载文件
来源：http://jj.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pv.9csxet.cn

[R59] 发 POST JSON
来源：http://ta.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://si.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://sw.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dm.hahajie.cn

[R61] 磁盘占用
来源：http://re.jctech888.com.cn

df -h;  du -sh *
来源：http://we.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://hw.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://jw.shxzukj.cn

[R63] 内存与进程
来源：http://zk.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://mt.szsharing.cn

[R64] 结束进程
来源：http://yd.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://nv.bjjhwx.cn

[R65] 查看端口占用
来源：http://mc.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vs.chemitech.net.cn

[R66] 定时任务
来源：http://kc.9csxet.cn

crontab -e;  crontab -l
来源：http://bx.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://to.nszjky.cn

openssl rand -hex 16
来源：http://va.colortex.cn

[R68] 计算文件校验值
来源：http://iz.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yj.shxzukj.cn

[R69] 生成随机密码
来源：http://ot.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://qm.huixiangedu.cn

[R70] 时间戳与互转
来源：http://xe.nicolike.cn

date +%s;  date -d @1700000000
来源：http://vd.shxzukj.cn

[R71] 日期格式化
来源：http://vb.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jg.haigaiapp.cn

[R72] 等待端口就绪
来源：http://gj.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://as.huixiangedu.cn

[R73] 分割大日志
来源：http://tx.9csxet.cn

split -l 1000 big.log part_
来源：http://dy.nicolike.cn

[R74] 批量重命名
来源：http://zg.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oy.shxzukj.cn

[R75] 导出环境变量
来源：http://mf.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://gg.bjjhwx.cn

[R76] 使用临时文件
来源：http://sa.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oy.shtwfgs.cn

[R77] 读取用户输入
来源：http://fd.9csxet.cn

read -rp "请输入: " ans
来源：http://qq.shtwfgs.cn

[R78] 交互式菜单
来源：http://al.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wi.colortex.cn

[R79] 解析命令行选项
来源：http://kl.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vs.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://js.9csxet.cn

time ./run.sh
来源：http://ql.bookmarksfly.cn

================================================================================
来源：http://ys.panjiajie.cn

S. C / C++ 专题
来源：http://in.jianghongdianzi.cn

================================================================================
来源：http://nb.yuexingan06.cn

[S01] C：Hello World
来源：http://hh.newstarts.cn

#include <stdio.h>
来源：http://di.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bf.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://al.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://ym.bookmarksfly.cn

[S03] C：读入整数
来源：http://xq.9csxet.cn

int x; scanf("%d", &x);
来源：http://ks.bookmarksfly.cn

[S04] C：字符串复制
来源：http://ya.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://on.huanxung.cn

[S05] C：字符串长度
来源：http://eg.wgjwhj.cn

strlen(s)
来源：http://on.jctech888.com.cn

[S06] C：字符串比较
来源：http://sx.bjjhwx.cn

strcmp(a, b) == 0
来源：http://gu.shxzskj.cn

[S07] C：数组遍历求和
来源：http://kz.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qs.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://kq.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rk.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://tz.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sl.colortex.cn

[S10] C：指针与解引用
来源：http://kn.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://zr.huanxung.cn

[S11] C：逐行读文件
来源：http://ic.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://hj.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kg.colortex.cn

fclose(f);
来源：http://ut.muxihuayi.cn

[S12] C：写文件
来源：http://bz.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wd.huanxung.cn

[S13] C：宏定义
来源：http://wp.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gc.lnxyls.cn

[S14] C：枚举
来源：http://hv.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ko.nicolike.cn

[S15] C：类型转换
来源：http://kq.chemitech.net.cn

(double) a / b
来源：http://gv.nszjky.cn

[S16] C：位操作置位
来源：http://wu.yuexingan06.cn

x |= (1 << 3);
来源：http://as.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://qt.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rw.yuexingan06.cn

[S18] C：命令行参数
来源：http://jt.colortex.cn

int main(int argc, char **argv)
来源：http://me.szsharing.cn

[S19] C：快速排序
来源：http://gi.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ci.chemitech.net.cn

[S20] C：二分查找
来源：http://gq.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://go.shxzskj.cn

[S21] C：字符类别判断
来源：http://ej.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zm.jctech888.com.cn

[S22] C：字符串转数字
来源：http://hb.gzmigu.cn


<!-- 参考信息 -->