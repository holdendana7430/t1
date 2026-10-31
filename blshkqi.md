代发 wailian999

[Q48] CTE 公用表表达式
来源：http://uo.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ff.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://zt.shtwfgs.cn

[Q49] 更新单行
来源：http://sm.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xw.shxzskj.cn

[Q50] 批量更新
来源：http://ee.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qc.gzmigu.cn

[Q51] 用子查询更新
来源：http://nf.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tx.huanxung.cn

[Q52] 删除指定行
来源：http://xn.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://jq.shtwfgs.cn

[Q53] 按条件删除
来源：http://ky.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rb.szxytkj.cn

[Q54] 清空表
来源：http://hf.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://wr.asd995.cn

[Q55] 排名（并列占位）
来源：http://lb.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xr.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://lv.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kh.jianghongdianzi.cn

[Q57] 行号
来源：http://xi.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tn.huanxung.cn

[Q58] 累计求和
来源：http://yq.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iu.huixiangedu.cn

[Q59] 分组内累计
来源：http://va.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://np.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://ol.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gg.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yj.hahajie.cn

[Q61] 移动平均
来源：http://ic.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eo.521024.cn

[Q62] 分组占比
来源：http://vy.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jz.jianghongdianzi.cn

[Q63] 开启事务
来源：http://nf.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ky.bookmarksfly.cn

[Q64] 提交事务
来源：http://bf.wgjwhj.cn

COMMIT;
来源：http://yu.521024.cn

[Q65] 回滚事务
来源：http://zl.huixinmuqiang.cn

ROLLBACK;
来源：http://xw.bjjhwx.cn

[Q66] 行锁查询
来源：http://qo.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rs.asd995.cn

[Q67] 设置隔离级别
来源：http://qq.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pl.szxytkj.cn

[Q68] 保存点
来源：http://hw.panjiajie.cn

SAVEPOINT sp1;
来源：http://ss.521024.cn

ROLLBACK TO sp1;
来源：http://uv.colortex.cn

[Q69] 查看执行计划
来源：http://hi.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sv.bjjhwx.cn

[Q70] 更新统计信息
来源：http://nu.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://zf.newstarts.cn

[Q71] 查看建表语句
来源：http://yw.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lf.chemitech.net.cn

[Q72] 查看索引
来源：http://ss.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://mx.9csxet.cn

[Q73] 查看表状态
来源：http://pl.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yp.lnxyls.cn

[Q74] 强制使用索引
来源：http://ab.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ov.chemitech.net.cn

[Q75] 日期格式化
来源：http://jb.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fd.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://su.huanxung.cn

[Q76] 按天统计
来源：http://pb.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zs.shtwfgs.cn

[Q77] 时间加减
来源：http://qj.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vc.haigaiapp.cn

[Q78] 当前时间
来源：http://tg.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gt.szsharing.cn

[Q79] 字符串拼接
来源：http://nu.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xf.hahajie.cn

[Q80] 字符串截取
来源：http://xv.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lm.bookmarksfly.cn

[Q81] 字符串替换
来源：http://jp.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hx.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://ah.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ll.szxytkj.cn

[Q83] 大小写转换
来源：http://gx.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gg.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://dg.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://zz.hahajie.cn

[Q85] 数值取整
来源：http://pp.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cs.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://rx.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wh.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://bi.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iz.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://al.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ui.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zr.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://vg.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oy.huanxung.cn

[Q90] 生成序号列
来源：http://ta.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hy.bookmarksfly.cn

================================================================================
来源：http://ul.wgjwhj.cn

R. Bash 专题
来源：http://op.szsharing.cn

================================================================================
来源：http://ob.nicolike.cn

[R01] shebang 与严格模式
来源：http://zr.hnjuh.cn

#!/usr/bin/env bash
来源：http://ng.nicolike.cn

set -euo pipefail
来源：http://hn.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://xg.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://wq.jctech888.com.cn

[R03] 只读变量
来源：http://kd.wgjwhj.cn

readonly PI=3.14
来源：http://af.jctech888.com.cn

[R04] 位置参数
来源：http://wz.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yg.nszjky.cn

[R05] 参数默认值
来源：http://fw.asd995.cn

name="${1:-default}"
来源：http://xb.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://zt.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kt.bjjhwx.cn

[R07] if 判断文件
来源：http://pb.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ip.yuexingan06.cn

