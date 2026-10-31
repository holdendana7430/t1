代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://pu.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://es.shxzukj.cn

[Q43] 标量子查询
来源：http://fl.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yj.colortex.cn

[Q44] IN 子查询
来源：http://ih.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ud.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://ok.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hr.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sz.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://by.yuexingan06.cn

[Q47] 与平均值比较
来源：http://nb.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qp.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://fo.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://if.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://zh.yuexingan06.cn

[Q49] 更新单行
来源：http://rm.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tc.huanxung.cn

[Q50] 批量更新
来源：http://sc.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ni.muxihuayi.cn

[Q51] 用子查询更新
来源：http://lp.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rr.colortex.cn

[Q52] 删除指定行
来源：http://hc.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://rk.hahajie.cn

[Q53] 按条件删除
来源：http://xn.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lr.hnjuh.cn

[Q54] 清空表
来源：http://fk.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://wv.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://no.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uh.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://te.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gv.bookmarksfly.cn

[Q57] 行号
来源：http://xy.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pn.yuntaijiaju.cn

[Q58] 累计求和
来源：http://lx.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://le.haigaiapp.cn

[Q59] 分组内累计
来源：http://yl.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zl.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://yo.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wv.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oq.lnxyls.cn

[Q61] 移动平均
来源：http://jf.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mr.szxytkj.cn

[Q62] 分组占比
来源：http://bi.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ze.shxzukj.cn

[Q63] 开启事务
来源：http://py.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dz.hnjuh.cn

[Q64] 提交事务
来源：http://mi.bjjhwx.cn

COMMIT;
来源：http://un.asd995.cn

[Q65] 回滚事务
来源：http://xy.jianghongdianzi.cn

ROLLBACK;
来源：http://lu.wgjwhj.cn

[Q66] 行锁查询
来源：http://wl.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://md.hnjuh.cn

[Q67] 设置隔离级别
来源：http://lb.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xb.521024.cn

[Q68] 保存点
来源：http://gl.szsharing.cn

SAVEPOINT sp1;
来源：http://xv.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://qo.szxytkj.cn

[Q69] 查看执行计划
来源：http://aw.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bd.jctech888.com.cn

[Q70] 更新统计信息
来源：http://qh.colortex.cn

ANALYZE TABLE users;
来源：http://ka.9csxet.cn

[Q71] 查看建表语句
来源：http://so.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rh.gzmigu.cn

[Q72] 查看索引
来源：http://xe.shxzskj.cn

SHOW INDEX FROM users;
来源：http://xy.wgjwhj.cn

[Q73] 查看表状态
来源：http://ad.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://se.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://hv.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rn.huanxung.cn

[Q75] 日期格式化
来源：http://la.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jy.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cb.szsharing.cn

[Q76] 按天统计
来源：http://mu.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pi.shxzskj.cn

[Q77] 时间加减
来源：http://ql.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cu.yuexingan06.cn

[Q78] 当前时间
来源：http://fl.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://il.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://ut.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fy.nszjky.cn

[Q80] 字符串截取
来源：http://tq.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pc.szsharing.cn

[Q81] 字符串替换
来源：http://ad.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cj.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://rk.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sc.haigaiapp.cn

[Q83] 大小写转换
来源：http://wp.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ph.gzmigu.cn

[Q84] 去除首尾空格
来源：http://gl.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://gf.nszjky.cn

[Q85] 数值取整
来源：http://fb.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gt.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://gu.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jy.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://kw.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://by.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://et.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xg.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tz.panjiajie.cn

[Q89] 判断表是否存在
来源：http://fg.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cn.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://qg.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vz.shtwfgs.cn

================================================================================
来源：http://do.colortex.cn

R. Bash 专题
来源：http://eo.huixinmuqiang.cn

================================================================================
来源：http://oh.panjiajie.cn

[R01] shebang 与严格模式
来源：http://ld.szsharing.cn

#!/usr/bin/env bash
来源：http://sw.newstarts.cn

set -euo pipefail
来源：http://am.szsharing.cn

[R02] 变量赋值与使用
来源：http://iw.szsharing.cn

name="Tom"; echo "$name"
来源：http://vm.bjjhwx.cn

