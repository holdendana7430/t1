代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xc.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zy.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ac.hnjuh.cn

[Q41] 多表连接
来源：http://yr.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xy.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://bf.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://jl.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://xt.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://me.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pw.chemitech.net.cn

[Q43] 标量子查询
来源：http://co.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gz.jctech888.com.cn

[Q44] IN 子查询
来源：http://iv.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lt.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://ke.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uv.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gt.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aq.colortex.cn

[Q47] 与平均值比较
来源：http://tb.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gp.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://nk.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ab.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://bv.jianghongdianzi.cn

[Q49] 更新单行
来源：http://xo.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://me.chemitech.net.cn

[Q50] 批量更新
来源：http://ks.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://an.szxytkj.cn

[Q51] 用子查询更新
来源：http://rg.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gr.asd995.cn

[Q52] 删除指定行
来源：http://tq.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://pp.shtwfgs.cn

[Q53] 按条件删除
来源：http://gq.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vn.panjiajie.cn

[Q54] 清空表
来源：http://co.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://zx.newstarts.cn

[Q55] 排名（并列占位）
来源：http://xu.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dy.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://je.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ib.huixinmuqiang.cn

[Q57] 行号
来源：http://wd.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pp.bookmarksfly.cn

[Q58] 累计求和
来源：http://mi.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wh.jctech888.com.cn

[Q59] 分组内累计
来源：http://mr.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wy.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://jn.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://di.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lv.szsharing.cn

[Q61] 移动平均
来源：http://la.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gf.lnxyls.cn

[Q62] 分组占比
来源：http://bh.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wj.szsharing.cn

[Q63] 开启事务
来源：http://vp.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sw.nszjky.cn

[Q64] 提交事务
来源：http://pk.huixinmuqiang.cn

COMMIT;
来源：http://iz.asd995.cn

[Q65] 回滚事务
来源：http://bl.panjiajie.cn

ROLLBACK;
来源：http://ok.lnxyls.cn

[Q66] 行锁查询
来源：http://fc.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mj.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://nd.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qk.colortex.cn

[Q68] 保存点
来源：http://sz.panjiajie.cn

SAVEPOINT sp1;
来源：http://xm.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://uo.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://sj.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://so.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://ih.muxihuayi.cn

ANALYZE TABLE users;
来源：http://nm.521024.cn

[Q71] 查看建表语句
来源：http://sp.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ua.huanxung.cn

[Q72] 查看索引
来源：http://tl.asd995.cn

SHOW INDEX FROM users;
来源：http://vt.panjiajie.cn

[Q73] 查看表状态
来源：http://lu.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ek.9csxet.cn

[Q74] 强制使用索引
来源：http://ii.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xw.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://gd.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fi.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zs.bjjhwx.cn

[Q76] 按天统计
来源：http://ue.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hw.nicolike.cn

[Q77] 时间加减
来源：http://hk.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sk.lnxyls.cn

[Q78] 当前时间
来源：http://fq.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dk.muxihuayi.cn

[Q79] 字符串拼接
来源：http://vf.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ex.panjiajie.cn

[Q80] 字符串截取
来源：http://es.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fi.shxzukj.cn

[Q81] 字符串替换
来源：http://vz.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lq.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://zy.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hi.shtwfgs.cn

[Q83] 大小写转换
来源：http://nu.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rm.huanxung.cn

[Q84] 去除首尾空格
来源：http://te.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://pd.nicolike.cn

[Q85] 数值取整
来源：http://ax.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jz.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://bw.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ru.9csxet.cn

[Q87] JSON 字段做条件
来源：http://lb.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xc.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://tw.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hh.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pc.hahajie.cn

[Q89] 判断表是否存在
来源：http://yg.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qr.muxihuayi.cn

[Q90] 生成序号列
来源：http://sk.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vr.nicolike.cn

================================================================================
来源：http://ch.yuntaijiaju.cn

R. Bash 专题
来源：http://ei.yuexingan06.cn

================================================================================
来源：http://vo.521024.cn

[R01] shebang 与严格模式
来源：http://xc.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://ls.bookmarksfly.cn

set -euo pipefail
来源：http://tr.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://pq.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://ll.huixiangedu.cn

