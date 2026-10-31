代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vs.panjiajie.cn

[Q24] 去重
来源：http://ii.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://oy.asd995.cn

[Q25] 只取前 N 条
来源：http://qv.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ao.hnjuh.cn

[Q26] 计数
来源：http://tq.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://ic.huixinmuqiang.cn

[Q27] 条件计数
来源：http://ye.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kv.hahajie.cn

[Q28] 求和与平均
来源：http://bz.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ty.muxihuayi.cn

[Q29] 最大最小值
来源：http://yw.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yb.colortex.cn

[Q30] 分组统计
来源：http://os.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bh.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://zh.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://co.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://qk.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jo.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jc.bjjhwx.cn

[Q33] 多列分组
来源：http://ch.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dc.nszjky.cn

[Q34] 每组取第一条
来源：http://fv.chemitech.net.cn

SELECT * FROM (
来源：http://jl.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ou.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://aa.9csxet.cn

[Q35] 内连接
来源：http://zd.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oc.shtwfgs.cn

[Q36] 左连接
来源：http://yi.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pn.bjjhwx.cn

[Q37] 右连接
来源：http://bp.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wo.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mv.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jd.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://sy.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dg.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lw.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ly.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://st.shtwfgs.cn

[Q41] 多表连接
来源：http://lo.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zx.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://oh.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://ke.521024.cn

[Q42] 连接条件附加过滤
来源：http://aq.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://wh.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tf.shxzskj.cn

[Q43] 标量子查询
来源：http://jl.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://af.nszjky.cn

[Q44] IN 子查询
来源：http://cg.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ay.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://fk.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ki.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://du.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zk.lnxyls.cn

[Q47] 与平均值比较
来源：http://zm.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gl.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://bk.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wy.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://yk.newstarts.cn

[Q49] 更新单行
来源：http://vg.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ep.yuexingan06.cn

[Q50] 批量更新
来源：http://gz.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kp.huanxung.cn

[Q51] 用子查询更新
来源：http://gl.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fk.9csxet.cn

[Q52] 删除指定行
来源：http://gf.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://fr.wgjwhj.cn

[Q53] 按条件删除
来源：http://yf.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rg.yuexingan06.cn

[Q54] 清空表
来源：http://ox.521024.cn

TRUNCATE TABLE logs;
来源：http://cg.nicolike.cn

[Q55] 排名（并列占位）
来源：http://bb.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ki.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://ol.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vj.shtwfgs.cn

[Q57] 行号
来源：http://vw.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jv.muxihuayi.cn

[Q58] 累计求和
来源：http://wi.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wu.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://rf.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wp.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://af.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sr.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nu.bookmarksfly.cn

[Q61] 移动平均
来源：http://cf.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xz.yuexingan06.cn

[Q62] 分组占比
来源：http://op.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jh.521024.cn

[Q63] 开启事务
来源：http://mf.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bm.yuexingan06.cn

[Q64] 提交事务
来源：http://al.nicolike.cn

COMMIT;
来源：http://mg.shxzskj.cn

[Q65] 回滚事务
来源：http://ku.bookmarksfly.cn

ROLLBACK;
来源：http://td.nszjky.cn

[Q66] 行锁查询
来源：http://sw.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ps.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://cv.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://js.shxzukj.cn

[Q68] 保存点
来源：http://cg.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://ib.nicolike.cn

ROLLBACK TO sp1;
来源：http://wk.panjiajie.cn

[Q69] 查看执行计划
来源：http://rf.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dq.shxzskj.cn

[Q70] 更新统计信息
来源：http://vp.haigaiapp.cn

ANALYZE TABLE users;
来源：http://vb.lnxyls.cn

[Q71] 查看建表语句
来源：http://ry.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fs.huixiangedu.cn

[Q72] 查看索引
来源：http://cg.szxytkj.cn

SHOW INDEX FROM users;
来源：http://hv.szsharing.cn

[Q73] 查看表状态
来源：http://of.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wt.nszjky.cn

[Q74] 强制使用索引
来源：http://ri.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://no.muxihuayi.cn

[Q75] 日期格式化
来源：http://rx.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tc.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sv.9csxet.cn

[Q76] 按天统计
来源：http://xv.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zc.yuntaijiaju.cn

[Q77] 时间加减
来源：http://xb.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ui.szxytkj.cn

[Q78] 当前时间
来源：http://uj.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hy.hnjuh.cn

[Q79] 字符串拼接
来源：http://mk.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jm.newstarts.cn

[Q80] 字符串截取
来源：http://vd.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qf.shxzukj.cn

[Q81] 字符串替换
来源：http://il.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://co.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://ll.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gx.muxihuayi.cn

[Q83] 大小写转换
来源：http://np.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vx.hnjuh.cn

[Q84] 去除首尾空格
来源：http://gc.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://cl.yuexingan06.cn

[Q85] 数值取整
来源：http://yr.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://os.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://oo.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zr.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://bs.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ab.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://fd.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jy.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vq.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://jn.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ke.9csxet.cn

[Q90] 生成序号列
来源：http://hx.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ez.shxzskj.cn

================================================================================
来源：http://wp.bookmarksfly.cn

R. Bash 专题
来源：http://js.hnjuh.cn

================================================================================
来源：http://dc.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://fl.bjjhwx.cn

#!/usr/bin/env bash
来源：http://ch.jctech888.com.cn

set -euo pipefail
来源：http://rx.hahajie.cn

[R02] 变量赋值与使用
来源：http://ys.nicolike.cn

name="Tom"; echo "$name"
来源：http://kq.muxihuayi.cn

[R03] 只读变量
来源：http://ck.huanxung.cn

readonly PI=3.14
来源：http://uj.hnjuh.cn

[R04] 位置参数
来源：http://zo.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qv.muxihuayi.cn

[R05] 参数默认值
来源：http://xc.asd995.cn

name="${1:-default}"
来源：http://za.gzmigu.cn

[R06] 判断命令是否存在
来源：http://op.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rv.9csxet.cn

[R07] if 判断文件
来源：http://qf.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gp.shxzukj.cn

[R08] 数值比较
来源：http://ge.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ez.yuntaijiaju.cn

[R09] 字符串比较
来源：http://af.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yf.yuntaijiaju.cn

[R10] 正则匹配
来源：http://by.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tv.huanxung.cn

[R11] case 多分支
来源：http://vs.lnxyls.cn

case "$1" in
来源：http://iz.muxihuayi.cn

start) echo "启动" ;;
来源：http://ej.521024.cn

