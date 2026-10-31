代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cx.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://nh.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://es.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cx.shxzukj.cn

[Q33] 多列分组
来源：http://rt.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dn.szsharing.cn

[Q34] 每组取第一条
来源：http://aw.shxzukj.cn

SELECT * FROM (
来源：http://gl.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ic.9csxet.cn

) t WHERE rn = 1;
来源：http://cw.haigaiapp.cn

[Q35] 内连接
来源：http://iu.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ui.asd995.cn

[Q36] 左连接
来源：http://kn.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jr.521024.cn

[Q37] 右连接
来源：http://yj.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mv.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ch.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xh.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://ix.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zg.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ff.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mu.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xy.nszjky.cn

[Q41] 多表连接
来源：http://gq.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mr.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://sx.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://yk.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://ms.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://fz.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eb.shtwfgs.cn

[Q43] 标量子查询
来源：http://wb.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zm.521024.cn

[Q44] IN 子查询
来源：http://gg.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zy.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://ro.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vd.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gu.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://to.shxzskj.cn

[Q47] 与平均值比较
来源：http://hz.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qw.asd995.cn

[Q48] CTE 公用表表达式
来源：http://vs.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qr.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://zj.shxzukj.cn

[Q49] 更新单行
来源：http://vd.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cx.haigaiapp.cn

[Q50] 批量更新
来源：http://nk.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pt.haigaiapp.cn

[Q51] 用子查询更新
来源：http://qp.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wy.colortex.cn

[Q52] 删除指定行
来源：http://eg.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://nd.szsharing.cn

[Q53] 按条件删除
来源：http://ms.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://it.wgjwhj.cn

[Q54] 清空表
来源：http://pq.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://jr.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://ti.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pl.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://bo.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://va.nicolike.cn

[Q57] 行号
来源：http://ep.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zp.haigaiapp.cn

[Q58] 累计求和
来源：http://yx.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://an.nszjky.cn

[Q59] 分组内累计
来源：http://lh.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wc.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://ue.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oi.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wl.panjiajie.cn

[Q61] 移动平均
来源：http://gu.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ns.shxzukj.cn

[Q62] 分组占比
来源：http://xz.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wc.huixinmuqiang.cn

[Q63] 开启事务
来源：http://eu.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xr.yuexingan06.cn

[Q64] 提交事务
来源：http://uo.hahajie.cn

COMMIT;
来源：http://nl.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://nz.nicolike.cn

ROLLBACK;
来源：http://um.shxzskj.cn

[Q66] 行锁查询
来源：http://wi.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wi.huanxung.cn

[Q67] 设置隔离级别
来源：http://vl.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zs.szsharing.cn

[Q68] 保存点
来源：http://xa.shtwfgs.cn

SAVEPOINT sp1;
来源：http://ig.nicolike.cn

ROLLBACK TO sp1;
来源：http://eo.jctech888.com.cn

[Q69] 查看执行计划
来源：http://fh.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zm.colortex.cn

[Q70] 更新统计信息
来源：http://ao.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://id.muxihuayi.cn

[Q71] 查看建表语句
来源：http://tv.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vx.huanxung.cn

[Q72] 查看索引
来源：http://pe.nszjky.cn

SHOW INDEX FROM users;
来源：http://ev.asd995.cn

[Q73] 查看表状态
来源：http://gx.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://up.newstarts.cn

[Q74] 强制使用索引
来源：http://rf.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vu.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://wv.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fv.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://by.szsharing.cn

[Q76] 按天统计
来源：http://ra.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://be.521024.cn

[Q77] 时间加减
来源：http://nb.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fe.9csxet.cn

[Q78] 当前时间
来源：http://xo.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fm.haigaiapp.cn

[Q79] 字符串拼接
来源：http://bt.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wj.hahajie.cn

[Q80] 字符串截取
来源：http://ff.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zt.panjiajie.cn

[Q81] 字符串替换
来源：http://ki.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nz.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://jf.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yt.521024.cn

[Q83] 大小写转换
来源：http://hr.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jc.szxytkj.cn

[Q84] 去除首尾空格
来源：http://oq.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://rc.szsharing.cn