[R03] 只读变量
来源：http://gy.muxihuayi.cn

readonly PI=3.14
来源：http://yy.colortex.cn

[R04] 位置参数
来源：http://qi.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iy.huixinmuqiang.cn

[R05] 参数默认值
来源：http://xt.gzmigu.cn

name="${1:-default}"
来源：http://vp.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://vy.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qd.wgjwhj.cn

[R07] if 判断文件
来源：http://qz.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jd.muxihuayi.cn

[R08] 数值比较
来源：http://zo.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yq.panjiajie.cn

[R09] 字符串比较
来源：http://bv.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ee.huanxung.cn

[R10] 正则匹配
来源：http://qa.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yr.muxihuayi.cn

[R11] case 多分支
来源：http://vz.bookmarksfly.cn

case "$1" in
来源：http://vx.huanxung.cn

start) echo "启动" ;;
来源：http://ij.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://mx.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://mc.gzmigu.cn

esac
来源：http://fw.panjiajie.cn

[R12] for 遍历文件
来源：http://sk.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://jk.hahajie.cn

[R13] for 计数循环
来源：http://sk.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://af.szxytkj.cn

[R14] C 风格 for
来源：http://xn.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ea.szxytkj.cn

[R15] while 逐行读文件
来源：http://yr.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nr.bjjhwx.cn

[R16] until 等待条件
来源：http://me.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lm.lnxyls.cn

[R17] 数组定义与取值
来源：http://fz.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cu.huixiangedu.cn

[R18] 遍历数组
来源：http://cl.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cr.haigaiapp.cn

[R19] 数组长度
来源：http://dl.jctech888.com.cn

echo "${#arr[@]}"
来源：http://up.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://je.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fc.bjjhwx.cn

[R21] 字符串长度
来源：http://to.huanxung.cn

echo "${#s}"
来源：http://hv.shxzskj.cn

[R22] 截取子串
来源：http://ga.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://hq.lnxyls.cn

[R23] 字符串替换
来源：http://qf.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xu.szxytkj.cn

[R24] 大小写转换
来源：http://hn.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xe.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://sk.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ac.521024.cn

[R26] 命令替换
来源：http://ap.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://sb.bjjhwx.cn

[R27] 算术展开
来源：http://yx.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://nq.shxzukj.cn

[R28] 浮点运算
来源：http://vr.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://my.9csxet.cn

[R29] 定义函数
来源：http://mh.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ag.hahajie.cn

[R30] 函数返回状态码
来源：http://lb.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://qw.9csxet.cn

[R31] 局部变量
来源：http://qy.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://wc.shxzukj.cn

[R32] 参数个数校验
来源：http://ez.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ry.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://pq.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cg.521024.cn

[R34] 退出时清理
来源：http://dt.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iz.shxzskj.cn

[R35] 后台执行并等待
来源：http://uw.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ek.huanxung.cn

[R36] 并发执行多个任务
来源：http://qx.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dk.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://dr.szxytkj.cn

files=$(ls -1)
来源：http://af.haigaiapp.cn

[R38] 管道串联
来源：http://xl.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://gl.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://lo.chemitech.net.cn

cmd > out.log 2>&1
来源：http://nu.muxihuayi.cn

[R40] 追加写日志
来源：http://gb.nicolike.cn

echo "log" >> out.log
来源：http://ah.huanxung.cn

[R41] 丢弃输出
来源：http://lb.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://nc.muxihuayi.cn

[R42] 输入重定向
来源：http://os.newstarts.cn

wc -l < a.txt
来源：http://aa.hahajie.cn

[R43] 按名字查找文件
来源：http://ze.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://iz.chemitech.net.cn

[R44] 按修改时间查找
来源：http://hv.huixiangedu.cn

find . -mtime -7 -type f
来源：http://zz.yuntaijiaju.cn

[R45] 批量删除
来源：http://cu.9csxet.cn

find . -name "*.tmp" -delete
来源：http://zm.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://aa.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ns.yuexingan06.cn

[R47] sed 单行替换
来源：http://hl.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://po.shxzskj.cn

[R48] awk 取指定列
来源：http://vm.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://hg.shxzskj.cn

