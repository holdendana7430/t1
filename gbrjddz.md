代发 wailian999

[Q44] IN 子查询
来源：http://oo.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qh.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://ns.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zh.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wi.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xb.szsharing.cn

[Q47] 与平均值比较
来源：http://sn.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gj.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://xx.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jv.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ar.shtwfgs.cn

[Q49] 更新单行
来源：http://js.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wk.hnjuh.cn

[Q50] 批量更新
来源：http://dp.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eh.nicolike.cn

[Q51] 用子查询更新
来源：http://xg.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zy.shxzskj.cn

[Q52] 删除指定行
来源：http://ue.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://ug.szxytkj.cn

[Q53] 按条件删除
来源：http://kj.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xf.huanxung.cn

[Q54] 清空表
来源：http://qo.hahajie.cn

TRUNCATE TABLE logs;
来源：http://vi.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://es.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dp.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://gt.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://az.gzmigu.cn

[Q57] 行号
来源：http://jc.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fu.521024.cn

[Q58] 累计求和
来源：http://kw.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xc.9csxet.cn

[Q59] 分组内累计
来源：http://ex.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zy.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://qd.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mw.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zq.shtwfgs.cn

[Q61] 移动平均
来源：http://yt.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bm.colortex.cn

[Q62] 分组占比
来源：http://ng.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fk.hahajie.cn

[Q63] 开启事务
来源：http://gx.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oy.nszjky.cn

[Q64] 提交事务
来源：http://sz.jianghongdianzi.cn

COMMIT;
来源：http://ot.newstarts.cn

[Q65] 回滚事务
来源：http://kt.nszjky.cn

ROLLBACK;
来源：http://rr.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://td.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gb.huanxung.cn

[Q67] 设置隔离级别
来源：http://bg.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xr.chemitech.net.cn

[Q68] 保存点
来源：http://ww.gzmigu.cn

SAVEPOINT sp1;
来源：http://yf.colortex.cn

ROLLBACK TO sp1;
来源：http://us.shxzskj.cn

[Q69] 查看执行计划
来源：http://jy.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://op.chemitech.net.cn

[Q70] 更新统计信息
来源：http://cn.asd995.cn

ANALYZE TABLE users;
来源：http://cz.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://em.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ts.521024.cn

[Q72] 查看索引
来源：http://ix.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://gq.bookmarksfly.cn

[Q73] 查看表状态
来源：http://uw.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vs.szxytkj.cn

[Q74] 强制使用索引
来源：http://lj.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fs.9csxet.cn

[Q75] 日期格式化
来源：http://hu.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dd.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lt.jctech888.com.cn

[Q76] 按天统计
来源：http://ls.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://di.shxzukj.cn

[Q77] 时间加减
来源：http://ry.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dn.shxzskj.cn

[Q78] 当前时间
来源：http://qe.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sc.newstarts.cn

[Q79] 字符串拼接
来源：http://ef.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zq.lnxyls.cn

[Q80] 字符串截取
来源：http://cs.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cz.szxytkj.cn

[Q81] 字符串替换
来源：http://rr.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qi.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://zl.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bb.huixiangedu.cn

[Q83] 大小写转换
来源：http://pp.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uf.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://ej.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://hd.muxihuayi.cn

[Q85] 数值取整
来源：http://ph.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qn.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://hy.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dx.colortex.cn

[Q87] JSON 字段做条件
来源：http://qc.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://is.521024.cn

[Q88] 行转列（条件聚合）
来源：http://vv.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iv.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ds.hahajie.cn

[Q89] 判断表是否存在
来源：http://fg.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sv.bjjhwx.cn

[Q90] 生成序号列
来源：http://bt.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cp.bookmarksfly.cn

================================================================================
来源：http://qn.panjiajie.cn

R. Bash 专题
来源：http://eo.521024.cn

================================================================================
来源：http://or.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://cj.jctech888.com.cn

#!/usr/bin/env bash
来源：http://ke.huanxung.cn

set -euo pipefail
来源：http://tk.shxzskj.cn

[R02] 变量赋值与使用
来源：http://rn.9csxet.cn

name="Tom"; echo "$name"
来源：http://mu.lnxyls.cn

[R03] 只读变量
来源：http://bf.lnxyls.cn

