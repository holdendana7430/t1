代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://tj.bjjhwx.cn

[Q22] 排序
来源：http://wy.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rd.chemitech.net.cn

[Q23] 分页
来源：http://jd.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dj.huanxung.cn

[Q24] 去重
来源：http://ej.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://if.szsharing.cn

[Q25] 只取前 N 条
来源：http://zq.yuexingan06.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dr.newstarts.cn

[Q26] 计数
来源：http://uy.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://cm.asd995.cn

[Q27] 条件计数
来源：http://wp.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nh.muxihuayi.cn

[Q28] 求和与平均
来源：http://jd.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zb.jctech888.com.cn

[Q29] 最大最小值
来源：http://bk.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aj.szsharing.cn

[Q30] 分组统计
来源：http://rf.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lm.colortex.cn

[Q31] 分组后过滤
来源：http://it.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pj.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://eu.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uf.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zt.shxzukj.cn

[Q33] 多列分组
来源：http://ir.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ar.haigaiapp.cn

[Q34] 每组取第一条
来源：http://rm.huanxung.cn

SELECT * FROM (
来源：http://ti.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oy.nszjky.cn

) t WHERE rn = 1;
来源：http://dv.9csxet.cn

[Q35] 内连接
来源：http://lo.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rq.huixinmuqiang.cn

[Q36] 左连接
来源：http://vn.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ju.9csxet.cn

[Q37] 右连接
来源：http://ho.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gn.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ef.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://so.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://uj.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fj.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yh.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xj.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iy.szsharing.cn

[Q41] 多表连接
来源：http://pm.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://an.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://uj.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://js.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://kh.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://at.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wm.shtwfgs.cn

[Q43] 标量子查询
来源：http://wa.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hn.nicolike.cn

[Q44] IN 子查询
来源：http://pv.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yu.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://lb.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hk.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ad.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tr.colortex.cn

[Q47] 与平均值比较
来源：http://pg.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://td.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://px.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ud.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://bm.shxzskj.cn

[Q49] 更新单行
来源：http://ul.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bl.szxytkj.cn

[Q50] 批量更新
来源：http://hm.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wt.muxihuayi.cn

[Q51] 用子查询更新
来源：http://jc.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://av.lnxyls.cn

[Q52] 删除指定行
来源：http://zq.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://dh.colortex.cn

[Q53] 按条件删除
来源：http://ll.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ue.asd995.cn

[Q54] 清空表
来源：http://iv.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://sg.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://fu.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hj.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://bv.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gz.shxzukj.cn

[Q57] 行号
来源：http://mc.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cu.nicolike.cn

[Q58] 累计求和
来源：http://fx.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yp.shtwfgs.cn

[Q59] 分组内累计
来源：http://xd.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kq.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://nw.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wy.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pg.huixiangedu.cn

[Q61] 移动平均
来源：http://kh.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vb.gzmigu.cn

[Q62] 分组占比
来源：http://rl.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lx.bjjhwx.cn

[Q63] 开启事务
来源：http://zm.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://je.huixinmuqiang.cn

[Q64] 提交事务
来源：http://vx.hnjuh.cn

COMMIT;
来源：http://xl.shxzskj.cn

[Q65] 回滚事务
来源：http://rn.jctech888.com.cn

ROLLBACK;
来源：http://qf.bjjhwx.cn

[Q66] 行锁查询
来源：http://wg.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lg.huanxung.cn

[Q67] 设置隔离级别
来源：http://mr.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ny.gzmigu.cn

[Q68] 保存点
来源：http://gg.wgjwhj.cn

SAVEPOINT sp1;
来源：http://js.shxzukj.cn

ROLLBACK TO sp1;
来源：http://qx.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://wb.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://du.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://tt.gzmigu.cn

ANALYZE TABLE users;
来源：http://ao.9csxet.cn

[Q71] 查看建表语句
来源：http://eh.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qd.gzmigu.cn

[Q72] 查看索引
来源：http://og.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://pg.nicolike.cn

[Q73] 查看表状态
来源：http://ac.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ii.yuexingan06.cn

[Q74] 强制使用索引
来源：http://pi.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cv.nicolike.cn

