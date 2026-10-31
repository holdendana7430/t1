代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://af.huanxung.cn

[Q50] 批量更新
来源：http://df.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eo.shtwfgs.cn

[Q51] 用子查询更新
来源：http://tz.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://up.colortex.cn

[Q52] 删除指定行
来源：http://ee.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://vu.wgjwhj.cn

[Q53] 按条件删除
来源：http://qn.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sz.shtwfgs.cn

[Q54] 清空表
来源：http://ko.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://pj.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://sn.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yk.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://cn.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://as.hahajie.cn

[Q57] 行号
来源：http://xj.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fl.hahajie.cn

[Q58] 累计求和
来源：http://to.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fm.haigaiapp.cn

[Q59] 分组内累计
来源：http://so.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fh.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://nq.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tu.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lg.jctech888.com.cn

[Q61] 移动平均
来源：http://xx.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://an.panjiajie.cn

[Q62] 分组占比
来源：http://gu.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cl.hahajie.cn

[Q63] 开启事务
来源：http://ls.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iw.yuntaijiaju.cn

[Q64] 提交事务
来源：http://vv.shtwfgs.cn

COMMIT;
来源：http://ui.shxzukj.cn

[Q65] 回滚事务
来源：http://tw.huixiangedu.cn

ROLLBACK;
来源：http://sv.lnxyls.cn

[Q66] 行锁查询
来源：http://cm.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xs.gzmigu.cn

[Q67] 设置隔离级别
来源：http://vb.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://so.521024.cn

[Q68] 保存点
来源：http://it.hahajie.cn

SAVEPOINT sp1;
来源：http://at.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://ps.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://ot.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gh.newstarts.cn

[Q70] 更新统计信息
来源：http://hv.asd995.cn

ANALYZE TABLE users;
来源：http://he.haigaiapp.cn

[Q71] 查看建表语句
来源：http://sg.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://as.lnxyls.cn

[Q72] 查看索引
来源：http://vn.9csxet.cn

SHOW INDEX FROM users;
来源：http://jh.hnjuh.cn

[Q73] 查看表状态
来源：http://mk.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://it.muxihuayi.cn

[Q74] 强制使用索引
来源：http://fo.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cs.nicolike.cn

[Q75] 日期格式化
来源：http://ns.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wj.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jx.haigaiapp.cn

[Q76] 按天统计
来源：http://zk.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://te.hnjuh.cn

[Q77] 时间加减
来源：http://fm.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tb.szxytkj.cn

[Q78] 当前时间
来源：http://hr.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yn.haigaiapp.cn

[Q79] 字符串拼接
来源：http://su.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ug.newstarts.cn

[Q80] 字符串截取
来源：http://lu.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iz.bjjhwx.cn

[Q81] 字符串替换
来源：http://we.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jv.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://pq.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nz.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://ld.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bt.newstarts.cn

[Q84] 去除首尾空格
来源：http://ky.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://yn.shxzukj.cn

[Q85] 数值取整
来源：http://uu.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dw.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://zn.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cr.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://jk.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kl.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://af.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://au.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rm.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://tr.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ms.shxzukj.cn

[Q90] 生成序号列
来源：http://av.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dk.szxytkj.cn

================================================================================
来源：http://pd.colortex.cn

R. Bash 专题
来源：http://fh.szxytkj.cn

================================================================================
来源：http://jc.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://tt.huixiangedu.cn

#!/usr/bin/env bash
来源：http://fb.bookmarksfly.cn

set -euo pipefail
来源：http://sa.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://nk.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://bg.muxihuayi.cn

[R03] 只读变量
来源：http://uc.muxihuayi.cn

readonly PI=3.14
来源：http://jr.gzmigu.cn

[R04] 位置参数
来源：http://lo.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ng.panjiajie.cn

[R05] 参数默认值
来源：http://na.yuntaijiaju.cn

name="${1:-default}"
来源：http://ls.lnxyls.cn

[R06] 判断命令是否存在
来源：http://bb.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eb.nicolike.cn

[R07] if 判断文件
来源：http://ic.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ju.bjjhwx.cn

[R08] 数值比较
来源：http://vd.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://on.yuexingan06.cn

[R09] 字符串比较
来源：http://bd.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tp.yuexingan06.cn

[R10] 正则匹配
来源：http://tg.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zp.9csxet.cn

[R11] case 多分支
来源：http://st.521024.cn

case "$1" in
来源：http://so.panjiajie.cn