[R49] awk 带条件
来源：http://fw.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qp.gzmigu.cn

[R50] awk 求和
来源：http://ze.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ba.panjiajie.cn

[R51] 排序去重取前几
来源：http://tl.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dc.jianghongdianzi.cn

[R52] 统计行数
来源：http://ak.huanxung.cn

wc -l a.txt
来源：http://vh.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://di.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ni.yuexingan06.cn

[R54] 比较两个文件
来源：http://yi.bjjhwx.cn

diff a.txt b.txt
来源：http://bn.hahajie.cn

[R55] 压缩与解压
来源：http://er.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oj.hahajie.cn

[R56] 远程拷贝
来源：http://nr.panjiajie.cn

scp file user@host:/path/
来源：http://yq.yuexingan06.cn

[R57] 远程执行命令
来源：http://wu.jctech888.com.cn

ssh user@host 'uptime'
来源：http://us.wgjwhj.cn

[R58] 下载文件
来源：http://ud.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dm.lnxyls.cn

[R59] 发 POST JSON
来源：http://lo.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://np.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://xt.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pm.hahajie.cn

[R61] 磁盘占用
来源：http://oo.hnjuh.cn

df -h;  du -sh *
来源：http://kt.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://ju.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://li.9csxet.cn

[R63] 内存与进程
来源：http://ph.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://ws.muxihuayi.cn

[R64] 结束进程
来源：http://wc.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://zk.huixiangedu.cn

[R65] 查看端口占用
来源：http://hm.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mr.wgjwhj.cn

[R66] 定时任务
来源：http://js.huanxung.cn

crontab -e;  crontab -l
来源：http://jb.nicolike.cn

[R67] 生成随机十六进制串
来源：http://yb.chemitech.net.cn

openssl rand -hex 16
来源：http://gl.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://oj.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://em.panjiajie.cn

[R69] 生成随机密码
来源：http://jp.521024.cn

head -c 16 /dev/urandom | base64
来源：http://gz.colortex.cn

[R70] 时间戳与互转
来源：http://nf.newstarts.cn

date +%s;  date -d @1700000000
来源：http://nk.muxihuayi.cn

[R71] 日期格式化
来源：http://wg.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nz.gzmigu.cn

[R72] 等待端口就绪
来源：http://zw.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qo.newstarts.cn

[R73] 分割大日志
来源：http://el.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://ys.asd995.cn

[R74] 批量重命名
来源：http://hr.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xo.szsharing.cn

[R75] 导出环境变量
来源：http://dc.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://ls.bjjhwx.cn

[R76] 使用临时文件
来源：http://ld.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mk.wgjwhj.cn

[R77] 读取用户输入
来源：http://ur.panjiajie.cn

read -rp "请输入: " ans
来源：http://in.shxzskj.cn

[R78] 交互式菜单
来源：http://mq.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wz.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://ga.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jn.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://ka.huixiangedu.cn

time ./run.sh
来源：http://xr.newstarts.cn

================================================================================
来源：http://cv.haigaiapp.cn

S. C / C++ 专题
来源：http://tm.bjjhwx.cn

================================================================================
来源：http://np.muxihuayi.cn

[S01] C：Hello World
来源：http://ki.szxytkj.cn

#include <stdio.h>
来源：http://ph.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ve.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://th.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://lt.szsharing.cn

[S03] C：读入整数
来源：http://wp.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://mj.colortex.cn

[S04] C：字符串复制
来源：http://cw.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ao.wgjwhj.cn

[S05] C：字符串长度
来源：http://gh.huixinmuqiang.cn

strlen(s)
来源：http://sw.nicolike.cn

[S06] C：字符串比较
来源：http://qu.hahajie.cn

strcmp(a, b) == 0
来源：http://me.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://gg.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ws.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://dj.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dq.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://iu.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ab.yuexingan06.cn

[S10] C：指针与解引用
来源：http://vu.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://cq.hahajie.cn

[S11] C：逐行读文件
来源：http://ci.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://ml.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ow.newstarts.cn

fclose(f);
来源：http://ai.9csxet.cn

[S12] C：写文件
来源：http://va.jianghongdianzi.cn


<!-- 参考信息 -->