代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qf.lnxyls.cn

[Q24] 去重
来源：http://ol.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://cz.nszjky.cn

[Q25] 只取前 N 条
来源：http://zq.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kd.szxytkj.cn

[Q26] 计数
来源：http://sg.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://aq.521024.cn

[Q27] 条件计数
来源：http://ww.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qm.hahajie.cn

[Q28] 求和与平均
来源：http://ax.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://om.nicolike.cn

[Q29] 最大最小值
来源：http://em.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zk.shxzukj.cn

[Q30] 分组统计
来源：http://ai.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oz.chemitech.net.cn

[Q31] 分组后过滤
来源：http://yi.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aj.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://xr.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lo.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lg.szxytkj.cn

[Q33] 多列分组
来源：http://fd.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bm.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://tl.bjjhwx.cn

SELECT * FROM (
来源：http://sq.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ix.shxzskj.cn

) t WHERE rn = 1;
来源：http://ev.9csxet.cn

[Q35] 内连接
来源：http://ki.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bq.gzmigu.cn

[Q36] 左连接
来源：http://wn.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://at.nicolike.cn

[Q37] 右连接
来源：http://kp.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ei.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sa.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pp.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://qc.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dv.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cf.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://le.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tw.lnxyls.cn

[Q41] 多表连接
来源：http://ij.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qi.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://yv.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ij.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://ce.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://xn.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gw.shxzskj.cn

[Q43] 标量子查询
来源：http://uc.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vh.9csxet.cn

[Q44] IN 子查询
来源：http://by.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qe.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://gn.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uc.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tj.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ri.huanxung.cn

[Q47] 与平均值比较
来源：http://qj.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jk.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://zc.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mz.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://pb.huixiangedu.cn

[Q49] 更新单行
来源：http://ra.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ye.nszjky.cn

[Q50] 批量更新
来源：http://yz.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yo.wgjwhj.cn

[Q51] 用子查询更新
来源：http://tq.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rw.szsharing.cn

[Q52] 删除指定行
来源：http://xc.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://av.gzmigu.cn

[Q53] 按条件删除
来源：http://cx.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oy.bookmarksfly.cn

[Q54] 清空表
来源：http://bj.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://iw.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://zd.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vz.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://nb.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zn.newstarts.cn

[Q57] 行号
来源：http://tb.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oc.9csxet.cn

[Q58] 累计求和
来源：http://kl.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ge.yuexingan06.cn

[Q59] 分组内累计
来源：http://lo.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wv.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://qr.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fw.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zs.nicolike.cn

[Q61] 移动平均
来源：http://oq.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dj.521024.cn

[Q62] 分组占比
来源：http://gv.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://os.yuntaijiaju.cn

[Q63] 开启事务
来源：http://tn.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lj.nszjky.cn

[Q64] 提交事务
来源：http://oy.nicolike.cn

COMMIT;
来源：http://ti.asd995.cn

[Q65] 回滚事务
来源：http://he.nszjky.cn

ROLLBACK;
来源：http://ta.yuexingan06.cn

[Q66] 行锁查询
来源：http://gz.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://so.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://aj.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hs.colortex.cn

[Q68] 保存点
来源：http://kq.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://xx.shxzukj.cn

ROLLBACK TO sp1;
来源：http://rd.lnxyls.cn

[Q69] 查看执行计划
来源：http://ep.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ld.bjjhwx.cn

[Q70] 更新统计信息
来源：http://qv.muxihuayi.cn

ANALYZE TABLE users;
来源：http://za.haigaiapp.cn

[Q71] 查看建表语句
来源：http://yz.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sx.panjiajie.cn

[Q72] 查看索引
来源：http://lk.nszjky.cn

SHOW INDEX FROM users;
来源：http://px.shtwfgs.cn

[Q73] 查看表状态
来源：http://cs.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ck.shtwfgs.cn

[Q74] 强制使用索引
来源：http://xt.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qa.bjjhwx.cn

