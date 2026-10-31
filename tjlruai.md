代发 wailian999

[Q44] IN 子查询
来源：http://em.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xy.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://dq.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bh.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wa.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ng.shxzukj.cn

[Q47] 与平均值比较
来源：http://nz.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ed.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://qw.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fh.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://ru.jianghongdianzi.cn

[Q49] 更新单行
来源：http://xr.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ew.9csxet.cn

[Q50] 批量更新
来源：http://fl.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lc.bjjhwx.cn

[Q51] 用子查询更新
来源：http://qh.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ml.shxzukj.cn

[Q52] 删除指定行
来源：http://lm.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://cz.jctech888.com.cn

[Q53] 按条件删除
来源：http://oc.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ov.szsharing.cn

[Q54] 清空表
来源：http://iv.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://ds.szsharing.cn

[Q55] 排名（并列占位）
来源：http://fe.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uh.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://zh.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ka.lnxyls.cn

[Q57] 行号
来源：http://za.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://os.shxzukj.cn

[Q58] 累计求和
来源：http://qd.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://om.huanxung.cn

[Q59] 分组内累计
来源：http://tg.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fe.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://ex.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pb.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fv.nicolike.cn

[Q61] 移动平均
来源：http://mm.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jv.huixiangedu.cn

[Q62] 分组占比
来源：http://ys.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vv.panjiajie.cn

[Q63] 开启事务
来源：http://ri.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uj.wgjwhj.cn

[Q64] 提交事务
来源：http://jo.szsharing.cn

COMMIT;
来源：http://wu.szxytkj.cn

[Q65] 回滚事务
来源：http://qj.bookmarksfly.cn

ROLLBACK;
来源：http://du.shtwfgs.cn

[Q66] 行锁查询
来源：http://qs.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sh.colortex.cn

[Q67] 设置隔离级别
来源：http://ab.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tj.yuntaijiaju.cn

[Q68] 保存点
来源：http://zd.muxihuayi.cn

SAVEPOINT sp1;
来源：http://ed.nicolike.cn

ROLLBACK TO sp1;
来源：http://jm.wgjwhj.cn

[Q69] 查看执行计划
来源：http://cy.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lj.hahajie.cn

[Q70] 更新统计信息
来源：http://vv.chemitech.net.cn

ANALYZE TABLE users;
来源：http://bc.szxytkj.cn

[Q71] 查看建表语句
来源：http://gd.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tt.szsharing.cn

[Q72] 查看索引
来源：http://hg.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://pe.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://yo.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ui.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://xa.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ri.colortex.cn

[Q75] 日期格式化
来源：http://vy.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qf.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hh.gzmigu.cn

[Q76] 按天统计
来源：http://bs.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wm.jctech888.com.cn

[Q77] 时间加减
来源：http://ug.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jd.hnjuh.cn

[Q78] 当前时间
来源：http://rn.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zn.huixiangedu.cn

[Q79] 字符串拼接
来源：http://zw.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://af.asd995.cn

[Q80] 字符串截取
来源：http://qa.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rp.yuexingan06.cn

[Q81] 字符串替换
来源：http://kb.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kc.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://qv.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ey.shxzukj.cn

[Q83] 大小写转换
来源：http://po.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://na.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://pl.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://ak.chemitech.net.cn

[Q85] 数值取整
来源：http://mf.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tp.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://er.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ix.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://cx.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ow.521024.cn

[Q88] 行转列（条件聚合）
来源：http://zt.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ma.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jl.shxzskj.cn

[Q89] 判断表是否存在
来源：http://qh.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yc.szsharing.cn

[Q90] 生成序号列
来源：http://bg.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vw.muxihuayi.cn

================================================================================
来源：http://xt.muxihuayi.cn

R. Bash 专题
来源：http://po.jianghongdianzi.cn

================================================================================
来源：http://oi.huanxung.cn

[R01] shebang 与严格模式
来源：http://nz.9csxet.cn

#!/usr/bin/env bash
来源：http://le.huixinmuqiang.cn

set -euo pipefail
来源：http://eh.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://nb.asd995.cn

name="Tom"; echo "$name"
来源：http://zx.huixinmuqiang.cn

[R03] 只读变量
来源：http://ra.521024.cn

readonly PI=3.14
来源：http://lm.colortex.cn

[R04] 位置参数
来源：http://mu.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rl.521024.cn

[R05] 参数默认值
来源：http://wb.shxzskj.cn