[Q75] 日期格式化
来源：http://mv.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zb.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fg.hahajie.cn

[Q76] 按天统计
来源：http://ep.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wr.nszjky.cn

[Q77] 时间加减
来源：http://nr.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zj.lnxyls.cn

[Q78] 当前时间
来源：http://yb.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bs.shxzukj.cn

[Q79] 字符串拼接
来源：http://da.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xv.asd995.cn

[Q80] 字符串截取
来源：http://od.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://we.chemitech.net.cn

[Q81] 字符串替换
来源：http://mm.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://av.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://eq.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cc.9csxet.cn

[Q83] 大小写转换
来源：http://vy.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eb.szxytkj.cn

[Q84] 去除首尾空格
来源：http://ip.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://jz.colortex.cn

[Q85] 数值取整
来源：http://aj.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jo.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://dc.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xg.nszjky.cn

[Q87] JSON 字段做条件
来源：http://qy.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://si.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://fd.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gd.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ot.hnjuh.cn

[Q89] 判断表是否存在
来源：http://jf.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gc.gzmigu.cn

[Q90] 生成序号列
来源：http://it.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kr.huixinmuqiang.cn

================================================================================
来源：http://uh.shtwfgs.cn

R. Bash 专题
来源：http://wj.hnjuh.cn

================================================================================
来源：http://te.asd995.cn

[R01] shebang 与严格模式
来源：http://yc.muxihuayi.cn

#!/usr/bin/env bash
来源：http://es.szsharing.cn

set -euo pipefail
来源：http://td.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://wc.colortex.cn

name="Tom"; echo "$name"
来源：http://rq.shxzskj.cn

[R03] 只读变量
来源：http://nl.asd995.cn

readonly PI=3.14
来源：http://jh.huixiangedu.cn

[R04] 位置参数
来源：http://lw.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ea.muxihuayi.cn

[R05] 参数默认值
来源：http://lr.jianghongdianzi.cn

name="${1:-default}"
来源：http://vh.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://ir.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pa.jianghongdianzi.cn

[R07] if 判断文件
来源：http://gq.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lp.szsharing.cn

[R08] 数值比较
来源：http://mu.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eb.yuntaijiaju.cn

[R09] 字符串比较
来源：http://qk.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ca.jianghongdianzi.cn

[R10] 正则匹配
来源：http://px.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dz.muxihuayi.cn

[R11] case 多分支
来源：http://bp.muxihuayi.cn

case "$1" in
来源：http://lx.asd995.cn

start) echo "启动" ;;
来源：http://nc.asd995.cn

stop)  echo "停止" ;;
来源：http://jp.hahajie.cn

*)     echo "未知命令" ;;
来源：http://zv.panjiajie.cn

esac
来源：http://pi.szxytkj.cn

[R12] for 遍历文件
来源：http://un.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://er.9csxet.cn

[R13] for 计数循环
来源：http://lt.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://vv.lnxyls.cn

[R14] C 风格 for
来源：http://ah.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mo.colortex.cn

[R15] while 逐行读文件
来源：http://hx.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lg.lnxyls.cn

[R16] until 等待条件
来源：http://kx.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gm.nszjky.cn

[R17] 数组定义与取值
来源：http://ld.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hs.521024.cn

[R18] 遍历数组
来源：http://hu.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ch.bjjhwx.cn

[R19] 数组长度
来源：http://ya.szxytkj.cn

echo "${#arr[@]}"
来源：http://gr.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://xf.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hx.panjiajie.cn

[R21] 字符串长度
来源：http://uu.bjjhwx.cn

echo "${#s}"
来源：http://nz.asd995.cn

[R22] 截取子串
来源：http://xz.521024.cn

echo "${s:0:5}"
来源：http://ck.haigaiapp.cn

[R23] 字符串替换
来源：http://fo.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yn.lnxyls.cn

[R24] 大小写转换
来源：http://mg.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lz.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://ug.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nm.lnxyls.cn

[R26] 命令替换
来源：http://zr.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://gv.shxzukj.cn

[R27] 算术展开
来源：http://ak.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://gi.newstarts.cn

[R28] 浮点运算
来源：http://gx.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://yf.jctech888.com.cn