readonly PI=3.14
来源：http://zb.nszjky.cn

[R04] 位置参数
来源：http://uo.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pw.haigaiapp.cn

[R05] 参数默认值
来源：http://wj.521024.cn

name="${1:-default}"
来源：http://la.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://kz.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://if.haigaiapp.cn

[R07] if 判断文件
来源：http://ec.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bm.nicolike.cn

[R08] 数值比较
来源：http://cv.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://io.lnxyls.cn

[R09] 字符串比较
来源：http://ok.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gu.wgjwhj.cn

[R10] 正则匹配
来源：http://uf.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hu.szsharing.cn

[R11] case 多分支
来源：http://jq.wgjwhj.cn

case "$1" in
来源：http://hj.yuexingan06.cn

start) echo "启动" ;;
来源：http://xr.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://zq.newstarts.cn

*)     echo "未知命令" ;;
来源：http://ap.521024.cn

esac
来源：http://cr.shxzukj.cn

[R12] for 遍历文件
来源：http://zx.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://ok.hahajie.cn

[R13] for 计数循环
来源：http://wq.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://nj.bjjhwx.cn

[R14] C 风格 for
来源：http://fb.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lu.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://rc.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xu.asd995.cn

[R16] until 等待条件
来源：http://dv.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wf.shxzukj.cn

[R17] 数组定义与取值
来源：http://uz.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ra.nicolike.cn

[R18] 遍历数组
来源：http://qj.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gv.huixiangedu.cn

[R19] 数组长度
来源：http://we.9csxet.cn

echo "${#arr[@]}"
来源：http://cw.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://dv.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ur.521024.cn

[R21] 字符串长度
来源：http://de.yuexingan06.cn

echo "${#s}"
来源：http://ki.shxzukj.cn

[R22] 截取子串
来源：http://gv.chemitech.net.cn

echo "${s:0:5}"
来源：http://bi.521024.cn

[R23] 字符串替换
来源：http://yv.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dj.huanxung.cn

[R24] 大小写转换
来源：http://so.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mf.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://tl.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ze.newstarts.cn

[R26] 命令替换
来源：http://ro.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://qv.521024.cn

[R27] 算术展开
来源：http://ei.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://pf.chemitech.net.cn

[R28] 浮点运算
来源：http://iu.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://hw.nicolike.cn

[R29] 定义函数
来源：http://ph.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ci.colortex.cn

[R30] 函数返回状态码
来源：http://sj.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://rk.chemitech.net.cn

[R31] 局部变量
来源：http://dx.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://tx.wgjwhj.cn

[R32] 参数个数校验
来源：http://ve.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rn.colortex.cn

[R33] 捕获错误并提示行号
来源：http://nd.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mu.yuntaijiaju.cn

[R34] 退出时清理
来源：http://ar.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fb.wgjwhj.cn

[R35] 后台执行并等待
来源：http://dj.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yu.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://sj.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zy.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://to.shxzukj.cn

files=$(ls -1)
来源：http://fq.bjjhwx.cn

[R38] 管道串联
来源：http://gj.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://jt.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://ek.szsharing.cn

cmd > out.log 2>&1
来源：http://qz.chemitech.net.cn

[R40] 追加写日志
来源：http://ij.muxihuayi.cn

echo "log" >> out.log
来源：http://zv.lnxyls.cn

[R41] 丢弃输出
来源：http://ne.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://rx.nicolike.cn

[R42] 输入重定向
来源：http://jm.asd995.cn

wc -l < a.txt
来源：http://wz.nszjky.cn

[R43] 按名字查找文件
来源：http://up.szsharing.cn

find . -name "*.log" -type f
来源：http://kv.panjiajie.cn

[R44] 按修改时间查找
来源：http://ls.9csxet.cn

find . -mtime -7 -type f
来源：http://la.nicolike.cn

[R45] 批量删除
来源：http://ss.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://ri.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://ql.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ca.haigaiapp.cn

[R47] sed 单行替换
来源：http://bd.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://eq.chemitech.net.cn

[R48] awk 取指定列
来源：http://yb.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://hb.nszjky.cn

[R49] awk 带条件
来源：http://ep.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://io.yuntaijiaju.cn

[R50] awk 求和
来源：http://yw.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vl.shxzukj.cn