name="${1:-default}"
来源：http://st.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://mr.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xq.panjiajie.cn

[R07] if 判断文件
来源：http://rv.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qo.hahajie.cn

[R08] 数值比较
来源：http://cd.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uk.panjiajie.cn

[R09] 字符串比较
来源：http://ff.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pi.haigaiapp.cn

[R10] 正则匹配
来源：http://yv.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mc.shxzskj.cn

[R11] case 多分支
来源：http://iz.colortex.cn

case "$1" in
来源：http://ox.szsharing.cn

start) echo "启动" ;;
来源：http://un.lnxyls.cn

stop)  echo "停止" ;;
来源：http://dn.nicolike.cn

*)     echo "未知命令" ;;
来源：http://ws.haigaiapp.cn

esac
来源：http://ux.haigaiapp.cn

[R12] for 遍历文件
来源：http://zm.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://ey.521024.cn

[R13] for 计数循环
来源：http://wj.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://pr.hahajie.cn

[R14] C 风格 for
来源：http://yo.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tg.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://wy.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ck.shtwfgs.cn

[R16] until 等待条件
来源：http://js.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sr.shtwfgs.cn

[R17] 数组定义与取值
来源：http://iv.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mn.chemitech.net.cn

[R18] 遍历数组
来源：http://xl.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yg.gzmigu.cn

[R19] 数组长度
来源：http://ir.nicolike.cn

echo "${#arr[@]}"
来源：http://um.lnxyls.cn

[R20] 关联数组（字典）
来源：http://wj.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rd.bjjhwx.cn

[R21] 字符串长度
来源：http://rx.szsharing.cn

echo "${#s}"
来源：http://ja.panjiajie.cn

[R22] 截取子串
来源：http://ot.panjiajie.cn

echo "${s:0:5}"
来源：http://rz.521024.cn

[R23] 字符串替换
来源：http://vd.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jo.shxzskj.cn

[R24] 大小写转换
来源：http://oj.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ze.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://wc.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xg.jctech888.com.cn

[R26] 命令替换
来源：http://wl.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://zn.shxzukj.cn

[R27] 算术展开
来源：http://mg.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://hs.yuexingan06.cn

[R28] 浮点运算
来源：http://wi.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://iq.jctech888.com.cn

[R29] 定义函数
来源：http://ny.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ye.shxzskj.cn

[R30] 函数返回状态码
来源：http://ph.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://fo.colortex.cn

[R31] 局部变量
来源：http://qq.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://xk.panjiajie.cn

[R32] 参数个数校验
来源：http://dg.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dz.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://gy.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nq.szxytkj.cn

[R34] 退出时清理
来源：http://mh.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qv.lnxyls.cn

[R35] 后台执行并等待
来源：http://qu.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ts.huanxung.cn

[R36] 并发执行多个任务
来源：http://sj.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vt.huanxung.cn

[R37] 把输出赋给变量
来源：http://tg.yuntaijiaju.cn

files=$(ls -1)
来源：http://xo.wgjwhj.cn

[R38] 管道串联
来源：http://za.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://xb.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://ot.shtwfgs.cn

cmd > out.log 2>&1
来源：http://pm.shxzukj.cn

[R40] 追加写日志
来源：http://tv.huanxung.cn

echo "log" >> out.log
来源：http://ua.nicolike.cn

[R41] 丢弃输出
来源：http://ch.521024.cn

cmd >/dev/null 2>&1
来源：http://cm.muxihuayi.cn

[R42] 输入重定向
来源：http://rl.bookmarksfly.cn

wc -l < a.txt
来源：http://bb.bjjhwx.cn

[R43] 按名字查找文件
来源：http://oy.chemitech.net.cn

find . -name "*.log" -type f
来源：http://cy.shxzukj.cn

[R44] 按修改时间查找
来源：http://os.jctech888.com.cn

find . -mtime -7 -type f
来源：http://cy.9csxet.cn

[R45] 批量删除
来源：http://rs.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://gx.nicolike.cn

[R46] 递归替换文件内容
来源：http://ed.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://de.shxzskj.cn

[R47] sed 单行替换
来源：http://uz.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://eg.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://ng.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://sv.jianghongdianzi.cn

[R49] awk 带条件
来源：http://qz.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mg.haigaiapp.cn

[R50] awk 求和
来源：http://tt.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ou.asd995.cn

[R51] 排序去重取前几
来源：http://wj.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sw.muxihuayi.cn

