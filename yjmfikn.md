代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hs.colortex.cn

[Q54] 清空表
来源：http://cw.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://ho.hahajie.cn

[Q55] 排名（并列占位）
来源：http://hn.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lt.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://nr.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jw.yuexingan06.cn

[Q57] 行号
来源：http://gz.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yo.lnxyls.cn

[Q58] 累计求和
来源：http://ii.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fs.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://xj.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://di.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://py.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vg.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fd.jianghongdianzi.cn

[Q61] 移动平均
来源：http://ri.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ww.bookmarksfly.cn

[Q62] 分组占比
来源：http://fy.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ba.newstarts.cn

[Q63] 开启事务
来源：http://pg.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pr.shtwfgs.cn

[Q64] 提交事务
来源：http://gt.jctech888.com.cn

COMMIT;
来源：http://ec.hahajie.cn

[Q65] 回滚事务
来源：http://kl.newstarts.cn

ROLLBACK;
来源：http://wj.jctech888.com.cn

[Q66] 行锁查询
来源：http://nj.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cv.521024.cn

[Q67] 设置隔离级别
来源：http://zf.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xq.chemitech.net.cn

[Q68] 保存点
来源：http://no.muxihuayi.cn

SAVEPOINT sp1;
来源：http://nt.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://rx.colortex.cn

[Q69] 查看执行计划
来源：http://ow.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mi.nszjky.cn

[Q70] 更新统计信息
来源：http://qo.asd995.cn

ANALYZE TABLE users;
来源：http://rt.asd995.cn

[Q71] 查看建表语句
来源：http://ju.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ww.wgjwhj.cn

[Q72] 查看索引
来源：http://dq.nicolike.cn

SHOW INDEX FROM users;
来源：http://sa.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://am.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cy.shtwfgs.cn

[Q74] 强制使用索引
来源：http://tg.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ku.bookmarksfly.cn

[Q75] 日期格式化
来源：http://qa.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bx.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fp.asd995.cn

[Q76] 按天统计
来源：http://eh.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kz.newstarts.cn

[Q77] 时间加减
来源：http://wr.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jq.huixinmuqiang.cn

[Q78] 当前时间
来源：http://nh.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ey.huixiangedu.cn

[Q79] 字符串拼接
来源：http://zq.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zu.521024.cn

[Q80] 字符串截取
来源：http://ct.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bv.muxihuayi.cn

[Q81] 字符串替换
来源：http://fq.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ex.colortex.cn

[Q82] 字符长度与字节长度
来源：http://ls.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ez.9csxet.cn

[Q83] 大小写转换
来源：http://fy.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fy.hnjuh.cn

[Q84] 去除首尾空格
来源：http://ou.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://fy.nicolike.cn

[Q85] 数值取整
来源：http://ed.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pa.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://xf.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vz.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://py.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iz.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://sx.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yb.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xv.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://mh.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qe.shxzukj.cn

[Q90] 生成序号列
来源：http://cz.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sq.yuexingan06.cn

================================================================================
来源：http://by.jctech888.com.cn

R. Bash 专题
来源：http://zs.yuntaijiaju.cn

================================================================================
来源：http://kl.lnxyls.cn

[R01] shebang 与严格模式
来源：http://fk.colortex.cn

#!/usr/bin/env bash
来源：http://sy.shxzskj.cn

set -euo pipefail
来源：http://wa.colortex.cn

[R02] 变量赋值与使用
来源：http://lw.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://pu.jctech888.com.cn

[R03] 只读变量
来源：http://cw.bookmarksfly.cn

readonly PI=3.14
来源：http://jh.szsharing.cn

[R04] 位置参数
来源：http://eu.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uf.panjiajie.cn

[R05] 参数默认值
来源：http://if.huixinmuqiang.cn

name="${1:-default}"
来源：http://wi.asd995.cn

[R06] 判断命令是否存在
来源：http://ep.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wa.jctech888.com.cn

[R07] if 判断文件
来源：http://sr.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://me.hnjuh.cn

[R08] 数值比较
来源：http://dj.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xn.szsharing.cn

[R09] 字符串比较
来源：http://zh.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://im.gzmigu.cn

[R10] 正则匹配
来源：http://fz.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ul.szxytkj.cn

[R11] case 多分支
来源：http://un.jianghongdianzi.cn

