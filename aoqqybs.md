代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yn.chemitech.net.cn

[Q28] 求和与平均
来源：http://sr.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ha.szxytkj.cn

[Q29] 最大最小值
来源：http://vb.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://di.shtwfgs.cn

[Q30] 分组统计
来源：http://ag.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vw.huixiangedu.cn

[Q31] 分组后过滤
来源：http://gb.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ml.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://wn.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gh.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rj.wgjwhj.cn

[Q33] 多列分组
来源：http://ii.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ir.lnxyls.cn

[Q34] 每组取第一条
来源：http://gn.haigaiapp.cn

SELECT * FROM (
来源：http://kn.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ax.asd995.cn

) t WHERE rn = 1;
来源：http://ij.bjjhwx.cn

[Q35] 内连接
来源：http://tp.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uk.yuntaijiaju.cn

[Q36] 左连接
来源：http://jn.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vl.chemitech.net.cn

[Q37] 右连接
来源：http://ct.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rn.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kj.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://go.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://xf.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://up.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aq.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lk.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wu.shxzskj.cn

[Q41] 多表连接
来源：http://ee.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mx.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://ds.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://vg.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://hy.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://kf.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sp.nicolike.cn

[Q43] 标量子查询
来源：http://fl.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mk.huixiangedu.cn

[Q44] IN 子查询
来源：http://gx.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zm.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://jx.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zt.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rh.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jd.panjiajie.cn

[Q47] 与平均值比较
来源：http://lv.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oe.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://iz.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qs.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://km.gzmigu.cn

[Q49] 更新单行
来源：http://mj.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fc.521024.cn

[Q50] 批量更新
来源：http://sk.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wz.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://xg.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ds.shxzskj.cn

[Q52] 删除指定行
来源：http://is.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://zv.huanxung.cn

[Q53] 按条件删除
来源：http://zm.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zz.hahajie.cn

[Q54] 清空表
来源：http://zi.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://jx.9csxet.cn

[Q55] 排名（并列占位）
来源：http://zt.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tf.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://cd.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kj.asd995.cn

[Q57] 行号
来源：http://lx.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bz.huixiangedu.cn

[Q58] 累计求和
来源：http://mo.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ep.shtwfgs.cn

[Q59] 分组内累计
来源：http://up.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qc.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://bu.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ei.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zo.yuexingan06.cn

[Q61] 移动平均
来源：http://tq.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fw.wgjwhj.cn

[Q62] 分组占比
来源：http://tl.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hk.hahajie.cn

[Q63] 开启事务
来源：http://vw.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ph.colortex.cn

[Q64] 提交事务
来源：http://px.huixinmuqiang.cn

COMMIT;
来源：http://gr.panjiajie.cn

[Q65] 回滚事务
来源：http://pq.wgjwhj.cn

ROLLBACK;
来源：http://gl.lnxyls.cn

[Q66] 行锁查询
来源：http://rf.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://un.gzmigu.cn

[Q67] 设置隔离级别
来源：http://ww.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ir.chemitech.net.cn

[Q68] 保存点
来源：http://qq.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://kb.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://tv.chemitech.net.cn

[Q69] 查看执行计划
来源：http://tx.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ka.9csxet.cn

[Q70] 更新统计信息
来源：http://aw.jctech888.com.cn

ANALYZE TABLE users;
来源：http://jn.nicolike.cn

[Q71] 查看建表语句
来源：http://ds.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fr.shtwfgs.cn

[Q72] 查看索引
来源：http://yu.lnxyls.cn

SHOW INDEX FROM users;
来源：http://ya.shxzukj.cn

[Q73] 查看表状态
来源：http://kd.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bx.jctech888.com.cn

[Q74] 强制使用索引
来源：http://oc.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hw.bjjhwx.cn

[Q75] 日期格式化
来源：http://fw.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dy.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wq.shxzskj.cn

[Q76] 按天统计
来源：http://jq.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yv.szsharing.cn

[Q77] 时间加减
来源：http://uf.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tb.colortex.cn