[R52] 统计行数
来源：http://mu.asd995.cn

wc -l a.txt
来源：http://jj.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://zy.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sl.9csxet.cn

[R54] 比较两个文件
来源：http://ul.jctech888.com.cn

diff a.txt b.txt
来源：http://kq.gzmigu.cn

[R55] 压缩与解压
来源：http://sd.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ad.bookmarksfly.cn

[R56] 远程拷贝
来源：http://vw.jianghongdianzi.cn

scp file user@host:/path/
来源：http://kh.colortex.cn

[R57] 远程执行命令
来源：http://zd.nicolike.cn

ssh user@host 'uptime'
来源：http://vz.huixiangedu.cn

[R58] 下载文件
来源：http://zm.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zx.chemitech.net.cn

[R59] 发 POST JSON
来源：http://dc.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sf.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://nc.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zu.muxihuayi.cn

[R61] 磁盘占用
来源：http://kv.9csxet.cn

df -h;  du -sh *
来源：http://zn.huanxung.cn

[R62] 找最占空间的文件
来源：http://hb.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://kg.huixinmuqiang.cn

[R63] 内存与进程
来源：http://vp.521024.cn

free -h;  ps aux | grep nginx
来源：http://jl.lnxyls.cn

[R64] 结束进程
来源：http://ln.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://kq.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://bx.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nf.521024.cn

[R66] 定时任务
来源：http://mn.szsharing.cn

crontab -e;  crontab -l
来源：http://et.colortex.cn

[R67] 生成随机十六进制串
来源：http://of.lnxyls.cn

openssl rand -hex 16
来源：http://sh.shxzskj.cn

[R68] 计算文件校验值
来源：http://ac.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fm.hnjuh.cn

[R69] 生成随机密码
来源：http://do.521024.cn

head -c 16 /dev/urandom | base64
来源：http://vj.nszjky.cn

[R70] 时间戳与互转
来源：http://on.hahajie.cn

date +%s;  date -d @1700000000
来源：http://gd.9csxet.cn

[R71] 日期格式化
来源：http://eq.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tw.newstarts.cn

[R72] 等待端口就绪
来源：http://uz.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zn.huixiangedu.cn

[R73] 分割大日志
来源：http://jq.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://qs.521024.cn

[R74] 批量重命名
来源：http://bk.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ri.huixiangedu.cn

[R75] 导出环境变量
来源：http://dj.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://pg.jctech888.com.cn

[R76] 使用临时文件
来源：http://ig.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wv.newstarts.cn

[R77] 读取用户输入
来源：http://hu.newstarts.cn

read -rp "请输入: " ans
来源：http://aj.asd995.cn

[R78] 交互式菜单
来源：http://db.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oj.muxihuayi.cn

[R79] 解析命令行选项
来源：http://ob.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://px.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://uc.bookmarksfly.cn

time ./run.sh
来源：http://fj.9csxet.cn

================================================================================
来源：http://lz.panjiajie.cn

S. C / C++ 专题
来源：http://jv.szxytkj.cn

================================================================================
来源：http://ee.jctech888.com.cn

[S01] C：Hello World
来源：http://bq.shtwfgs.cn

#include <stdio.h>
来源：http://bh.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://te.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://yw.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://re.jctech888.com.cn

[S03] C：读入整数
来源：http://yp.szsharing.cn

int x; scanf("%d", &x);
来源：http://qj.haigaiapp.cn

[S04] C：字符串复制
来源：http://fe.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://us.newstarts.cn

[S05] C：字符串长度
来源：http://dv.asd995.cn

strlen(s)
来源：http://ll.shxzukj.cn

[S06] C：字符串比较
来源：http://la.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://mr.asd995.cn

[S07] C：数组遍历求和
来源：http://ah.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yl.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://eu.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vo.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://ah.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bc.521024.cn

[S10] C：指针与解引用
来源：http://ve.hahajie.cn

int *p = &a;  *p = 5;
来源：http://ao.muxihuayi.cn

[S11] C：逐行读文件
来源：http://km.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://xx.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ce.jctech888.com.cn

fclose(f);
来源：http://yg.newstarts.cn

[S12] C：写文件
来源：http://rr.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zf.szxytkj.cn

[S13] C：宏定义
来源：http://pw.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qk.asd995.cn

[S14] C：枚举
来源：http://fr.huanxung.cn


<!-- 参考信息 -->