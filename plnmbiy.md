代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uh.9csxet.cn

[Q50] 批量更新
来源：http://ct.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xr.muxihuayi.cn

[Q51] 用子查询更新
来源：http://yw.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kc.nszjky.cn

[Q52] 删除指定行
来源：http://tz.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://pg.nszjky.cn

[Q53] 按条件删除
来源：http://ro.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jm.hahajie.cn

[Q54] 清空表
来源：http://kc.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://nc.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://lp.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jj.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://mb.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cx.panjiajie.cn

[Q57] 行号
来源：http://cn.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bm.9csxet.cn

[Q58] 累计求和
来源：http://xw.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yi.muxihuayi.cn

[Q59] 分组内累计
来源：http://rh.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ql.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://vw.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sh.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mk.haigaiapp.cn

[Q61] 移动平均
来源：http://fv.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vk.9csxet.cn

[Q62] 分组占比
来源：http://pv.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://he.yuntaijiaju.cn

[Q63] 开启事务
来源：http://no.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hj.lnxyls.cn

[Q64] 提交事务
来源：http://oh.nicolike.cn

COMMIT;
来源：http://zm.huixiangedu.cn

[Q65] 回滚事务
来源：http://ks.haigaiapp.cn

ROLLBACK;
来源：http://gb.haigaiapp.cn

[Q66] 行锁查询
来源：http://xe.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tr.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://rq.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jl.shtwfgs.cn

[Q68] 保存点
来源：http://sw.hnjuh.cn

SAVEPOINT sp1;
来源：http://wl.panjiajie.cn

ROLLBACK TO sp1;
来源：http://jj.lnxyls.cn

[Q69] 查看执行计划
来源：http://xm.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lb.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://gm.wgjwhj.cn

ANALYZE TABLE users;
来源：http://ur.gzmigu.cn

[Q71] 查看建表语句
来源：http://qb.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://if.shxzukj.cn

[Q72] 查看索引
来源：http://xf.shxzukj.cn

SHOW INDEX FROM users;
来源：http://dk.9csxet.cn

[Q73] 查看表状态
来源：http://ab.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kd.szxytkj.cn

[Q74] 强制使用索引
来源：http://bf.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://du.lnxyls.cn

[Q75] 日期格式化
来源：http://su.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mn.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://di.521024.cn

[Q76] 按天统计
来源：http://sk.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ox.huixinmuqiang.cn

[Q77] 时间加减
来源：http://gd.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sl.shxzskj.cn

[Q78] 当前时间
来源：http://es.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ug.521024.cn

[Q79] 字符串拼接
来源：http://cw.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oe.huanxung.cn

[Q80] 字符串截取
来源：http://vk.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pn.shxzukj.cn

[Q81] 字符串替换
来源：http://hq.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wp.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://my.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ao.haigaiapp.cn

[Q83] 大小写转换
来源：http://cq.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sv.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://mu.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://zg.hahajie.cn

[Q85] 数值取整
来源：http://jz.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zu.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://yv.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uy.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://gn.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sg.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://dy.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mr.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vk.lnxyls.cn

[Q89] 判断表是否存在
来源：http://ij.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lk.panjiajie.cn

[Q90] 生成序号列
来源：http://uv.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://id.huixiangedu.cn

================================================================================
来源：http://gh.lnxyls.cn

R. Bash 专题
来源：http://la.szxytkj.cn

================================================================================
来源：http://sf.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://sq.colortex.cn

#!/usr/bin/env bash
来源：http://mg.colortex.cn

set -euo pipefail
来源：http://wg.hnjuh.cn

[R02] 变量赋值与使用
来源：http://el.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://cg.shtwfgs.cn

[R03] 只读变量
来源：http://iy.gzmigu.cn

readonly PI=3.14
来源：http://qr.gzmigu.cn

[R04] 位置参数
来源：http://ot.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bc.bjjhwx.cn

[R05] 参数默认值
来源：http://el.nicolike.cn

name="${1:-default}"
来源：http://fx.panjiajie.cn

[R06] 判断命令是否存在
来源：http://ju.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rg.szxytkj.cn

[R07] if 判断文件
来源：http://sp.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lg.bookmarksfly.cn