start) echo "启动" ;;
来源：http://ou.asd995.cn

stop)  echo "停止" ;;
来源：http://xb.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://qh.521024.cn

esac
来源：http://ll.lnxyls.cn

[R12] for 遍历文件
来源：http://wa.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://pv.haigaiapp.cn

[R13] for 计数循环
来源：http://xh.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://ik.hahajie.cn

[R14] C 风格 for
来源：http://xt.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tp.panjiajie.cn

[R15] while 逐行读文件
来源：http://de.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pc.yuntaijiaju.cn

[R16] until 等待条件
来源：http://rv.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bj.huixiangedu.cn

[R17] 数组定义与取值
来源：http://hn.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hn.wgjwhj.cn

[R18] 遍历数组
来源：http://cm.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mr.gzmigu.cn

[R19] 数组长度
来源：http://nc.hnjuh.cn

echo "${#arr[@]}"
来源：http://pe.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://se.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://za.huanxung.cn

[R21] 字符串长度
来源：http://vg.yuexingan06.cn

echo "${#s}"
来源：http://av.shxzukj.cn

[R22] 截取子串
来源：http://ra.newstarts.cn

echo "${s:0:5}"
来源：http://nl.lnxyls.cn

[R23] 字符串替换
来源：http://sz.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fj.huixiangedu.cn

[R24] 大小写转换
来源：http://ul.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cq.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://hv.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rz.szsharing.cn

[R26] 命令替换
来源：http://hi.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://lv.bjjhwx.cn

[R27] 算术展开
来源：http://cw.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://xg.shxzukj.cn

[R28] 浮点运算
来源：http://wp.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://ni.panjiajie.cn

[R29] 定义函数
来源：http://fl.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fi.huixiangedu.cn

[R30] 函数返回状态码
来源：http://nt.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://bp.chemitech.net.cn

[R31] 局部变量
来源：http://oi.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://qo.bjjhwx.cn

[R32] 参数个数校验
来源：http://cg.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ds.asd995.cn

[R33] 捕获错误并提示行号
来源：http://ik.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ca.chemitech.net.cn

[R34] 退出时清理
来源：http://es.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wo.colortex.cn

[R35] 后台执行并等待
来源：http://mn.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ef.nszjky.cn

[R36] 并发执行多个任务
来源：http://mr.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uh.panjiajie.cn

[R37] 把输出赋给变量
来源：http://ox.huixiangedu.cn

files=$(ls -1)
来源：http://wy.asd995.cn

[R38] 管道串联
来源：http://ly.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://ew.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://le.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://ek.nicolike.cn

[R40] 追加写日志
来源：http://ra.yuntaijiaju.cn

echo "log" >> out.log
来源：http://js.panjiajie.cn

[R41] 丢弃输出
来源：http://ql.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://rj.bookmarksfly.cn

[R42] 输入重定向
来源：http://kj.colortex.cn

wc -l < a.txt
来源：http://qv.panjiajie.cn

[R43] 按名字查找文件
来源：http://bf.newstarts.cn

find . -name "*.log" -type f
来源：http://qt.jctech888.com.cn

[R44] 按修改时间查找
来源：http://de.newstarts.cn

find . -mtime -7 -type f
来源：http://yf.521024.cn

[R45] 批量删除
来源：http://rf.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://jr.panjiajie.cn

[R46] 递归替换文件内容
来源：http://mf.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://li.hahajie.cn

[R47] sed 单行替换
来源：http://qd.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fk.szsharing.cn

[R48] awk 取指定列
来源：http://hk.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://ti.huixinmuqiang.cn

[R49] awk 带条件
来源：http://od.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rm.9csxet.cn

[R50] awk 求和
来源：http://kg.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kj.9csxet.cn

[R51] 排序去重取前几
来源：http://rk.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://to.jctech888.com.cn

[R52] 统计行数
来源：http://ji.jianghongdianzi.cn

wc -l a.txt
来源：http://dc.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://an.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tf.shxzskj.cn

[R54] 比较两个文件
来源：http://kg.jctech888.com.cn

diff a.txt b.txt
来源：http://wf.shxzukj.cn

[R55] 压缩与解压
来源：http://qf.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bz.wgjwhj.cn

[R56] 远程拷贝
来源：http://eu.yuexingan06.cn

scp file user@host:/path/
来源：http://pm.nicolike.cn

[R57] 远程执行命令
来源：http://kx.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://ag.bjjhwx.cn

