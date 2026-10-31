代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jm.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://zq.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vp.shtwfgs.cn

[Q29] 最大最小值
来源：http://pi.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vh.hahajie.cn

[Q30] 分组统计
来源：http://nm.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yl.nszjky.cn

[Q31] 分组后过滤
来源：http://cx.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xf.szsharing.cn

[Q32] 分组拼接字符串
来源：http://oa.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ph.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ef.bookmarksfly.cn

[Q33] 多列分组
来源：http://gc.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zt.muxihuayi.cn

[Q34] 每组取第一条
来源：http://dq.shxzukj.cn

SELECT * FROM (
来源：http://kt.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ph.nszjky.cn

) t WHERE rn = 1;
来源：http://dy.panjiajie.cn

[Q35] 内连接
来源：http://av.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://az.nicolike.cn

[Q36] 左连接
来源：http://js.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cw.szsharing.cn

[Q37] 右连接
来源：http://ub.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sy.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wj.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://sj.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yp.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fy.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://im.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qw.gzmigu.cn

[Q41] 多表连接
来源：http://kw.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lx.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://ku.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://uo.521024.cn

[Q42] 连接条件附加过滤
来源：http://gn.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://qx.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rh.chemitech.net.cn

[Q43] 标量子查询
来源：http://iq.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yf.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://lv.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://da.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://tf.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gy.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vd.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ks.shxzskj.cn

[Q47] 与平均值比较
来源：http://us.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://si.colortex.cn

[Q48] CTE 公用表表达式
来源：http://th.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xl.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://sr.chemitech.net.cn

[Q49] 更新单行
来源：http://pl.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xe.nszjky.cn

[Q50] 批量更新
来源：http://fu.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rz.newstarts.cn

[Q51] 用子查询更新
来源：http://wx.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jl.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://du.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://zs.newstarts.cn

[Q53] 按条件删除
来源：http://am.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://om.panjiajie.cn

[Q54] 清空表
来源：http://ut.hahajie.cn

TRUNCATE TABLE logs;
来源：http://ja.nicolike.cn

[Q55] 排名（并列占位）
来源：http://uk.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ie.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://ti.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vj.bjjhwx.cn

[Q57] 行号
来源：http://xk.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ht.panjiajie.cn

[Q58] 累计求和
来源：http://xj.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://my.szxytkj.cn

[Q59] 分组内累计
来源：http://bo.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aa.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://fe.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gv.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://at.shtwfgs.cn

[Q61] 移动平均
来源：http://ll.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://es.shtwfgs.cn

[Q62] 分组占比
来源：http://rk.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xk.wgjwhj.cn

[Q63] 开启事务
来源：http://xe.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xl.panjiajie.cn

[Q64] 提交事务
来源：http://fc.bookmarksfly.cn

COMMIT;
来源：http://co.hnjuh.cn

[Q65] 回滚事务
来源：http://pg.muxihuayi.cn

ROLLBACK;
来源：http://tt.shxzukj.cn

[Q66] 行锁查询
来源：http://zj.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xo.szxytkj.cn

[Q67] 设置隔离级别
来源：http://ki.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wg.yuntaijiaju.cn

[Q68] 保存点
来源：http://va.colortex.cn

SAVEPOINT sp1;
来源：http://fv.szsharing.cn

ROLLBACK TO sp1;
来源：http://be.jctech888.com.cn

[Q69] 查看执行计划
来源：http://tt.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hl.hahajie.cn

[Q70] 更新统计信息
来源：http://nm.521024.cn

ANALYZE TABLE users;
来源：http://ap.nszjky.cn

[Q71] 查看建表语句
来源：http://ar.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nl.nicolike.cn

[Q72] 查看索引
来源：http://pz.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://ru.lnxyls.cn

[Q73] 查看表状态
来源：http://ik.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ph.shxzukj.cn

[Q74] 强制使用索引
来源：http://yr.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hp.chemitech.net.cn

[Q75] 日期格式化
来源：http://dk.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zq.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kh.chemitech.net.cn

[Q76] 按天统计
来源：http://lj.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ys.lnxyls.cn

[Q77] 时间加减
来源：http://qr.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oe.wgjwhj.cn