[R03] 只读变量
来源：http://lm.wgjwhj.cn

readonly PI=3.14
来源：http://wh.shtwfgs.cn

[R04] 位置参数
来源：http://gp.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dm.jctech888.com.cn

[R05] 参数默认值
来源：http://lr.bjjhwx.cn

name="${1:-default}"
来源：http://el.huanxung.cn

[R06] 判断命令是否存在
来源：http://mo.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xs.muxihuayi.cn

[R07] if 判断文件
来源：http://oa.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gy.haigaiapp.cn

[R08] 数值比较
来源：http://li.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zj.521024.cn

[R09] 字符串比较
来源：http://su.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wl.bookmarksfly.cn

[R10] 正则匹配
来源：http://ug.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iw.nszjky.cn

[R11] case 多分支
来源：http://ng.nicolike.cn

case "$1" in
来源：http://dw.lnxyls.cn

start) echo "启动" ;;
来源：http://sq.panjiajie.cn

stop)  echo "停止" ;;
来源：http://er.colortex.cn

*)     echo "未知命令" ;;
来源：http://ak.jianghongdianzi.cn

esac
来源：http://tq.szxytkj.cn

[R12] for 遍历文件
来源：http://es.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://ls.nszjky.cn

[R13] for 计数循环
来源：http://xu.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://bx.nicolike.cn

[R14] C 风格 for
来源：http://jl.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oq.gzmigu.cn

[R15] while 逐行读文件
来源：http://mf.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wz.jctech888.com.cn

[R16] until 等待条件
来源：http://qk.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://by.hahajie.cn

[R17] 数组定义与取值
来源：http://fg.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yi.jctech888.com.cn

[R18] 遍历数组
来源：http://rb.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gv.colortex.cn

[R19] 数组长度
来源：http://lf.shxzukj.cn

echo "${#arr[@]}"
来源：http://zi.hnjuh.cn

[R20] 关联数组（字典）
来源：http://vt.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lj.szxytkj.cn

[R21] 字符串长度
来源：http://nt.jianghongdianzi.cn

echo "${#s}"
来源：http://rd.lnxyls.cn

[R22] 截取子串
来源：http://mv.shxzskj.cn

echo "${s:0:5}"
来源：http://kx.jianghongdianzi.cn

[R23] 字符串替换
来源：http://om.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wl.bookmarksfly.cn

[R24] 大小写转换
来源：http://rd.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dj.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://xa.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://an.shxzukj.cn

[R26] 命令替换
来源：http://bk.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://ol.panjiajie.cn

[R27] 算术展开
来源：http://gk.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://xv.hahajie.cn

[R28] 浮点运算
来源：http://le.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://wq.9csxet.cn

[R29] 定义函数
来源：http://gh.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lp.newstarts.cn

[R30] 函数返回状态码
来源：http://jd.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://gq.szxytkj.cn

[R31] 局部变量
来源：http://rg.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://gn.bookmarksfly.cn

[R32] 参数个数校验
来源：http://ww.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bs.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://bo.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qd.hnjuh.cn

[R34] 退出时清理
来源：http://wd.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ak.szsharing.cn

[R35] 后台执行并等待
来源：http://hs.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kz.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://hm.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://op.szsharing.cn

[R37] 把输出赋给变量
来源：http://dh.newstarts.cn

files=$(ls -1)
来源：http://fx.gzmigu.cn

[R38] 管道串联
来源：http://uh.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://wa.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://mr.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://mq.shxzskj.cn

[R40] 追加写日志
来源：http://ts.wgjwhj.cn

echo "log" >> out.log
来源：http://xj.wgjwhj.cn

[R41] 丢弃输出
来源：http://tj.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://jl.chemitech.net.cn

[R42] 输入重定向
来源：http://xe.yuexingan06.cn

wc -l < a.txt
来源：http://ww.wgjwhj.cn

[R43] 按名字查找文件
来源：http://is.gzmigu.cn

find . -name "*.log" -type f
来源：http://gj.szxytkj.cn

[R44] 按修改时间查找
来源：http://ge.szxytkj.cn

find . -mtime -7 -type f
来源：http://zg.jctech888.com.cn