stop)  echo "停止" ;;
来源：http://tb.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://qd.shxzukj.cn

esac
来源：http://ab.huixiangedu.cn

[R12] for 遍历文件
来源：http://rz.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://qq.bjjhwx.cn

[R13] for 计数循环
来源：http://rc.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://jc.chemitech.net.cn

[R14] C 风格 for
来源：http://gr.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://af.shxzskj.cn

[R15] while 逐行读文件
来源：http://if.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uz.bookmarksfly.cn

[R16] until 等待条件
来源：http://nz.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fo.haigaiapp.cn

[R17] 数组定义与取值
来源：http://zb.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xs.yuntaijiaju.cn

[R18] 遍历数组
来源：http://xr.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pu.haigaiapp.cn

[R19] 数组长度
来源：http://qu.huixiangedu.cn

echo "${#arr[@]}"
来源：http://sw.szxytkj.cn

[R20] 关联数组（字典）
来源：http://qf.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ek.hnjuh.cn

[R21] 字符串长度
来源：http://ot.hahajie.cn

echo "${#s}"
来源：http://et.jctech888.com.cn

[R22] 截取子串
来源：http://gw.521024.cn

echo "${s:0:5}"
来源：http://sh.shtwfgs.cn

[R23] 字符串替换
来源：http://xv.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tt.shxzskj.cn

[R24] 大小写转换
来源：http://uy.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lg.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://vt.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ro.asd995.cn

[R26] 命令替换
来源：http://yv.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://ah.9csxet.cn

[R27] 算术展开
来源：http://vv.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://ke.muxihuayi.cn

[R28] 浮点运算
来源：http://oe.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://hg.szxytkj.cn