case "$1" in
来源：http://jw.asd995.cn

start) echo "启动" ;;
来源：http://ka.szxytkj.cn

stop)  echo "停止" ;;
来源：http://cw.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://jr.521024.cn

esac
来源：http://ym.szsharing.cn

[R12] for 遍历文件
来源：http://wx.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://ub.szsharing.cn

[R13] for 计数循环
来源：http://af.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://ui.szxytkj.cn

[R14] C 风格 for
来源：http://ts.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ez.lnxyls.cn

[R15] while 逐行读文件
来源：http://iy.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wo.gzmigu.cn

[R16] until 等待条件
来源：http://vk.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wd.hahajie.cn

[R17] 数组定义与取值
来源：http://ia.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ln.bjjhwx.cn

[R18] 遍历数组
来源：http://az.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://la.shxzskj.cn

[R19] 数组长度
来源：http://uh.yuexingan06.cn

echo "${#arr[@]}"
来源：http://go.shxzskj.cn

[R20] 关联数组（字典）
来源：http://rx.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qf.hahajie.cn

[R21] 字符串长度
来源：http://ch.gzmigu.cn

echo "${#s}"
来源：http://zd.huanxung.cn

[R22] 截取子串
来源：http://sg.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://vn.huixiangedu.cn

[R23] 字符串替换
来源：http://mw.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kx.colortex.cn

[R24] 大小写转换
来源：http://cl.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tx.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://we.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ml.szsharing.cn

[R26] 命令替换
来源：http://jw.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://er.szxytkj.cn

[R27] 算术展开
来源：http://ak.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://gv.muxihuayi.cn

[R28] 浮点运算
来源：http://an.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://yb.hnjuh.cn

[R29] 定义函数
来源：http://ri.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xa.wgjwhj.cn

[R30] 函数返回状态码
来源：http://ho.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://fw.huanxung.cn

[R31] 局部变量
来源：http://os.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://od.wgjwhj.cn

[R32] 参数个数校验
来源：http://qf.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tr.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://wz.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://og.jianghongdianzi.cn

[R34] 退出时清理
来源：http://vc.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ny.jctech888.com.cn

[R35] 后台执行并等待
来源：http://iw.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vu.nicolike.cn

[R36] 并发执行多个任务
来源：http://nf.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mm.gzmigu.cn

[R37] 把输出赋给变量
来源：http://vy.huixiangedu.cn

files=$(ls -1)
来源：http://tz.9csxet.cn

[R38] 管道串联
来源：http://ce.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://vg.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://dj.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://tf.bookmarksfly.cn

[R40] 追加写日志
来源：http://fj.yuexingan06.cn

echo "log" >> out.log
来源：http://lu.jctech888.com.cn

[R41] 丢弃输出
来源：http://ke.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://uv.panjiajie.cn

[R42] 输入重定向
来源：http://ky.shtwfgs.cn

wc -l < a.txt
来源：http://xy.bjjhwx.cn

[R43] 按名字查找文件
来源：http://hb.yuexingan06.cn

find . -name "*.log" -type f
来源：http://ig.lnxyls.cn

[R44] 按修改时间查找
来源：http://qy.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://gx.chemitech.net.cn

[R45] 批量删除
来源：http://cz.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://lz.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://ch.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://og.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://ml.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rs.jctech888.com.cn

[R48] awk 取指定列
来源：http://wt.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://cy.shtwfgs.cn

[R49] awk 带条件
来源：http://kf.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://se.gzmigu.cn

[R50] awk 求和
来源：http://tz.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pt.hnjuh.cn

[R51] 排序去重取前几
来源：http://oz.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cl.szsharing.cn

[R52] 统计行数
来源：http://fk.szxytkj.cn

wc -l a.txt
来源：http://cl.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://mi.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nr.panjiajie.cn

[R54] 比较两个文件
来源：http://wo.jctech888.com.cn

diff a.txt b.txt
来源：http://sl.9csxet.cn

[R55] 压缩与解压
来源：http://oh.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gz.colortex.cn

[R56] 远程拷贝
来源：http://gy.9csxet.cn

scp file user@host:/path/
来源：http://yl.jctech888.com.cn

[R57] 远程执行命令
来源：http://lo.haigaiapp.cn

ssh user@host 'uptime'
来源：http://xa.yuntaijiaju.cn