[Q85] 数值取整
来源：http://vj.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ia.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://fm.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pw.huanxung.cn

[Q87] JSON 字段做条件
来源：http://fv.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pf.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://ru.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ja.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hv.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://lp.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nf.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://yl.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://us.hnjuh.cn

================================================================================
来源：http://xn.wgjwhj.cn

R. Bash 专题
来源：http://jv.huanxung.cn

================================================================================
来源：http://ba.nicolike.cn

[R01] shebang 与严格模式
来源：http://bg.shtwfgs.cn

#!/usr/bin/env bash
来源：http://lx.colortex.cn

set -euo pipefail
来源：http://li.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://ch.huanxung.cn

name="Tom"; echo "$name"
来源：http://oq.9csxet.cn

[R03] 只读变量
来源：http://sa.muxihuayi.cn

readonly PI=3.14
来源：http://yj.bookmarksfly.cn

[R04] 位置参数
来源：http://wt.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jk.huixinmuqiang.cn

[R05] 参数默认值
来源：http://wy.hnjuh.cn

name="${1:-default}"
来源：http://qj.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://hu.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ez.asd995.cn

[R07] if 判断文件
来源：http://qp.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gl.nicolike.cn

[R08] 数值比较
来源：http://uc.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://if.huanxung.cn

[R09] 字符串比较
来源：http://fy.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nh.huixiangedu.cn

[R10] 正则匹配
来源：http://cv.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://us.haigaiapp.cn

[R11] case 多分支
来源：http://uf.jianghongdianzi.cn

case "$1" in
来源：http://if.szxytkj.cn

start) echo "启动" ;;
来源：http://gj.hnjuh.cn

stop)  echo "停止" ;;
来源：http://dz.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://tw.9csxet.cn

esac
来源：http://ck.shxzskj.cn

[R12] for 遍历文件
来源：http://au.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://xp.panjiajie.cn

[R13] for 计数循环
来源：http://tx.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://uf.shxzskj.cn

[R14] C 风格 for
来源：http://fq.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eb.wgjwhj.cn

[R15] while 逐行读文件
来源：http://mi.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://et.bjjhwx.cn

[R16] until 等待条件
来源：http://ef.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sc.chemitech.net.cn

[R17] 数组定义与取值
来源：http://sk.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mh.szsharing.cn

[R18] 遍历数组
来源：http://wn.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vo.chemitech.net.cn

[R19] 数组长度
来源：http://ee.521024.cn

echo "${#arr[@]}"
来源：http://bc.hnjuh.cn

[R20] 关联数组（字典）
来源：http://xf.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ic.9csxet.cn

[R21] 字符串长度
来源：http://ox.gzmigu.cn

echo "${#s}"
来源：http://xj.nszjky.cn

[R22] 截取子串
来源：http://yn.521024.cn

echo "${s:0:5}"
来源：http://en.hahajie.cn

[R23] 字符串替换
来源：http://bi.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fp.yuntaijiaju.cn

[R24] 大小写转换
来源：http://hx.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ln.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://bj.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://im.521024.cn

[R26] 命令替换
来源：http://lg.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://el.hahajie.cn

[R27] 算术展开
来源：http://oq.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://jc.muxihuayi.cn

[R28] 浮点运算
来源：http://vu.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://xg.jctech888.com.cn

[R29] 定义函数
来源：http://lj.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ts.wgjwhj.cn

[R30] 函数返回状态码
来源：http://pq.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://rw.chemitech.net.cn

[R31] 局部变量
来源：http://ta.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://th.nszjky.cn

[R32] 参数个数校验
来源：http://sg.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://me.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://nr.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nw.huixinmuqiang.cn

[R34] 退出时清理
来源：http://md.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xx.szsharing.cn

[R35] 后台执行并等待
来源：http://ng.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://aw.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://hl.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ec.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://fg.521024.cn

files=$(ls -1)
来源：http://mr.panjiajie.cn

[R38] 管道串联
来源：http://cm.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://na.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://oc.nicolike.cn

cmd > out.log 2>&1
来源：http://ok.shtwfgs.cn