[R29] 定义函数
来源：http://oq.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dt.colortex.cn

[R30] 函数返回状态码
来源：http://ps.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://lm.gzmigu.cn

[R31] 局部变量
来源：http://yr.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://ki.shxzskj.cn

[R32] 参数个数校验
来源：http://rm.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ab.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://yg.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cr.panjiajie.cn

[R34] 退出时清理
来源：http://bw.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eg.gzmigu.cn

[R35] 后台执行并等待
来源：http://us.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ze.nicolike.cn

[R36] 并发执行多个任务
来源：http://re.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://od.colortex.cn

[R37] 把输出赋给变量
来源：http://hx.panjiajie.cn

files=$(ls -1)
来源：http://nc.521024.cn

[R38] 管道串联
来源：http://vy.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://ba.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://pz.szxytkj.cn

cmd > out.log 2>&1
来源：http://eb.nicolike.cn

[R40] 追加写日志
来源：http://he.hahajie.cn

echo "log" >> out.log
来源：http://gc.asd995.cn

[R41] 丢弃输出
来源：http://ro.newstarts.cn

cmd >/dev/null 2>&1
来源：http://pr.muxihuayi.cn

[R42] 输入重定向
来源：http://zz.shxzukj.cn

wc -l < a.txt
来源：http://rt.jctech888.com.cn

[R43] 按名字查找文件
来源：http://vx.panjiajie.cn

find . -name "*.log" -type f
来源：http://lw.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://jy.jctech888.com.cn

find . -mtime -7 -type f
来源：http://cc.haigaiapp.cn

[R45] 批量删除
来源：http://kj.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://gs.nszjky.cn

[R46] 递归替换文件内容
来源：http://nc.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pl.szsharing.cn

[R47] sed 单行替换
来源：http://xx.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jo.nszjky.cn

[R48] awk 取指定列
来源：http://eo.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://wa.yuntaijiaju.cn

[R49] awk 带条件
来源：http://un.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://se.hahajie.cn

[R50] awk 求和
来源：http://qv.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ox.shxzukj.cn

[R51] 排序去重取前几
来源：http://sp.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kd.szxytkj.cn

[R52] 统计行数
来源：http://le.jctech888.com.cn

wc -l a.txt
来源：http://bz.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://ug.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://av.9csxet.cn

[R54] 比较两个文件
来源：http://zj.shxzukj.cn

diff a.txt b.txt
来源：http://qh.521024.cn

[R55] 压缩与解压
来源：http://xs.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ge.gzmigu.cn

[R56] 远程拷贝
来源：http://pu.bjjhwx.cn

scp file user@host:/path/
来源：http://wq.hahajie.cn

[R57] 远程执行命令
来源：http://tz.gzmigu.cn

ssh user@host 'uptime'
来源：http://iu.9csxet.cn

[R58] 下载文件
来源：http://ki.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mr.huanxung.cn

[R59] 发 POST JSON
来源：http://az.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cb.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://eq.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gd.yuexingan06.cn

[R61] 磁盘占用
来源：http://bg.shxzskj.cn

df -h;  du -sh *
来源：http://rp.colortex.cn

[R62] 找最占空间的文件
来源：http://ub.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://pe.bookmarksfly.cn

[R63] 内存与进程
来源：http://qk.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://sx.jctech888.com.cn

[R64] 结束进程
来源：http://xv.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://ef.bookmarksfly.cn

[R65] 查看端口占用
来源：http://ca.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yg.521024.cn

[R66] 定时任务
来源：http://xv.hahajie.cn

crontab -e;  crontab -l
来源：http://mf.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://gc.chemitech.net.cn

openssl rand -hex 16
来源：http://vy.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://eg.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gp.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://wk.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://zs.9csxet.cn

[R70] 时间戳与互转
来源：http://os.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://aj.chemitech.net.cn

[R71] 日期格式化
来源：http://cy.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qh.lnxyls.cn

[R72] 等待端口就绪
来源：http://zw.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cn.huixinmuqiang.cn

[R73] 分割大日志
来源：http://vr.gzmigu.cn


<!-- 参考信息 -->