[R29] 定义函数
来源：http://kw.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ka.jctech888.com.cn

[R30] 函数返回状态码
来源：http://yj.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://em.bookmarksfly.cn

[R31] 局部变量
来源：http://ih.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://xq.bjjhwx.cn

[R32] 参数个数校验
来源：http://kl.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hv.521024.cn

[R33] 捕获错误并提示行号
来源：http://nq.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jp.jctech888.com.cn

[R34] 退出时清理
来源：http://ba.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rm.shxzskj.cn

[R35] 后台执行并等待
来源：http://nt.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ym.nicolike.cn

[R36] 并发执行多个任务
来源：http://jp.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zw.nicolike.cn

[R37] 把输出赋给变量
来源：http://rn.panjiajie.cn

files=$(ls -1)
来源：http://jo.bookmarksfly.cn

[R38] 管道串联
来源：http://tz.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://gx.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://bw.wgjwhj.cn

cmd > out.log 2>&1
来源：http://zg.521024.cn

[R40] 追加写日志
来源：http://or.bjjhwx.cn

echo "log" >> out.log
来源：http://yr.yuexingan06.cn

[R41] 丢弃输出
来源：http://gf.huanxung.cn

cmd >/dev/null 2>&1
来源：http://or.colortex.cn

[R42] 输入重定向
来源：http://ed.521024.cn

wc -l < a.txt
来源：http://zf.shtwfgs.cn

[R43] 按名字查找文件
来源：http://jz.shxzskj.cn

find . -name "*.log" -type f
来源：http://xq.521024.cn

[R44] 按修改时间查找
来源：http://uz.yuexingan06.cn

find . -mtime -7 -type f
来源：http://hz.9csxet.cn

[R45] 批量删除
来源：http://fr.nicolike.cn

find . -name "*.tmp" -delete
来源：http://uf.nszjky.cn

[R46] 递归替换文件内容
来源：http://vc.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xv.panjiajie.cn

[R47] sed 单行替换
来源：http://sz.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gu.nszjky.cn

[R48] awk 取指定列
来源：http://kj.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://xr.bookmarksfly.cn

[R49] awk 带条件
来源：http://zq.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fv.jianghongdianzi.cn

[R50] awk 求和
来源：http://tz.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fb.jctech888.com.cn

[R51] 排序去重取前几
来源：http://yp.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jz.colortex.cn

[R52] 统计行数
来源：http://yn.newstarts.cn

wc -l a.txt
来源：http://gs.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://cm.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kn.huanxung.cn

[R54] 比较两个文件
来源：http://oh.9csxet.cn

diff a.txt b.txt
来源：http://sc.jctech888.com.cn

[R55] 压缩与解压
来源：http://zx.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lq.hnjuh.cn

[R56] 远程拷贝
来源：http://ql.panjiajie.cn

scp file user@host:/path/
来源：http://lx.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://zy.jctech888.com.cn

ssh user@host 'uptime'
来源：http://gq.hnjuh.cn

[R58] 下载文件
来源：http://lt.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://we.muxihuayi.cn

[R59] 发 POST JSON
来源：http://dy.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rg.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://wv.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ze.wgjwhj.cn

[R61] 磁盘占用
来源：http://bg.hahajie.cn

df -h;  du -sh *
来源：http://rf.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://gp.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://yp.asd995.cn

[R63] 内存与进程
来源：http://fp.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://sh.szsharing.cn

[R64] 结束进程
来源：http://yy.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://pt.lnxyls.cn

[R65] 查看端口占用
来源：http://sg.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kv.wgjwhj.cn

[R66] 定时任务
来源：http://bg.shxzskj.cn

crontab -e;  crontab -l
来源：http://bz.asd995.cn

[R67] 生成随机十六进制串
来源：http://wq.bookmarksfly.cn

openssl rand -hex 16
来源：http://ry.muxihuayi.cn

[R68] 计算文件校验值
来源：http://zs.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ot.hnjuh.cn

[R69] 生成随机密码
来源：http://qr.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://yp.huanxung.cn

[R70] 时间戳与互转
来源：http://tq.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://fv.gzmigu.cn

[R71] 日期格式化
来源：http://qe.huixinmuqiang.cn


<!-- 参考信息 -->