[Q78] 当前时间
来源：http://jg.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zo.haigaiapp.cn

[Q79] 字符串拼接
来源：http://gv.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kh.asd995.cn

[Q80] 字符串截取
来源：http://uc.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hf.hnjuh.cn

[Q81] 字符串替换
来源：http://vr.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ob.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://lf.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://ss.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lx.9csxet.cn

[Q84] 去除首尾空格
来源：http://ob.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://sj.szxytkj.cn

[Q85] 数值取整
来源：http://cv.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pf.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://sp.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dn.9csxet.cn

[Q87] JSON 字段做条件
来源：http://ah.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pz.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://qt.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vd.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dj.9csxet.cn

[Q89] 判断表是否存在
来源：http://ts.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gm.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://nv.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://st.huanxung.cn

================================================================================
来源：http://ha.yuntaijiaju.cn

R. Bash 专题
来源：http://do.szxytkj.cn

================================================================================
来源：http://qw.newstarts.cn

[R01] shebang 与严格模式
来源：http://eo.hnjuh.cn

#!/usr/bin/env bash
来源：http://mn.huixiangedu.cn

set -euo pipefail
来源：http://lt.szsharing.cn

[R02] 变量赋值与使用
来源：http://sq.nszjky.cn

name="Tom"; echo "$name"
来源：http://by.yuntaijiaju.cn

[R03] 只读变量
来源：http://fz.bookmarksfly.cn

readonly PI=3.14
来源：http://oo.huanxung.cn

[R04] 位置参数
来源：http://pa.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ao.huixiangedu.cn

[R05] 参数默认值
来源：http://al.shxzukj.cn

name="${1:-default}"
来源：http://rd.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://no.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uj.asd995.cn

[R07] if 判断文件
来源：http://bb.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ij.haigaiapp.cn

[R08] 数值比较
来源：http://yj.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ad.9csxet.cn

[R09] 字符串比较
来源：http://yn.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://az.hnjuh.cn

[R10] 正则匹配
来源：http://hr.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ll.huanxung.cn

[R11] case 多分支
来源：http://xj.9csxet.cn

case "$1" in
来源：http://fz.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://zs.asd995.cn

stop)  echo "停止" ;;
来源：http://co.newstarts.cn

*)     echo "未知命令" ;;
来源：http://ig.panjiajie.cn

esac
来源：http://mj.szxytkj.cn

[R12] for 遍历文件
来源：http://xu.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://to.521024.cn

[R13] for 计数循环
来源：http://yt.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://yv.panjiajie.cn

[R14] C 风格 for
来源：http://kp.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ad.shtwfgs.cn

[R15] while 逐行读文件
来源：http://in.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yc.hahajie.cn

[R16] until 等待条件
来源：http://sf.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://km.haigaiapp.cn

[R17] 数组定义与取值
来源：http://am.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hh.huanxung.cn

[R18] 遍历数组
来源：http://tq.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fz.hahajie.cn

[R19] 数组长度
来源：http://kn.haigaiapp.cn

echo "${#arr[@]}"
来源：http://er.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://nf.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dh.huixinmuqiang.cn

[R21] 字符串长度
来源：http://yn.hahajie.cn

echo "${#s}"
来源：http://or.nszjky.cn

[R22] 截取子串
来源：http://wa.haigaiapp.cn

echo "${s:0:5}"
来源：http://so.hnjuh.cn

[R23] 字符串替换
来源：http://mo.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://af.panjiajie.cn

[R24] 大小写转换
来源：http://qc.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ku.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://tl.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dp.shxzskj.cn

[R26] 命令替换
来源：http://im.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://kf.jctech888.com.cn

[R27] 算术展开
来源：http://ro.newstarts.cn

echo $((1 + 2 * 3))
来源：http://ha.yuntaijiaju.cn

[R28] 浮点运算
来源：http://xe.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://zh.9csxet.cn

[R29] 定义函数
来源：http://es.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ld.jctech888.com.cn

[R30] 函数返回状态码
来源：http://le.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://lw.asd995.cn

[R31] 局部变量
来源：http://td.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://ge.newstarts.cn

[R32] 参数个数校验
来源：http://ei.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iw.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://ih.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dh.hahajie.cn

