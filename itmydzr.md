代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tt.shxzskj.cn

[Q50] 批量更新
来源：http://sz.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ee.nicolike.cn

[Q51] 用子查询更新
来源：http://ho.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yu.chemitech.net.cn

[Q52] 删除指定行
来源：http://gr.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://ve.szxytkj.cn

[Q53] 按条件删除
来源：http://cv.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mf.shtwfgs.cn

[Q54] 清空表
来源：http://kp.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://xv.huanxung.cn

[Q55] 排名（并列占位）
来源：http://kl.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wv.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://zr.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mr.9csxet.cn

[Q57] 行号
来源：http://op.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tu.jianghongdianzi.cn

[Q58] 累计求和
来源：http://vr.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://el.haigaiapp.cn

[Q59] 分组内累计
来源：http://pw.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xx.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://mw.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gv.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hj.chemitech.net.cn

[Q61] 移动平均
来源：http://sq.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://os.muxihuayi.cn

[Q62] 分组占比
来源：http://hr.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ys.jianghongdianzi.cn

[Q63] 开启事务
来源：http://mu.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xx.shxzukj.cn

[Q64] 提交事务
来源：http://rm.jianghongdianzi.cn

COMMIT;
来源：http://or.asd995.cn

[Q65] 回滚事务
来源：http://fr.newstarts.cn

ROLLBACK;
来源：http://lq.lnxyls.cn

[Q66] 行锁查询
来源：http://tt.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eg.hnjuh.cn

[Q67] 设置隔离级别
来源：http://vz.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tt.yuexingan06.cn

[Q68] 保存点
来源：http://de.hnjuh.cn

SAVEPOINT sp1;
来源：http://jk.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://ct.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://xm.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://up.9csxet.cn

[Q70] 更新统计信息
来源：http://lt.haigaiapp.cn

ANALYZE TABLE users;
来源：http://dd.chemitech.net.cn

[Q71] 查看建表语句
来源：http://uy.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ql.muxihuayi.cn

[Q72] 查看索引
来源：http://bf.nicolike.cn

SHOW INDEX FROM users;
来源：http://si.muxihuayi.cn

[Q73] 查看表状态
来源：http://ol.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rw.9csxet.cn

[Q74] 强制使用索引
来源：http://se.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vv.shxzukj.cn

[Q75] 日期格式化
来源：http://ve.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qc.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mg.shtwfgs.cn

[Q76] 按天统计
来源：http://rx.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bz.szxytkj.cn

[Q77] 时间加减
来源：http://gp.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dd.shxzskj.cn

[Q78] 当前时间
来源：http://lb.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bl.bjjhwx.cn

[Q79] 字符串拼接
来源：http://ki.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rd.lnxyls.cn

[Q80] 字符串截取
来源：http://hj.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zo.hahajie.cn

[Q81] 字符串替换
来源：http://tm.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mh.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://wt.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zj.nszjky.cn

[Q83] 大小写转换
来源：http://mm.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jm.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://vd.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://kt.szsharing.cn

[Q85] 数值取整
来源：http://fx.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://st.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://al.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qi.asd995.cn

[Q87] JSON 字段做条件
来源：http://on.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gs.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://ar.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vy.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jg.hnjuh.cn

[Q89] 判断表是否存在
来源：http://um.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xk.panjiajie.cn

[Q90] 生成序号列
来源：http://io.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ic.9csxet.cn

================================================================================
来源：http://eq.yuntaijiaju.cn

R. Bash 专题
来源：http://qm.yuexingan06.cn

================================================================================
来源：http://ic.colortex.cn

[R01] shebang 与严格模式
来源：http://af.muxihuayi.cn

#!/usr/bin/env bash
来源：http://if.gzmigu.cn

set -euo pipefail
来源：http://ws.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://mc.521024.cn

name="Tom"; echo "$name"
来源：http://vx.muxihuayi.cn

[R03] 只读变量
来源：http://kz.haigaiapp.cn

readonly PI=3.14
来源：http://yk.panjiajie.cn

[R04] 位置参数
来源：http://yw.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jt.haigaiapp.cn

[R05] 参数默认值
来源：http://cn.huixinmuqiang.cn

name="${1:-default}"
来源：http://ns.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://mh.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://al.panjiajie.cn

[R07] if 判断文件
来源：http://fy.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xb.bookmarksfly.cn