[R51] 排序去重取前几
来源：http://ig.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ag.szxytkj.cn

[R52] 统计行数
来源：http://tc.asd995.cn

wc -l a.txt
来源：http://qz.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://gs.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lk.huanxung.cn

[R54] 比较两个文件
来源：http://xo.szxytkj.cn

diff a.txt b.txt
来源：http://ep.colortex.cn

[R55] 压缩与解压
来源：http://kt.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xh.muxihuayi.cn

[R56] 远程拷贝
来源：http://jj.huixinmuqiang.cn

scp file user@host:/path/
来源：http://wd.nicolike.cn

[R57] 远程执行命令
来源：http://bd.huanxung.cn

ssh user@host 'uptime'
来源：http://se.jctech888.com.cn

[R58] 下载文件
来源：http://mg.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pj.hnjuh.cn

[R59] 发 POST JSON
来源：http://qd.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zh.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://ys.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kc.szxytkj.cn

[R61] 磁盘占用
来源：http://lp.yuexingan06.cn

df -h;  du -sh *
来源：http://yy.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://bj.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://lc.hahajie.cn

[R63] 内存与进程
来源：http://nu.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://hn.bookmarksfly.cn

[R64] 结束进程
来源：http://ha.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://nz.asd995.cn

[R65] 查看端口占用
来源：http://ji.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dd.lnxyls.cn

[R66] 定时任务
来源：http://nc.nicolike.cn

crontab -e;  crontab -l
来源：http://ev.521024.cn

[R67] 生成随机十六进制串
来源：http://mf.huixinmuqiang.cn

openssl rand -hex 16
来源：http://zn.lnxyls.cn

[R68] 计算文件校验值
来源：http://hi.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gr.gzmigu.cn

[R69] 生成随机密码
来源：http://ig.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://jy.nicolike.cn

[R70] 时间戳与互转
来源：http://zt.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://sx.asd995.cn

[R71] 日期格式化
来源：http://pa.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lk.gzmigu.cn

[R72] 等待端口就绪
来源：http://hj.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eh.nszjky.cn

[R73] 分割大日志
来源：http://lo.panjiajie.cn

split -l 1000 big.log part_
来源：http://vw.nicolike.cn

[R74] 批量重命名
来源：http://xv.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pe.newstarts.cn

[R75] 导出环境变量
来源：http://op.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://uc.szxytkj.cn

[R76] 使用临时文件
来源：http://mz.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yl.shxzskj.cn

[R77] 读取用户输入
来源：http://mw.chemitech.net.cn

read -rp "请输入: " ans
来源：http://lj.huixiangedu.cn

[R78] 交互式菜单
来源：http://rw.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fq.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://nc.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qu.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://er.shxzskj.cn

time ./run.sh
来源：http://na.muxihuayi.cn

================================================================================
来源：http://sq.gzmigu.cn

S. C / C++ 专题
来源：http://dw.gzmigu.cn

================================================================================
来源：http://iz.panjiajie.cn

[S01] C：Hello World
来源：http://sy.yuntaijiaju.cn

#include <stdio.h>
来源：http://he.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jw.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://xk.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://bj.bookmarksfly.cn

[S03] C：读入整数
来源：http://gk.asd995.cn

int x; scanf("%d", &x);
来源：http://gb.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://pi.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://do.jctech888.com.cn

[S05] C：字符串长度
来源：http://ka.szxytkj.cn

strlen(s)
来源：http://pr.gzmigu.cn

[S06] C：字符串比较
来源：http://xs.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://lh.szsharing.cn

[S07] C：数组遍历求和
来源：http://bq.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nh.521024.cn

[S08] C：动态内存分配与释放
来源：http://po.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lw.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://hx.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fb.newstarts.cn

[S10] C：指针与解引用
来源：http://tc.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://tc.bjjhwx.cn

[S11] C：逐行读文件
来源：http://yh.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://vy.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ou.bjjhwx.cn

fclose(f);
来源：http://fr.yuexingan06.cn

[S12] C：写文件
来源：http://ey.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gn.huixiangedu.cn

[S13] C：宏定义
来源：http://pb.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sf.shtwfgs.cn

[S14] C：枚举
来源：http://gq.bjjhwx.cn


<!-- 参考信息 -->