[R40] 追加写日志
来源：http://tk.lnxyls.cn

echo "log" >> out.log
来源：http://sy.bjjhwx.cn

[R41] 丢弃输出
来源：http://mg.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://ty.yuexingan06.cn

[R42] 输入重定向
来源：http://tn.521024.cn

wc -l < a.txt
来源：http://ze.szxytkj.cn

[R43] 按名字查找文件
来源：http://we.yuexingan06.cn

find . -name "*.log" -type f
来源：http://xo.huixiangedu.cn

[R44] 按修改时间查找
来源：http://nn.panjiajie.cn

find . -mtime -7 -type f
来源：http://na.bookmarksfly.cn

[R45] 批量删除
来源：http://db.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://ko.nszjky.cn

[R46] 递归替换文件内容
来源：http://mz.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pp.panjiajie.cn

[R47] sed 单行替换
来源：http://jq.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://la.newstarts.cn

[R48] awk 取指定列
来源：http://zk.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://wf.hnjuh.cn

[R49] awk 带条件
来源：http://gx.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://il.jctech888.com.cn

[R50] awk 求和
来源：http://bw.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yl.shxzskj.cn

[R51] 排序去重取前几
来源：http://yl.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wo.hahajie.cn

[R52] 统计行数
来源：http://ad.newstarts.cn

wc -l a.txt
来源：http://so.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://oh.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ib.hnjuh.cn

[R54] 比较两个文件
来源：http://em.muxihuayi.cn

diff a.txt b.txt
来源：http://lz.muxihuayi.cn

[R55] 压缩与解压
来源：http://ea.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://la.lnxyls.cn

[R56] 远程拷贝
来源：http://xi.hnjuh.cn

scp file user@host:/path/
来源：http://cm.9csxet.cn

[R57] 远程执行命令
来源：http://al.gzmigu.cn

ssh user@host 'uptime'
来源：http://ht.hahajie.cn

[R58] 下载文件
来源：http://hw.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ox.panjiajie.cn

[R59] 发 POST JSON
来源：http://if.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sa.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://uk.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xd.panjiajie.cn

[R61] 磁盘占用
来源：http://os.shxzskj.cn

df -h;  du -sh *
来源：http://pg.asd995.cn

[R62] 找最占空间的文件
来源：http://nu.colortex.cn

du -ah . | sort -rh | head -10
来源：http://jn.panjiajie.cn

[R63] 内存与进程
来源：http://wh.521024.cn

free -h;  ps aux | grep nginx
来源：http://ok.hnjuh.cn

[R64] 结束进程
来源：http://kj.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://hz.chemitech.net.cn

[R65] 查看端口占用
来源：http://wk.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://of.hahajie.cn

[R66] 定时任务
来源：http://vn.shtwfgs.cn

crontab -e;  crontab -l
来源：http://xu.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://td.shtwfgs.cn

openssl rand -hex 16
来源：http://ww.jctech888.com.cn

[R68] 计算文件校验值
来源：http://jp.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://or.jctech888.com.cn

[R69] 生成随机密码
来源：http://hj.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://uu.szsharing.cn

[R70] 时间戳与互转
来源：http://ci.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://kq.nszjky.cn

[R71] 日期格式化
来源：http://bp.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ps.szsharing.cn

[R72] 等待端口就绪
来源：http://dt.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jd.bookmarksfly.cn

[R73] 分割大日志
来源：http://nn.nicolike.cn

split -l 1000 big.log part_
来源：http://uc.colortex.cn

[R74] 批量重命名
来源：http://my.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nt.521024.cn

[R75] 导出环境变量
来源：http://qh.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://xq.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://rh.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ue.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://wh.hahajie.cn

read -rp "请输入: " ans
来源：http://ti.szsharing.cn

[R78] 交互式菜单
来源：http://cr.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qj.yuexingan06.cn

[R79] 解析命令行选项
来源：http://fs.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ge.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://nz.wgjwhj.cn

time ./run.sh
来源：http://eu.asd995.cn

================================================================================
来源：http://kl.jctech888.com.cn


<!-- 参考信息 -->