[Q75] 日期格式化
来源：http://dh.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mk.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gy.chemitech.net.cn

[Q76] 按天统计
来源：http://mf.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mg.szxytkj.cn

[Q77] 时间加减
来源：http://pc.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ts.muxihuayi.cn

[Q78] 当前时间
来源：http://sj.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rv.szxytkj.cn

[Q79] 字符串拼接
来源：http://lu.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qo.9csxet.cn

[Q80] 字符串截取
来源：http://oh.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rj.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://tg.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dy.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://vx.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xk.shxzskj.cn

[Q83] 大小写转换
来源：http://yc.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sp.szxytkj.cn

[Q84] 去除首尾空格
来源：http://xw.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://io.bookmarksfly.cn

[Q85] 数值取整
来源：http://ls.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zy.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://af.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hi.szsharing.cn

[Q87] JSON 字段做条件
来源：http://nw.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ee.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://tq.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://av.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yy.lnxyls.cn

[Q89] 判断表是否存在
来源：http://lp.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bu.chemitech.net.cn

[Q90] 生成序号列
来源：http://qj.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ff.jctech888.com.cn

================================================================================
来源：http://ug.jctech888.com.cn

R. Bash 专题
来源：http://un.huixinmuqiang.cn

================================================================================
来源：http://eb.521024.cn

[R01] shebang 与严格模式
来源：http://ej.gzmigu.cn

#!/usr/bin/env bash
来源：http://mt.szxytkj.cn

set -euo pipefail
来源：http://ib.panjiajie.cn

[R02] 变量赋值与使用
来源：http://co.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://bo.haigaiapp.cn

[R03] 只读变量
来源：http://sg.szsharing.cn

readonly PI=3.14
来源：http://kw.szsharing.cn

[R04] 位置参数
来源：http://mw.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yi.newstarts.cn

[R05] 参数默认值
来源：http://sw.muxihuayi.cn

name="${1:-default}"
来源：http://lv.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://id.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ks.521024.cn

[R07] if 判断文件
来源：http://hw.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://io.szxytkj.cn

[R08] 数值比较
来源：http://oi.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tr.huixinmuqiang.cn

[R09] 字符串比较
来源：http://mq.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pu.nszjky.cn

[R10] 正则匹配
来源：http://et.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gj.huixiangedu.cn

[R11] case 多分支
来源：http://gz.yuntaijiaju.cn

case "$1" in
来源：http://qo.colortex.cn

start) echo "启动" ;;
来源：http://df.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://pp.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://yu.nszjky.cn

esac
来源：http://qs.shxzukj.cn

[R12] for 遍历文件
来源：http://en.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://gv.wgjwhj.cn

[R13] for 计数循环
来源：http://pk.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://jk.haigaiapp.cn

[R14] C 风格 for
来源：http://rz.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bx.lnxyls.cn

[R15] while 逐行读文件
来源：http://vb.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bz.szsharing.cn

[R16] until 等待条件
来源：http://cc.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gv.haigaiapp.cn

[R17] 数组定义与取值
来源：http://fx.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ks.hnjuh.cn

[R18] 遍历数组
来源：http://vp.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qt.yuexingan06.cn

[R19] 数组长度
来源：http://co.jctech888.com.cn

echo "${#arr[@]}"
来源：http://dz.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://mn.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mw.bookmarksfly.cn

[R21] 字符串长度
来源：http://jb.muxihuayi.cn

echo "${#s}"
来源：http://hf.chemitech.net.cn

[R22] 截取子串
来源：http://rs.newstarts.cn

echo "${s:0:5}"
来源：http://vu.jianghongdianzi.cn

[R23] 字符串替换
来源：http://ig.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xh.muxihuayi.cn

[R24] 大小写转换
来源：http://th.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ne.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://bs.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nz.nszjky.cn

[R26] 命令替换
来源：http://od.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://fo.huixinmuqiang.cn

[R27] 算术展开
来源：http://lz.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://xb.huixinmuqiang.cn

[R28] 浮点运算
来源：http://se.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://kw.colortex.cn