[R08] 数值比较
来源：http://dc.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://me.szxytkj.cn

[R09] 字符串比较
来源：http://fi.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qf.521024.cn

[R10] 正则匹配
来源：http://tm.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dh.nszjky.cn

[R11] case 多分支
来源：http://ud.chemitech.net.cn

case "$1" in
来源：http://qc.lnxyls.cn

start) echo "启动" ;;
来源：http://mg.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://sg.colortex.cn

*)     echo "未知命令" ;;
来源：http://rq.bjjhwx.cn

esac
来源：http://oa.gzmigu.cn

[R12] for 遍历文件
来源：http://rg.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://jt.jianghongdianzi.cn

[R13] for 计数循环
来源：http://sh.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://cl.521024.cn

[R14] C 风格 for
来源：http://zg.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ou.hnjuh.cn

[R15] while 逐行读文件
来源：http://hn.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fx.nszjky.cn

[R16] until 等待条件
来源：http://rl.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oe.szxytkj.cn

[R17] 数组定义与取值
来源：http://rw.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wt.nicolike.cn

[R18] 遍历数组
来源：http://aw.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nx.chemitech.net.cn

[R19] 数组长度
来源：http://cu.colortex.cn

echo "${#arr[@]}"
来源：http://eg.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://zb.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nr.shxzskj.cn

[R21] 字符串长度
来源：http://qf.huixinmuqiang.cn

echo "${#s}"
来源：http://uy.szxytkj.cn

[R22] 截取子串
来源：http://pz.9csxet.cn

echo "${s:0:5}"
来源：http://rs.shxzukj.cn

[R23] 字符串替换
来源：http://jk.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xx.huixiangedu.cn

[R24] 大小写转换
来源：http://oj.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sh.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://tg.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iv.nicolike.cn

[R26] 命令替换
来源：http://kw.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://dg.hahajie.cn

[R27] 算术展开
来源：http://bu.huanxung.cn

echo $((1 + 2 * 3))
来源：http://mw.huixiangedu.cn

[R28] 浮点运算
来源：http://eg.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://pl.521024.cn

[R29] 定义函数
来源：http://dl.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zg.szxytkj.cn

[R30] 函数返回状态码
来源：http://uu.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://dx.9csxet.cn

[R31] 局部变量
来源：http://bs.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://kc.shtwfgs.cn

[R32] 参数个数校验
来源：http://er.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://so.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://eu.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cj.nszjky.cn

[R34] 退出时清理
来源：http://tn.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ac.szxytkj.cn

[R35] 后台执行并等待
来源：http://vy.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kj.panjiajie.cn

[R36] 并发执行多个任务
来源：http://ox.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ut.lnxyls.cn

[R37] 把输出赋给变量
来源：http://ez.jianghongdianzi.cn

files=$(ls -1)
来源：http://fy.huixinmuqiang.cn

[R38] 管道串联
来源：http://pw.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://te.colortex.cn

[R39] 重定向标准输出与错误
来源：http://mv.hnjuh.cn

cmd > out.log 2>&1
来源：http://np.bjjhwx.cn

[R40] 追加写日志
来源：http://dk.haigaiapp.cn

echo "log" >> out.log
来源：http://eb.shxzskj.cn

[R41] 丢弃输出
来源：http://iz.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://od.chemitech.net.cn

[R42] 输入重定向
来源：http://bt.yuntaijiaju.cn

wc -l < a.txt
来源：http://oi.haigaiapp.cn

[R43] 按名字查找文件
来源：http://yx.jctech888.com.cn

find . -name "*.log" -type f
来源：http://cp.wgjwhj.cn

[R44] 按修改时间查找
来源：http://ir.shxzskj.cn

find . -mtime -7 -type f
来源：http://rc.shxzukj.cn

[R45] 批量删除
来源：http://xc.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://ai.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://jc.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ey.hnjuh.cn

[R47] sed 单行替换
来源：http://wo.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ec.shtwfgs.cn

[R48] awk 取指定列
来源：http://ka.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://bj.panjiajie.cn

[R49] awk 带条件
来源：http://cw.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lj.newstarts.cn

[R50] awk 求和
来源：http://hb.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hj.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://zo.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://op.haigaiapp.cn

[R52] 统计行数
来源：http://yd.nicolike.cn

wc -l a.txt
来源：http://xy.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://bo.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ly.bjjhwx.cn