[R58] 下载文件
来源：http://mz.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ds.9csxet.cn

[R59] 发 POST JSON
来源：http://af.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tb.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://lo.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xe.colortex.cn

[R61] 磁盘占用
来源：http://hs.521024.cn

df -h;  du -sh *
来源：http://of.colortex.cn

[R62] 找最占空间的文件
来源：http://ot.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://om.bookmarksfly.cn

[R63] 内存与进程
来源：http://dy.asd995.cn

free -h;  ps aux | grep nginx
来源：http://rc.yuntaijiaju.cn

[R64] 结束进程
来源：http://am.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://wd.bookmarksfly.cn

[R65] 查看端口占用
来源：http://qk.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ym.szsharing.cn

[R66] 定时任务
来源：http://hn.hahajie.cn

crontab -e;  crontab -l
来源：http://ga.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://df.hnjuh.cn

openssl rand -hex 16
来源：http://xe.nszjky.cn

[R68] 计算文件校验值
来源：http://ln.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ae.nicolike.cn

[R69] 生成随机密码
来源：http://hi.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://fl.bjjhwx.cn

[R70] 时间戳与互转
来源：http://cu.szsharing.cn

date +%s;  date -d @1700000000
来源：http://mb.bookmarksfly.cn

[R71] 日期格式化
来源：http://ps.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yq.newstarts.cn

[R72] 等待端口就绪
来源：http://fp.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cj.muxihuayi.cn

[R73] 分割大日志
来源：http://df.521024.cn

split -l 1000 big.log part_
来源：http://hy.haigaiapp.cn

[R74] 批量重命名
来源：http://wn.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mb.newstarts.cn

[R75] 导出环境变量
来源：http://qk.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://jy.hnjuh.cn

[R76] 使用临时文件
来源：http://wg.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zv.yuexingan06.cn

[R77] 读取用户输入
来源：http://tn.huanxung.cn

read -rp "请输入: " ans
来源：http://bc.chemitech.net.cn

[R78] 交互式菜单
来源：http://fw.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tu.nszjky.cn

[R79] 解析命令行选项
来源：http://sw.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sj.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://gd.muxihuayi.cn

time ./run.sh
来源：http://tp.szsharing.cn

================================================================================
来源：http://ey.yuntaijiaju.cn

S. C / C++ 专题
来源：http://cs.szsharing.cn

================================================================================
来源：http://qp.newstarts.cn

[S01] C：Hello World
来源：http://id.asd995.cn

#include <stdio.h>
来源：http://jf.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ew.hahajie.cn

[S02] C：变量与格式化输出
来源：http://db.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://ew.shxzskj.cn

[S03] C：读入整数
来源：http://hf.szsharing.cn

int x; scanf("%d", &x);
来源：http://fz.jctech888.com.cn

[S04] C：字符串复制
来源：http://xj.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zj.gzmigu.cn

[S05] C：字符串长度
来源：http://bd.jctech888.com.cn

strlen(s)
来源：http://fv.shtwfgs.cn

[S06] C：字符串比较
来源：http://dj.panjiajie.cn

strcmp(a, b) == 0
来源：http://ru.521024.cn

[S07] C：数组遍历求和
来源：http://xw.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tf.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://qp.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://my.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://hb.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pm.asd995.cn

[S10] C：指针与解引用
来源：http://qw.colortex.cn

int *p = &a;  *p = 5;
来源：http://bs.hahajie.cn

[S11] C：逐行读文件
来源：http://ay.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://fw.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pu.yuntaijiaju.cn

fclose(f);
来源：http://yy.asd995.cn

[S12] C：写文件
来源：http://pi.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pp.yuntaijiaju.cn

[S13] C：宏定义
来源：http://yl.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://le.gzmigu.cn

[S14] C：枚举
来源：http://sz.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://er.asd995.cn

[S15] C：类型转换
来源：http://ek.haigaiapp.cn

(double) a / b
来源：http://fm.muxihuayi.cn

[S16] C：位操作置位
来源：http://gp.9csxet.cn

x |= (1 << 3);
来源：http://pz.newstarts.cn

[S17] C：安全拼接字符串
来源：http://fz.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hy.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://fa.521024.cn

int main(int argc, char **argv)
来源：http://fl.yuntaijiaju.cn

[S19] C：快速排序
来源：http://az.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ab.bookmarksfly.cn

[S20] C：二分查找
来源：http://vu.9csxet.cn


<!-- 参考信息 -->