[R08] 数值比较
来源：http://dt.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wk.haigaiapp.cn

[R09] 字符串比较
来源：http://kk.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ux.huanxung.cn

[R10] 正则匹配
来源：http://gr.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ht.9csxet.cn

[R11] case 多分支
来源：http://il.yuexingan06.cn

case "$1" in
来源：http://za.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://vc.szxytkj.cn

stop)  echo "停止" ;;
来源：http://zj.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://an.haigaiapp.cn

esac
来源：http://dn.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://qh.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://tc.shtwfgs.cn

[R13] for 计数循环
来源：http://uf.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://bb.hahajie.cn

[R14] C 风格 for
来源：http://wo.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lu.shxzukj.cn

[R15] while 逐行读文件
来源：http://rc.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iw.jctech888.com.cn

[R16] until 等待条件
来源：http://ip.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://we.shtwfgs.cn

[R17] 数组定义与取值
来源：http://eg.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yq.hnjuh.cn

[R18] 遍历数组
来源：http://fq.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xa.lnxyls.cn

[R19] 数组长度
来源：http://ws.shtwfgs.cn

echo "${#arr[@]}"
来源：http://kt.nicolike.cn

[R20] 关联数组（字典）
来源：http://yp.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lw.9csxet.cn

[R21] 字符串长度
来源：http://rs.panjiajie.cn

echo "${#s}"
来源：http://eq.nszjky.cn

[R22] 截取子串
来源：http://zo.szsharing.cn

echo "${s:0:5}"
来源：http://jq.hahajie.cn

[R23] 字符串替换
来源：http://ek.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zi.haigaiapp.cn

[R24] 大小写转换
来源：http://wi.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fe.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://mt.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fj.hnjuh.cn

[R26] 命令替换
来源：http://um.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://yp.panjiajie.cn

[R27] 算术展开
来源：http://tz.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://rg.haigaiapp.cn

[R28] 浮点运算
来源：http://rk.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://jm.newstarts.cn

[R29] 定义函数
来源：http://kg.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rc.hnjuh.cn

[R30] 函数返回状态码
来源：http://ja.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://og.shtwfgs.cn

[R31] 局部变量
来源：http://td.521024.cn

f() { local x=1; echo "$x"; }
来源：http://dc.yuexingan06.cn

[R32] 参数个数校验
来源：http://iq.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hh.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://zr.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vt.yuexingan06.cn

[R34] 退出时清理
来源：http://jp.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://in.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://si.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://io.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://gd.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gy.9csxet.cn

[R37] 把输出赋给变量
来源：http://vh.bookmarksfly.cn

files=$(ls -1)
来源：http://xr.szxytkj.cn

[R38] 管道串联
来源：http://nv.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://tn.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://ox.nszjky.cn

cmd > out.log 2>&1
来源：http://cl.nszjky.cn

[R40] 追加写日志
来源：http://kd.szxytkj.cn

echo "log" >> out.log
来源：http://tm.colortex.cn

[R41] 丢弃输出
来源：http://ac.521024.cn

cmd >/dev/null 2>&1
来源：http://ta.nicolike.cn

[R42] 输入重定向
来源：http://wa.wgjwhj.cn

wc -l < a.txt
来源：http://we.shxzukj.cn

[R43] 按名字查找文件
来源：http://rh.haigaiapp.cn

find . -name "*.log" -type f
来源：http://gt.huanxung.cn

[R44] 按修改时间查找
来源：http://ir.shtwfgs.cn

find . -mtime -7 -type f
来源：http://rf.nszjky.cn

[R45] 批量删除
来源：http://pn.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://mr.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://yq.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wv.hahajie.cn

[R47] sed 单行替换
来源：http://rq.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ws.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://ug.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://ms.chemitech.net.cn

[R49] awk 带条件
来源：http://ll.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ls.huixinmuqiang.cn

[R50] awk 求和
来源：http://ks.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wb.yuexingan06.cn

[R51] 排序去重取前几
来源：http://qq.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qk.asd995.cn

[R52] 统计行数
来源：http://ni.szsharing.cn

wc -l a.txt
来源：http://ue.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://nv.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uo.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://us.shxzukj.cn

diff a.txt b.txt
来源：http://ta.shxzukj.cn