[R54] 比较两个文件
来源：http://ve.hnjuh.cn

diff a.txt b.txt
来源：http://xi.shxzskj.cn

[R55] 压缩与解压
来源：http://qk.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ez.huanxung.cn

[R56] 远程拷贝
来源：http://ek.asd995.cn

scp file user@host:/path/
来源：http://rl.bjjhwx.cn

[R57] 远程执行命令
来源：http://op.jctech888.com.cn

ssh user@host 'uptime'
来源：http://ps.lnxyls.cn

[R58] 下载文件
来源：http://rp.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jp.szxytkj.cn

[R59] 发 POST JSON
来源：http://eu.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nl.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://jf.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://id.bjjhwx.cn

[R61] 磁盘占用
来源：http://pw.hnjuh.cn

df -h;  du -sh *
来源：http://qm.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://wk.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://sj.hnjuh.cn

[R63] 内存与进程
来源：http://mw.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://uw.haigaiapp.cn

[R64] 结束进程
来源：http://eu.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://jl.jctech888.com.cn

[R65] 查看端口占用
来源：http://lb.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gl.szxytkj.cn

[R66] 定时任务
来源：http://hn.lnxyls.cn

crontab -e;  crontab -l
来源：http://et.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://gn.colortex.cn

openssl rand -hex 16
来源：http://un.gzmigu.cn

[R68] 计算文件校验值
来源：http://eu.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zf.gzmigu.cn

[R69] 生成随机密码
来源：http://ov.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://ae.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://bi.huanxung.cn

date +%s;  date -d @1700000000
来源：http://sh.shxzskj.cn

[R71] 日期格式化
来源：http://pp.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uu.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://ke.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vg.nicolike.cn

[R73] 分割大日志
来源：http://od.jctech888.com.cn

split -l 1000 big.log part_
来源：http://wm.chemitech.net.cn

[R74] 批量重命名
来源：http://dq.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mn.szxytkj.cn

[R75] 导出环境变量
来源：http://hr.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://rg.chemitech.net.cn

[R76] 使用临时文件
来源：http://rt.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vl.lnxyls.cn

[R77] 读取用户输入
来源：http://ya.521024.cn

read -rp "请输入: " ans
来源：http://ss.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://gp.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cb.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://wq.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pq.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://ba.jianghongdianzi.cn

time ./run.sh
来源：http://nt.bjjhwx.cn

================================================================================
来源：http://zc.jctech888.com.cn

S. C / C++ 专题
来源：http://bv.yuexingan06.cn

================================================================================
来源：http://kk.szxytkj.cn

[S01] C：Hello World
来源：http://mj.jianghongdianzi.cn

#include <stdio.h>
来源：http://lj.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://au.9csxet.cn

[S02] C：变量与格式化输出
来源：http://qo.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://yw.9csxet.cn

[S03] C：读入整数
来源：http://xo.nszjky.cn

int x; scanf("%d", &x);
来源：http://ux.yuexingan06.cn

[S04] C：字符串复制
来源：http://jo.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qi.nicolike.cn

[S05] C：字符串长度
来源：http://al.chemitech.net.cn

strlen(s)
来源：http://ui.nicolike.cn

[S06] C：字符串比较
来源：http://rr.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://jf.huanxung.cn

[S07] C：数组遍历求和
来源：http://mh.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vr.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ln.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bn.asd995.cn

[S09] C：结构体定义与初始化
来源：http://yk.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ah.gzmigu.cn

[S10] C：指针与解引用
来源：http://oc.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://um.gzmigu.cn

[S11] C：逐行读文件
来源：http://kp.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://cz.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bc.jianghongdianzi.cn

fclose(f);
来源：http://ti.shxzskj.cn

[S12] C：写文件
来源：http://qi.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zg.haigaiapp.cn

[S13] C：宏定义
来源：http://nv.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ck.newstarts.cn

[S14] C：枚举
来源：http://ww.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://wv.szxytkj.cn

[S15] C：类型转换
来源：http://mc.gzmigu.cn

(double) a / b
来源：http://vn.colortex.cn

[S16] C：位操作置位
来源：http://xz.jctech888.com.cn

x |= (1 << 3);
来源：http://bj.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://cg.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yy.jctech888.com.cn

[S18] C：命令行参数
来源：http://wq.yuexingan06.cn


<!-- 参考信息 -->