[R08] 数值比较
来源：http://vg.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gi.huixiangedu.cn

[R09] 字符串比较
来源：http://ki.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qs.newstarts.cn

[R10] 正则匹配
来源：http://aq.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cv.wgjwhj.cn

[R11] case 多分支
来源：http://xq.muxihuayi.cn

case "$1" in
来源：http://ld.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://nx.shxzskj.cn

stop)  echo "停止" ;;
来源：http://rq.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://mt.wgjwhj.cn

esac
来源：http://nn.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://tf.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://ib.huanxung.cn

[R13] for 计数循环
来源：http://tf.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://mt.hnjuh.cn

[R14] C 风格 for
来源：http://of.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ya.hahajie.cn

[R15] while 逐行读文件
来源：http://ej.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ew.newstarts.cn

[R16] until 等待条件
来源：http://ss.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vq.newstarts.cn

[R17] 数组定义与取值
来源：http://sd.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bm.szxytkj.cn

[R18] 遍历数组
来源：http://ee.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qy.yuexingan06.cn

[R19] 数组长度
来源：http://tc.huixiangedu.cn

echo "${#arr[@]}"
来源：http://fc.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://fm.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jx.521024.cn

[R21] 字符串长度
来源：http://qm.huanxung.cn

echo "${#s}"
来源：http://pq.9csxet.cn

[R22] 截取子串
来源：http://lk.shtwfgs.cn

echo "${s:0:5}"
来源：http://fd.lnxyls.cn

[R23] 字符串替换
来源：http://rh.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qt.szxytkj.cn

[R24] 大小写转换
来源：http://wp.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bs.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://yg.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tn.haigaiapp.cn

[R26] 命令替换
来源：http://dr.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://xp.yuntaijiaju.cn

[R27] 算术展开
来源：http://rh.newstarts.cn

echo $((1 + 2 * 3))
来源：http://ks.shxzukj.cn

[R28] 浮点运算
来源：http://oy.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://aw.jianghongdianzi.cn

[R29] 定义函数
来源：http://bk.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nl.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://ce.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://fi.jctech888.com.cn

[R31] 局部变量
来源：http://dy.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://fa.panjiajie.cn

[R32] 参数个数校验
来源：http://qu.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zu.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://xk.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rz.shxzskj.cn

[R34] 退出时清理
来源：http://gk.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zj.colortex.cn

[R35] 后台执行并等待
来源：http://yp.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gu.hnjuh.cn

[R36] 并发执行多个任务
来源：http://sz.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://im.panjiajie.cn

[R37] 把输出赋给变量
来源：http://hn.lnxyls.cn

files=$(ls -1)
来源：http://gb.bookmarksfly.cn

[R38] 管道串联
来源：http://xd.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://ts.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://ok.hahajie.cn

cmd > out.log 2>&1
来源：http://rh.huanxung.cn

[R40] 追加写日志
来源：http://py.yuexingan06.cn

echo "log" >> out.log
来源：http://li.jctech888.com.cn

[R41] 丢弃输出
来源：http://ts.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://xv.nszjky.cn

[R42] 输入重定向
来源：http://ud.haigaiapp.cn

wc -l < a.txt
来源：http://gj.shxzskj.cn

[R43] 按名字查找文件
来源：http://we.hahajie.cn

find . -name "*.log" -type f
来源：http://zu.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://rf.bjjhwx.cn

find . -mtime -7 -type f
来源：http://pz.szxytkj.cn

[R45] 批量删除
来源：http://na.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://tv.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://yi.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ox.shxzskj.cn

[R47] sed 单行替换
来源：http://uo.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gd.yuexingan06.cn

[R48] awk 取指定列
来源：http://fb.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://eh.asd995.cn

[R49] awk 带条件
来源：http://tt.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mq.szxytkj.cn

[R50] awk 求和
来源：http://mu.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://op.shtwfgs.cn

[R51] 排序去重取前几
来源：http://cz.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fl.chemitech.net.cn

[R52] 统计行数
来源：http://kh.newstarts.cn

wc -l a.txt
来源：http://to.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://wi.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ch.nszjky.cn

[R54] 比较两个文件
来源：http://gv.panjiajie.cn

diff a.txt b.txt
来源：http://ms.muxihuayi.cn

[R55] 压缩与解压
来源：http://zi.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ik.shtwfgs.cn