[R45] 批量删除
来源：http://gu.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://lb.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://yk.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sw.muxihuayi.cn

[R47] sed 单行替换
来源：http://cl.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fg.521024.cn

[R48] awk 取指定列
来源：http://nx.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://zt.nicolike.cn

[R49] awk 带条件
来源：http://hz.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ny.shxzskj.cn

[R50] awk 求和
来源：http://xm.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fp.hahajie.cn

[R51] 排序去重取前几
来源：http://un.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dr.yuntaijiaju.cn

[R52] 统计行数
来源：http://rr.shxzskj.cn

wc -l a.txt
来源：http://tz.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://qf.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hd.hnjuh.cn

[R54] 比较两个文件
来源：http://md.nicolike.cn

diff a.txt b.txt
来源：http://ub.szxytkj.cn

[R55] 压缩与解压
来源：http://jz.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qa.panjiajie.cn

[R56] 远程拷贝
来源：http://wj.newstarts.cn

scp file user@host:/path/
来源：http://sd.haigaiapp.cn

[R57] 远程执行命令
来源：http://bi.muxihuayi.cn

ssh user@host 'uptime'
来源：http://mq.gzmigu.cn

[R58] 下载文件
来源：http://ad.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sq.panjiajie.cn

[R59] 发 POST JSON
来源：http://pl.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lt.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://pj.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://am.bookmarksfly.cn

[R61] 磁盘占用
来源：http://jy.shxzskj.cn

df -h;  du -sh *
来源：http://dd.szxytkj.cn

[R62] 找最占空间的文件
来源：http://vv.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://gy.asd995.cn

[R63] 内存与进程
来源：http://om.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://ah.panjiajie.cn

[R64] 结束进程
来源：http://va.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://ef.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://ds.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oi.huixinmuqiang.cn

[R66] 定时任务
来源：http://sa.chemitech.net.cn

crontab -e;  crontab -l
来源：http://dc.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://uc.hahajie.cn

openssl rand -hex 16
来源：http://ts.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://qw.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ia.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://wl.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://mi.shxzskj.cn

[R70] 时间戳与互转
来源：http://nu.asd995.cn

date +%s;  date -d @1700000000
来源：http://zj.asd995.cn

[R71] 日期格式化
来源：http://ns.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hx.shxzskj.cn

[R72] 等待端口就绪
来源：http://hp.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kf.huixiangedu.cn

[R73] 分割大日志
来源：http://vf.yuexingan06.cn

split -l 1000 big.log part_
来源：http://tv.huixinmuqiang.cn

[R74] 批量重命名
来源：http://hz.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nk.newstarts.cn

[R75] 导出环境变量
来源：http://so.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://rk.lnxyls.cn

[R76] 使用临时文件
来源：http://tv.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rw.panjiajie.cn

[R77] 读取用户输入
来源：http://bl.shtwfgs.cn

read -rp "请输入: " ans
来源：http://pc.jctech888.com.cn

[R78] 交互式菜单
来源：http://km.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tp.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://zm.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zj.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://hl.muxihuayi.cn

time ./run.sh
来源：http://hj.hahajie.cn

================================================================================
来源：http://uu.yuntaijiaju.cn

S. C / C++ 专题
来源：http://vm.muxihuayi.cn

================================================================================
来源：http://oh.yuntaijiaju.cn

[S01] C：Hello World
来源：http://qa.yuntaijiaju.cn

#include <stdio.h>
来源：http://vn.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mx.nszjky.cn

[S02] C：变量与格式化输出
来源：http://bq.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://fg.shxzukj.cn

[S03] C：读入整数
来源：http://wj.asd995.cn

int x; scanf("%d", &x);
来源：http://np.szsharing.cn

[S04] C：字符串复制
来源：http://px.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ky.haigaiapp.cn

[S05] C：字符串长度
来源：http://lg.huanxung.cn

strlen(s)
来源：http://is.bookmarksfly.cn

[S06] C：字符串比较
来源：http://qc.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://ly.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://wq.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gg.521024.cn

[S08] C：动态内存分配与释放
来源：http://or.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ns.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://dm.gzmigu.cn


<!-- 参考信息 -->