[R55] 压缩与解压
来源：http://gd.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mj.gzmigu.cn

[R56] 远程拷贝
来源：http://yq.yuexingan06.cn

scp file user@host:/path/
来源：http://qi.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://ds.521024.cn

ssh user@host 'uptime'
来源：http://oz.jctech888.com.cn

[R58] 下载文件
来源：http://ej.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yf.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://kg.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fa.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://sc.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dp.521024.cn

[R61] 磁盘占用
来源：http://gy.521024.cn

df -h;  du -sh *
来源：http://vw.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://py.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://pq.gzmigu.cn

[R63] 内存与进程
来源：http://oi.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://ku.yuexingan06.cn

[R64] 结束进程
来源：http://mv.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://wi.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://av.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://md.shxzukj.cn

[R66] 定时任务
来源：http://vm.szxytkj.cn

crontab -e;  crontab -l
来源：http://bo.colortex.cn

[R67] 生成随机十六进制串
来源：http://ym.chemitech.net.cn

openssl rand -hex 16
来源：http://ir.shxzskj.cn

[R68] 计算文件校验值
来源：http://co.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pq.nicolike.cn

[R69] 生成随机密码
来源：http://vb.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://oo.szxytkj.cn

[R70] 时间戳与互转
来源：http://og.hahajie.cn

date +%s;  date -d @1700000000
来源：http://di.panjiajie.cn

[R71] 日期格式化
来源：http://fc.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ua.hnjuh.cn

[R72] 等待端口就绪
来源：http://cc.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gw.asd995.cn

[R73] 分割大日志
来源：http://xt.nszjky.cn

split -l 1000 big.log part_
来源：http://la.huixinmuqiang.cn

[R74] 批量重命名
来源：http://ja.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ch.shxzskj.cn

[R75] 导出环境变量
来源：http://wr.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://dy.shtwfgs.cn

[R76] 使用临时文件
来源：http://jr.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://og.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://hs.yuexingan06.cn

read -rp "请输入: " ans
来源：http://iz.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://gq.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yw.haigaiapp.cn

[R79] 解析命令行选项
来源：http://tb.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nn.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://ry.szsharing.cn

time ./run.sh
来源：http://il.wgjwhj.cn

================================================================================
来源：http://dt.haigaiapp.cn

S. C / C++ 专题
来源：http://ri.shxzskj.cn

================================================================================
来源：http://ng.jctech888.com.cn

[S01] C：Hello World
来源：http://dz.nszjky.cn

#include <stdio.h>
来源：http://ho.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ef.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://jc.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://aj.jianghongdianzi.cn

[S03] C：读入整数
来源：http://jl.521024.cn

int x; scanf("%d", &x);
来源：http://ks.shxzukj.cn

[S04] C：字符串复制
来源：http://vf.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nc.shxzskj.cn

[S05] C：字符串长度
来源：http://bj.yuexingan06.cn

strlen(s)
来源：http://tm.hnjuh.cn

[S06] C：字符串比较
来源：http://zd.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://dr.hnjuh.cn

[S07] C：数组遍历求和
来源：http://uo.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ju.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://vn.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gi.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://ju.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vn.muxihuayi.cn

[S10] C：指针与解引用
来源：http://ar.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://ov.szsharing.cn

[S11] C：逐行读文件
来源：http://su.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://eb.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ka.nszjky.cn

fclose(f);
来源：http://qg.jianghongdianzi.cn

[S12] C：写文件
来源：http://ap.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vk.szxytkj.cn

[S13] C：宏定义
来源：http://vd.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fx.asd995.cn

[S14] C：枚举
来源：http://bp.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://hv.hahajie.cn

[S15] C：类型转换
来源：http://lh.bjjhwx.cn

(double) a / b
来源：http://fb.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://da.lnxyls.cn

x |= (1 << 3);
来源：http://ic.nszjky.cn

[S17] C：安全拼接字符串
来源：http://xu.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://el.9csxet.cn

[S18] C：命令行参数
来源：http://uy.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://fb.huanxung.cn

[S19] C：快速排序
来源：http://yp.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://js.9csxet.cn

[S20] C：二分查找
来源：http://qa.hnjuh.cn


<!-- 参考信息 -->