[R29] 定义函数
来源：http://rj.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ci.szxytkj.cn

[R30] 函数返回状态码
来源：http://tx.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://ya.9csxet.cn

[R31] 局部变量
来源：http://px.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://ih.bookmarksfly.cn

[R32] 参数个数校验
来源：http://hk.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oi.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://vs.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bd.muxihuayi.cn

[R34] 退出时清理
来源：http://ss.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sc.shtwfgs.cn

[R35] 后台执行并等待
来源：http://pq.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xn.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://wc.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qd.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://lz.nszjky.cn

files=$(ls -1)
来源：http://ai.huixiangedu.cn

[R38] 管道串联
来源：http://pq.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://gb.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://ox.bjjhwx.cn

cmd > out.log 2>&1
来源：http://ey.9csxet.cn

[R40] 追加写日志
来源：http://um.9csxet.cn

echo "log" >> out.log
来源：http://tv.jctech888.com.cn

[R41] 丢弃输出
来源：http://zq.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://vi.yuntaijiaju.cn

[R42] 输入重定向
来源：http://cv.chemitech.net.cn

wc -l < a.txt
来源：http://cg.asd995.cn

[R43] 按名字查找文件
来源：http://ed.shtwfgs.cn

find . -name "*.log" -type f
来源：http://aj.szxytkj.cn

[R44] 按修改时间查找
来源：http://hz.hahajie.cn

find . -mtime -7 -type f
来源：http://un.szxytkj.cn

[R45] 批量删除
来源：http://oo.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://wn.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://no.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ig.asd995.cn

[R47] sed 单行替换
来源：http://er.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yn.huanxung.cn

[R48] awk 取指定列
来源：http://lo.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://us.wgjwhj.cn

[R49] awk 带条件
来源：http://ph.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kn.chemitech.net.cn

[R50] awk 求和
来源：http://ez.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qf.gzmigu.cn

[R51] 排序去重取前几
来源：http://yl.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hw.huixinmuqiang.cn

[R52] 统计行数
来源：http://bu.hnjuh.cn

wc -l a.txt
来源：http://bq.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://zl.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ip.nszjky.cn

[R54] 比较两个文件
来源：http://pq.shtwfgs.cn

diff a.txt b.txt
来源：http://kb.521024.cn

[R55] 压缩与解压
来源：http://jl.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pa.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://cj.hnjuh.cn

scp file user@host:/path/
来源：http://ar.nszjky.cn

[R57] 远程执行命令
来源：http://ny.nszjky.cn

ssh user@host 'uptime'
来源：http://lm.jctech888.com.cn

[R58] 下载文件
来源：http://bb.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://it.jctech888.com.cn

[R59] 发 POST JSON
来源：http://db.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qi.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://qt.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zm.shtwfgs.cn

[R61] 磁盘占用
来源：http://sd.shtwfgs.cn

df -h;  du -sh *
来源：http://jk.panjiajie.cn

[R62] 找最占空间的文件
来源：http://zd.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://ay.szsharing.cn

[R63] 内存与进程
来源：http://gb.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://qf.huanxung.cn

[R64] 结束进程
来源：http://mc.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://di.bookmarksfly.cn

[R65] 查看端口占用
来源：http://kr.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bq.yuntaijiaju.cn

[R66] 定时任务
来源：http://iq.shtwfgs.cn

crontab -e;  crontab -l
来源：http://bd.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://wy.bjjhwx.cn

openssl rand -hex 16
来源：http://lr.hnjuh.cn

[R68] 计算文件校验值
来源：http://cq.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fh.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://nt.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://ip.gzmigu.cn

[R70] 时间戳与互转
来源：http://ni.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://ue.lnxyls.cn

[R71] 日期格式化
来源：http://nc.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oe.asd995.cn

[R72] 等待端口就绪
来源：http://op.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hd.colortex.cn

[R73] 分割大日志
来源：http://my.bjjhwx.cn


<!-- 参考信息 -->