[R56] 远程拷贝
来源：http://uw.yuntaijiaju.cn

scp file user@host:/path/
来源：http://ce.shxzskj.cn

[R57] 远程执行命令
来源：http://nu.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://ol.jctech888.com.cn

[R58] 下载文件
来源：http://ev.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xm.9csxet.cn

[R59] 发 POST JSON
来源：http://cc.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://en.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://wq.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cf.wgjwhj.cn

[R61] 磁盘占用
来源：http://qm.521024.cn

df -h;  du -sh *
来源：http://wv.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://cv.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://xj.colortex.cn

[R63] 内存与进程
来源：http://lc.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://nv.panjiajie.cn

[R64] 结束进程
来源：http://kk.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://vv.muxihuayi.cn

[R65] 查看端口占用
来源：http://kg.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://av.panjiajie.cn

[R66] 定时任务
来源：http://sk.nicolike.cn

crontab -e;  crontab -l
来源：http://re.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://rk.gzmigu.cn

openssl rand -hex 16
来源：http://gg.jctech888.com.cn

[R68] 计算文件校验值
来源：http://sp.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ui.shxzukj.cn

[R69] 生成随机密码
来源：http://hm.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://jb.9csxet.cn

[R70] 时间戳与互转
来源：http://xo.521024.cn

date +%s;  date -d @1700000000
来源：http://wn.jianghongdianzi.cn

[R71] 日期格式化
来源：http://ew.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cy.nicolike.cn

[R72] 等待端口就绪
来源：http://tc.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vz.jctech888.com.cn

[R73] 分割大日志
来源：http://fx.521024.cn

split -l 1000 big.log part_
来源：http://am.colortex.cn

[R74] 批量重命名
来源：http://xo.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bc.muxihuayi.cn

[R75] 导出环境变量
来源：http://kr.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://ky.shtwfgs.cn

[R76] 使用临时文件
来源：http://ap.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ar.gzmigu.cn

[R77] 读取用户输入
来源：http://ou.muxihuayi.cn

read -rp "请输入: " ans
来源：http://yy.wgjwhj.cn

[R78] 交互式菜单
来源：http://tj.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lk.chemitech.net.cn

[R79] 解析命令行选项
来源：http://kr.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kz.521024.cn

[R80] 查看脚本执行耗时
来源：http://je.9csxet.cn

time ./run.sh
来源：http://ab.yuexingan06.cn

================================================================================
来源：http://iy.colortex.cn

S. C / C++ 专题
来源：http://wm.huixiangedu.cn

================================================================================
来源：http://cz.nicolike.cn

[S01] C：Hello World
来源：http://jb.muxihuayi.cn

#include <stdio.h>
来源：http://hc.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vb.9csxet.cn

[S02] C：变量与格式化输出
来源：http://uk.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://qh.nszjky.cn

[S03] C：读入整数
来源：http://xl.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://rt.muxihuayi.cn

[S04] C：字符串复制
来源：http://jv.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qp.wgjwhj.cn

[S05] C：字符串长度
来源：http://mc.hnjuh.cn

strlen(s)
来源：http://ha.nszjky.cn

[S06] C：字符串比较
来源：http://jc.asd995.cn

strcmp(a, b) == 0
来源：http://id.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://bm.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vz.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://pl.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dv.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://ti.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vm.asd995.cn

[S10] C：指针与解引用
来源：http://mu.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://ns.gzmigu.cn

[S11] C：逐行读文件
来源：http://tb.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://jd.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gl.bookmarksfly.cn

fclose(f);
来源：http://jr.chemitech.net.cn

[S12] C：写文件
来源：http://ey.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ma.521024.cn

[S13] C：宏定义
来源：http://js.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ob.muxihuayi.cn

[S14] C：枚举
来源：http://it.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://ge.9csxet.cn

[S15] C：类型转换
来源：http://bx.yuntaijiaju.cn

(double) a / b
来源：http://vz.szxytkj.cn

[S16] C：位操作置位
来源：http://jg.nszjky.cn

x |= (1 << 3);
来源：http://vi.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://qm.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ru.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://qb.panjiajie.cn

int main(int argc, char **argv)
来源：http://xc.yuexingan06.cn

[S19] C：快速排序
来源：http://qq.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mq.haigaiapp.cn

[S20] C：二分查找
来源：http://ll.wgjwhj.cn


<!-- 参考信息 -->