[R58] 下载文件
来源：http://bn.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fq.lnxyls.cn

[R59] 发 POST JSON
来源：http://uf.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://df.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://hz.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://po.chemitech.net.cn

[R61] 磁盘占用
来源：http://ge.hahajie.cn

df -h;  du -sh *
来源：http://ie.szxytkj.cn

[R62] 找最占空间的文件
来源：http://py.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://sa.jianghongdianzi.cn

[R63] 内存与进程
来源：http://ku.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://aj.lnxyls.cn

[R64] 结束进程
来源：http://gu.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://wb.nicolike.cn

[R65] 查看端口占用
来源：http://lr.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qd.colortex.cn

[R66] 定时任务
来源：http://ru.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://dg.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://gg.huixinmuqiang.cn

openssl rand -hex 16
来源：http://dg.muxihuayi.cn

[R68] 计算文件校验值
来源：http://ug.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fn.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://us.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://nh.shtwfgs.cn

[R70] 时间戳与互转
来源：http://en.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://yy.gzmigu.cn

[R71] 日期格式化
来源：http://im.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uk.haigaiapp.cn

[R72] 等待端口就绪
来源：http://dg.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aq.shxzukj.cn

[R73] 分割大日志
来源：http://mg.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://js.asd995.cn

[R74] 批量重命名
来源：http://wp.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lx.jctech888.com.cn

[R75] 导出环境变量
来源：http://rr.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://qd.wgjwhj.cn

[R76] 使用临时文件
来源：http://fi.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gr.chemitech.net.cn

[R77] 读取用户输入
来源：http://it.hnjuh.cn

read -rp "请输入: " ans
来源：http://kk.huixiangedu.cn

[R78] 交互式菜单
来源：http://aq.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hx.newstarts.cn

[R79] 解析命令行选项
来源：http://jt.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hl.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://tt.newstarts.cn

time ./run.sh
来源：http://om.panjiajie.cn

================================================================================
来源：http://cn.haigaiapp.cn

S. C / C++ 专题
来源：http://sw.jianghongdianzi.cn

================================================================================
来源：http://km.jianghongdianzi.cn

[S01] C：Hello World
来源：http://zl.szsharing.cn

#include <stdio.h>
来源：http://qz.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bo.hahajie.cn

[S02] C：变量与格式化输出
来源：http://dg.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://qr.shxzukj.cn

[S03] C：读入整数
来源：http://sk.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://fb.nicolike.cn

[S04] C：字符串复制
来源：http://qf.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rp.shtwfgs.cn

[S05] C：字符串长度
来源：http://tc.hnjuh.cn

strlen(s)
来源：http://zo.nicolike.cn

[S06] C：字符串比较
来源：http://zf.wgjwhj.cn

strcmp(a, b) == 0
来源：http://fx.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://az.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bz.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://gr.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ev.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://yx.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nl.hahajie.cn

[S10] C：指针与解引用
来源：http://kc.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://jv.szsharing.cn

[S11] C：逐行读文件
来源：http://pm.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://vx.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ks.gzmigu.cn

fclose(f);
来源：http://rx.jctech888.com.cn

[S12] C：写文件
来源：http://vz.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lm.newstarts.cn

[S13] C：宏定义
来源：http://jx.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hj.chemitech.net.cn

[S14] C：枚举
来源：http://hb.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://xw.huixiangedu.cn

[S15] C：类型转换
来源：http://ts.huanxung.cn

(double) a / b
来源：http://xb.521024.cn

[S16] C：位操作置位
来源：http://oz.hahajie.cn

x |= (1 << 3);
来源：http://nt.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://wr.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hn.colortex.cn

[S18] C：命令行参数
来源：http://oy.gzmigu.cn

int main(int argc, char **argv)
来源：http://il.newstarts.cn

[S19] C：快速排序
来源：http://lr.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sq.nicolike.cn

[S20] C：二分查找
来源：http://bt.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uy.shxzukj.cn

[S21] C：字符类别判断
来源：http://yl.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vy.huixiangedu.cn

[S22] C：字符串转数字
来源：http://bo.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gz.gzmigu.cn

[S23] C：随机数
来源：http://hl.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mm.colortex.cn

[S24] C：获取本地时间
来源：http://gv.yuntaijiaju.cn


<!-- 参考信息 -->