[Q78] 当前时间
来源：http://gq.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jr.newstarts.cn

[Q79] 字符串拼接
来源：http://qi.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nj.bookmarksfly.cn

[Q80] 字符串截取
来源：http://uk.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nf.bjjhwx.cn

[Q81] 字符串替换
来源：http://kd.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ke.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://zw.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tx.lnxyls.cn

[Q83] 大小写转换
来源：http://ch.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lr.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://tr.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://xj.yuexingan06.cn

[Q85] 数值取整
来源：http://kz.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zp.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://lu.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iy.9csxet.cn

[Q87] JSON 字段做条件
来源：http://ic.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oo.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://xo.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cj.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://je.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://nh.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zz.huanxung.cn

[Q90] 生成序号列
来源：http://te.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vp.chemitech.net.cn

================================================================================
来源：http://tf.colortex.cn

R. Bash 专题
来源：http://nv.jctech888.com.cn

================================================================================
来源：http://ls.9csxet.cn

[R01] shebang 与严格模式
来源：http://uj.hahajie.cn

#!/usr/bin/env bash
来源：http://oc.lnxyls.cn

set -euo pipefail
来源：http://ky.hahajie.cn

[R02] 变量赋值与使用
来源：http://ei.shxzukj.cn

name="Tom"; echo "$name"
来源：http://pj.9csxet.cn

[R03] 只读变量
来源：http://yo.newstarts.cn

readonly PI=3.14
来源：http://xe.szsharing.cn

[R04] 位置参数
来源：http://pv.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qp.colortex.cn

[R05] 参数默认值
来源：http://rb.huixinmuqiang.cn

name="${1:-default}"
来源：http://xa.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://xd.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wb.asd995.cn

[R07] if 判断文件
来源：http://ky.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bz.szxytkj.cn

[R08] 数值比较
来源：http://pn.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wf.colortex.cn

[R09] 字符串比较
来源：http://aj.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uu.huanxung.cn

[R10] 正则匹配
来源：http://sn.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gq.newstarts.cn

[R11] case 多分支
来源：http://ya.muxihuayi.cn

case "$1" in
来源：http://hp.shxzskj.cn

start) echo "启动" ;;
来源：http://lt.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://fd.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://ca.nszjky.cn

esac
来源：http://oh.haigaiapp.cn

[R12] for 遍历文件
来源：http://fi.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://nh.asd995.cn

[R13] for 计数循环
来源：http://ry.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://fu.hahajie.cn

[R14] C 风格 for
来源：http://kk.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qg.gzmigu.cn

[R15] while 逐行读文件
来源：http://xe.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ea.hnjuh.cn

[R16] until 等待条件
来源：http://su.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wy.9csxet.cn

[R17] 数组定义与取值
来源：http://sg.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nl.colortex.cn

[R18] 遍历数组
来源：http://ve.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bm.yuexingan06.cn

[R19] 数组长度
来源：http://yv.huixiangedu.cn

echo "${#arr[@]}"
来源：http://up.szsharing.cn

[R20] 关联数组（字典）
来源：http://ma.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rt.huixiangedu.cn

[R21] 字符串长度
来源：http://oa.panjiajie.cn

echo "${#s}"
来源：http://kz.newstarts.cn

[R22] 截取子串
来源：http://tp.hnjuh.cn

echo "${s:0:5}"
来源：http://ga.hahajie.cn

[R23] 字符串替换
来源：http://ip.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://or.colortex.cn

[R24] 大小写转换
来源：http://fs.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bu.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://rn.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fe.jianghongdianzi.cn

[R26] 命令替换
来源：http://cs.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://iu.haigaiapp.cn

[R27] 算术展开
来源：http://zu.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://am.shxzskj.cn

[R28] 浮点运算
来源：http://gk.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://it.lnxyls.cn

[R29] 定义函数
来源：http://vd.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oa.nicolike.cn

[R30] 函数返回状态码
来源：http://ji.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://vs.colortex.cn

[R31] 局部变量
来源：http://hm.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://kk.szsharing.cn