[R34] 退出时清理
来源：http://yf.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://st.yuexingan06.cn

[R35] 后台执行并等待
来源：http://xv.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ph.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://vn.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vv.panjiajie.cn

[R37] 把输出赋给变量
来源：http://sn.huixinmuqiang.cn

files=$(ls -1)
来源：http://mi.colortex.cn

[R38] 管道串联
来源：http://ij.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://ll.colortex.cn

[R39] 重定向标准输出与错误
来源：http://ys.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://xa.shtwfgs.cn

[R40] 追加写日志
来源：http://qr.shxzskj.cn

echo "log" >> out.log
来源：http://vo.szsharing.cn

[R41] 丢弃输出
来源：http://pv.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://zm.shtwfgs.cn

[R42] 输入重定向
来源：http://bd.shtwfgs.cn

wc -l < a.txt
来源：http://xl.yuexingan06.cn

[R43] 按名字查找文件
来源：http://cd.panjiajie.cn

find . -name "*.log" -type f
来源：http://lq.hnjuh.cn

[R44] 按修改时间查找
来源：http://pp.shxzukj.cn

find . -mtime -7 -type f
来源：http://ma.jianghongdianzi.cn

[R45] 批量删除
来源：http://al.nicolike.cn

find . -name "*.tmp" -delete
来源：http://me.nszjky.cn

[R46] 递归替换文件内容
来源：http://fl.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oc.asd995.cn

[R47] sed 单行替换
来源：http://he.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rm.shtwfgs.cn

[R48] awk 取指定列
来源：http://wc.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://tw.newstarts.cn

[R49] awk 带条件
来源：http://kk.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ig.muxihuayi.cn

[R50] awk 求和
来源：http://no.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://td.yuexingan06.cn

[R51] 排序去重取前几
来源：http://om.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aw.hnjuh.cn

[R52] 统计行数
来源：http://ar.shxzukj.cn

wc -l a.txt
来源：http://fi.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://tt.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qy.nszjky.cn

[R54] 比较两个文件
来源：http://td.szxytkj.cn

diff a.txt b.txt
来源：http://xw.shtwfgs.cn

[R55] 压缩与解压
来源：http://bw.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ej.shtwfgs.cn

[R56] 远程拷贝
来源：http://jr.lnxyls.cn

scp file user@host:/path/
来源：http://kz.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://ek.yuexingan06.cn

ssh user@host 'uptime'
来源：http://nv.jctech888.com.cn

[R58] 下载文件
来源：http://aw.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cq.newstarts.cn

[R59] 发 POST JSON
来源：http://kj.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tu.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://ny.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lx.yuexingan06.cn

[R61] 磁盘占用
来源：http://qw.asd995.cn

df -h;  du -sh *
来源：http://jj.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://ru.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://oe.521024.cn

[R63] 内存与进程
来源：http://cp.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://pf.huixinmuqiang.cn

[R64] 结束进程
来源：http://jd.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://sv.chemitech.net.cn

[R65] 查看端口占用
来源：http://ei.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wd.panjiajie.cn

[R66] 定时任务
来源：http://ln.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://dl.521024.cn

[R67] 生成随机十六进制串
来源：http://op.chemitech.net.cn

openssl rand -hex 16
来源：http://yb.shxzukj.cn

[R68] 计算文件校验值
来源：http://xk.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://di.muxihuayi.cn

[R69] 生成随机密码
来源：http://xw.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://cx.521024.cn

[R70] 时间戳与互转
来源：http://hj.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://sp.bookmarksfly.cn

[R71] 日期格式化
来源：http://ut.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qp.yuexingan06.cn

[R72] 等待端口就绪
来源：http://vk.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zc.haigaiapp.cn

[R73] 分割大日志
来源：http://zo.lnxyls.cn

split -l 1000 big.log part_
来源：http://ay.huanxung.cn

[R74] 批量重命名
来源：http://bz.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hj.wgjwhj.cn

[R75] 导出环境变量
来源：http://jw.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://um.szxytkj.cn

[R76] 使用临时文件
来源：http://tm.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ne.szsharing.cn

[R77] 读取用户输入
来源：http://cw.haigaiapp.cn


<!-- 参考信息 -->