[R32] 参数个数校验
来源：http://ri.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://th.asd995.cn

[R33] 捕获错误并提示行号
来源：http://pc.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oh.asd995.cn

[R34] 退出时清理
来源：http://pn.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uw.newstarts.cn

[R35] 后台执行并等待
来源：http://ut.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://md.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://to.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nt.nicolike.cn

[R37] 把输出赋给变量
来源：http://qx.szxytkj.cn

files=$(ls -1)
来源：http://al.szxytkj.cn

[R38] 管道串联
来源：http://oh.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://yk.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://rf.521024.cn

cmd > out.log 2>&1
来源：http://hy.hnjuh.cn

[R40] 追加写日志
来源：http://se.hnjuh.cn

echo "log" >> out.log
来源：http://yq.lnxyls.cn

[R41] 丢弃输出
来源：http://am.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://px.lnxyls.cn

[R42] 输入重定向
来源：http://zd.szxytkj.cn

wc -l < a.txt
来源：http://lq.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://so.asd995.cn

find . -name "*.log" -type f
来源：http://gh.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://nm.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://li.panjiajie.cn

[R45] 批量删除
来源：http://wy.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://la.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://ub.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xs.huixiangedu.cn

[R47] sed 单行替换
来源：http://lv.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mu.szxytkj.cn

[R48] awk 取指定列
来源：http://zf.521024.cn

awk '{print $1, $3}' a.txt
来源：http://ii.jianghongdianzi.cn

[R49] awk 带条件
来源：http://mf.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zt.panjiajie.cn

[R50] awk 求和
来源：http://di.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vf.newstarts.cn

[R51] 排序去重取前几
来源：http://ba.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ne.newstarts.cn

[R52] 统计行数
来源：http://tk.9csxet.cn

wc -l a.txt
来源：http://fz.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://dl.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://za.shxzskj.cn

[R54] 比较两个文件
来源：http://vz.szsharing.cn

diff a.txt b.txt
来源：http://io.huanxung.cn

[R55] 压缩与解压
来源：http://cp.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qk.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://zn.shtwfgs.cn

scp file user@host:/path/
来源：http://di.panjiajie.cn

[R57] 远程执行命令
来源：http://uh.shxzukj.cn

ssh user@host 'uptime'
来源：http://ei.wgjwhj.cn

[R58] 下载文件
来源：http://zp.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mx.yuexingan06.cn

[R59] 发 POST JSON
来源：http://ix.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cb.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://aa.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yp.shxzukj.cn

[R61] 磁盘占用
来源：http://rw.hnjuh.cn

df -h;  du -sh *
来源：http://hd.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://cf.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://uo.shxzskj.cn

[R63] 内存与进程
来源：http://bi.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://ef.521024.cn

[R64] 结束进程
来源：http://lz.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://wy.bjjhwx.cn

[R65] 查看端口占用
来源：http://ud.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ln.chemitech.net.cn

[R66] 定时任务
来源：http://cw.lnxyls.cn

crontab -e;  crontab -l
来源：http://ib.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://wm.huixinmuqiang.cn

openssl rand -hex 16
来源：http://lj.wgjwhj.cn

[R68] 计算文件校验值
来源：http://aw.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ot.shtwfgs.cn

[R69] 生成随机密码
来源：http://gc.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://zn.nszjky.cn

[R70] 时间戳与互转
来源：http://ie.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://fn.nicolike.cn

[R71] 日期格式化
来源：http://ol.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bu.shxzskj.cn

[R72] 等待端口就绪
来源：http://bf.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tw.bjjhwx.cn

[R73] 分割大日志
来源：http://oa.9csxet.cn

split -l 1000 big.log part_
来源：http://il.wgjwhj.cn

[R74] 批量重命名
来源：http://uz.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://et.9csxet.cn

[R75] 导出环境变量
来源：http://bk.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://bf.lnxyls.cn

[R76] 使用临时文件
来源：http://qx.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bt.9csxet.cn

[R77] 读取用户输入
来源：http://yq.newstarts.cn


<!-- 参考信息 -->