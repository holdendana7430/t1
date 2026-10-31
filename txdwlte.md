代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wa.shtwfgs.cn

[Q24] 去重
来源：http://km.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://bb.shxzukj.cn

[Q25] 只取前 N 条
来源：http://bc.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jk.muxihuayi.cn

[Q26] 计数
来源：http://xw.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://od.huixinmuqiang.cn

[Q27] 条件计数
来源：http://mj.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cd.asd995.cn

[Q28] 求和与平均
来源：http://si.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vn.yuexingan06.cn

[Q29] 最大最小值
来源：http://xn.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zv.bjjhwx.cn

[Q30] 分组统计
来源：http://kz.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jr.gzmigu.cn

[Q31] 分组后过滤
来源：http://zg.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kp.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://ws.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ss.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bp.gzmigu.cn

[Q33] 多列分组
来源：http://lw.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sr.bjjhwx.cn

[Q34] 每组取第一条
来源：http://nd.huixiangedu.cn

SELECT * FROM (
来源：http://gd.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://da.hahajie.cn

) t WHERE rn = 1;
来源：http://zy.colortex.cn

[Q35] 内连接
来源：http://rk.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hy.gzmigu.cn

[Q36] 左连接
来源：http://po.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ej.yuntaijiaju.cn

[Q37] 右连接
来源：http://ma.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jy.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kv.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jk.asd995.cn

[Q39] 自连接（查上下级）
来源：http://am.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://so.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://co.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ow.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ka.bookmarksfly.cn

[Q41] 多表连接
来源：http://wu.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hm.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://by.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://nb.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://vo.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://gi.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nk.bookmarksfly.cn

[Q43] 标量子查询
来源：http://jt.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sr.huixiangedu.cn

[Q44] IN 子查询
来源：http://cg.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fw.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ob.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kq.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://he.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cu.chemitech.net.cn

[Q47] 与平均值比较
来源：http://pw.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ml.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://fm.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qj.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://ii.shxzukj.cn

[Q49] 更新单行
来源：http://ir.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nn.shxzskj.cn

[Q50] 批量更新
来源：http://ro.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vn.9csxet.cn

[Q51] 用子查询更新
来源：http://fx.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gq.wgjwhj.cn

[Q52] 删除指定行
来源：http://nw.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://hg.bjjhwx.cn

[Q53] 按条件删除
来源：http://ks.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bz.gzmigu.cn

[Q54] 清空表
来源：http://um.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://xm.nicolike.cn

[Q55] 排名（并列占位）
来源：http://rx.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vx.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://za.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tg.nicolike.cn

[Q57] 行号
来源：http://or.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ov.jianghongdianzi.cn

[Q58] 累计求和
来源：http://vy.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qs.shxzukj.cn

[Q59] 分组内累计
来源：http://ku.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rc.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://ed.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ig.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sc.jianghongdianzi.cn

[Q61] 移动平均
来源：http://rc.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mh.bookmarksfly.cn

[Q62] 分组占比
来源：http://nh.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iv.hnjuh.cn

[Q63] 开启事务
来源：http://pc.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://de.shtwfgs.cn

[Q64] 提交事务
来源：http://vc.huixiangedu.cn

COMMIT;
来源：http://rp.hahajie.cn

[Q65] 回滚事务
来源：http://eh.huixiangedu.cn

ROLLBACK;
来源：http://mq.nszjky.cn

[Q66] 行锁查询
来源：http://lb.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ti.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://bk.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ls.yuntaijiaju.cn

[Q68] 保存点
来源：http://jt.bjjhwx.cn

SAVEPOINT sp1;
来源：http://yu.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://kl.szsharing.cn

[Q69] 查看执行计划
来源：http://ic.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://to.colortex.cn

[Q70] 更新统计信息
来源：http://rd.colortex.cn

ANALYZE TABLE users;
来源：http://pw.haigaiapp.cn

[Q71] 查看建表语句
来源：http://hu.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nx.jianghongdianzi.cn

[Q72] 查看索引
来源：http://ed.szxytkj.cn

SHOW INDEX FROM users;
来源：http://tb.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://qz.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mw.jctech888.com.cn

[Q74] 强制使用索引
来源：http://zi.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qt.huixiangedu.cn

[Q75] 日期格式化
来源：http://se.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pz.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gi.huanxung.cn

[Q76] 按天统计
来源：http://lk.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jt.chemitech.net.cn

[Q77] 时间加减
来源：http://kg.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vd.shxzukj.cn

[Q78] 当前时间
来源：http://dk.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sl.colortex.cn

[Q79] 字符串拼接
来源：http://et.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sf.chemitech.net.cn

[Q80] 字符串截取
来源：http://ru.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ff.szxytkj.cn

[Q81] 字符串替换
来源：http://zx.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ei.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://hz.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://st.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://px.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wh.hnjuh.cn

[Q84] 去除首尾空格
来源：http://hh.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://bt.szsharing.cn

[Q85] 数值取整
来源：http://cd.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pa.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://tp.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ml.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://nm.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://md.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://vc.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ev.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zw.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://tc.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cg.bookmarksfly.cn

[Q90] 生成序号列
来源：http://cv.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://th.huixiangedu.cn

================================================================================
来源：http://yx.gzmigu.cn

R. Bash 专题
来源：http://kw.szxytkj.cn

================================================================================
来源：http://ue.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://mw.panjiajie.cn

#!/usr/bin/env bash
来源：http://od.lnxyls.cn

set -euo pipefail
来源：http://kt.nicolike.cn

[R02] 变量赋值与使用
来源：http://fy.hnjuh.cn

name="Tom"; echo "$name"
来源：http://nd.jianghongdianzi.cn

[R03] 只读变量
来源：http://tz.yuntaijiaju.cn

readonly PI=3.14
来源：http://vy.jctech888.com.cn

[R04] 位置参数
来源：http://go.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://so.bookmarksfly.cn

[R05] 参数默认值
来源：http://wi.haigaiapp.cn

name="${1:-default}"
来源：http://au.9csxet.cn

[R06] 判断命令是否存在
来源：http://xt.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rt.chemitech.net.cn

[R07] if 判断文件
来源：http://jx.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mc.lnxyls.cn

[R08] 数值比较
来源：http://zn.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dt.lnxyls.cn

[R09] 字符串比较
来源：http://aw.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nl.nszjky.cn

[R10] 正则匹配
来源：http://ue.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zm.szsharing.cn

[R11] case 多分支
来源：http://tj.colortex.cn

case "$1" in
来源：http://ns.colortex.cn

start) echo "启动" ;;
来源：http://qw.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://ha.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://ic.huixinmuqiang.cn

esac
来源：http://dg.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://oa.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://mx.gzmigu.cn

[R13] for 计数循环
来源：http://oc.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://tt.panjiajie.cn

[R14] C 风格 for
来源：http://rk.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tx.hnjuh.cn

[R15] while 逐行读文件
来源：http://ma.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cp.yuntaijiaju.cn

[R16] until 等待条件
来源：http://xq.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zo.panjiajie.cn

[R17] 数组定义与取值
来源：http://db.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ey.hnjuh.cn

[R18] 遍历数组
来源：http://zg.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://or.9csxet.cn

[R19] 数组长度
来源：http://qw.chemitech.net.cn

echo "${#arr[@]}"
来源：http://cv.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://uv.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ri.shtwfgs.cn

[R21] 字符串长度
来源：http://ck.asd995.cn

echo "${#s}"
来源：http://je.shxzskj.cn

[R22] 截取子串
来源：http://oj.gzmigu.cn

echo "${s:0:5}"
来源：http://zh.9csxet.cn

[R23] 字符串替换
来源：http://zw.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sj.haigaiapp.cn

[R24] 大小写转换
来源：http://eu.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oi.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://rz.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ga.huixinmuqiang.cn

[R26] 命令替换
来源：http://fp.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://oh.nszjky.cn

[R27] 算术展开
来源：http://fe.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://hd.chemitech.net.cn

[R28] 浮点运算
来源：http://su.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://tj.9csxet.cn

[R29] 定义函数
来源：http://jp.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://px.hahajie.cn

[R30] 函数返回状态码
来源：http://uw.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://cg.yuexingan06.cn

[R31] 局部变量
来源：http://ud.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://eg.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://va.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dp.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://lf.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dl.panjiajie.cn

[R34] 退出时清理
来源：http://ds.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qd.9csxet.cn

[R35] 后台执行并等待
来源：http://yd.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dm.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://qf.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xw.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://zt.chemitech.net.cn

files=$(ls -1)
来源：http://sj.nszjky.cn

[R38] 管道串联
来源：http://my.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://na.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://dm.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://dg.521024.cn

[R40] 追加写日志
来源：http://md.521024.cn

echo "log" >> out.log
来源：http://zm.9csxet.cn

[R41] 丢弃输出
来源：http://fi.9csxet.cn

cmd >/dev/null 2>&1
来源：http://oa.panjiajie.cn

[R42] 输入重定向
来源：http://km.szxytkj.cn

wc -l < a.txt
来源：http://vx.szsharing.cn

[R43] 按名字查找文件
来源：http://ds.huanxung.cn

find . -name "*.log" -type f
来源：http://mr.shxzukj.cn

[R44] 按修改时间查找
来源：http://nx.yuexingan06.cn

find . -mtime -7 -type f
来源：http://ns.nicolike.cn

[R45] 批量删除
来源：http://et.nszjky.cn

find . -name "*.tmp" -delete
来源：http://cs.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://fr.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uh.haigaiapp.cn

[R47] sed 单行替换
来源：http://uv.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://es.nicolike.cn

[R48] awk 取指定列
来源：http://gz.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://es.521024.cn

[R49] awk 带条件
来源：http://sk.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dd.szxytkj.cn

[R50] awk 求和
来源：http://yv.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jc.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://gb.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ep.gzmigu.cn

[R52] 统计行数
来源：http://so.colortex.cn

wc -l a.txt
来源：http://zg.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://lu.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://np.jctech888.com.cn

[R54] 比较两个文件
来源：http://sd.colortex.cn

diff a.txt b.txt
来源：http://bl.asd995.cn

[R55] 压缩与解压
来源：http://xs.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ea.chemitech.net.cn

[R56] 远程拷贝
来源：http://tl.yuexingan06.cn

scp file user@host:/path/
来源：http://ra.hnjuh.cn

[R57] 远程执行命令
来源：http://hq.hnjuh.cn

ssh user@host 'uptime'
来源：http://wx.nszjky.cn

[R58] 下载文件
来源：http://hn.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://be.muxihuayi.cn

[R59] 发 POST JSON
来源：http://zl.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hl.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://ft.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ao.shxzukj.cn

[R61] 磁盘占用
来源：http://qj.jianghongdianzi.cn

df -h;  du -sh *
来源：http://md.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://of.asd995.cn

du -ah . | sort -rh | head -10
来源：http://uu.shxzukj.cn

[R63] 内存与进程
来源：http://vg.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://yx.hnjuh.cn

[R64] 结束进程
来源：http://tz.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://aq.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://na.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cb.szsharing.cn

[R66] 定时任务
来源：http://ib.9csxet.cn

crontab -e;  crontab -l
来源：http://nn.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://gv.yuexingan06.cn

openssl rand -hex 16
来源：http://qi.nszjky.cn

[R68] 计算文件校验值
来源：http://lp.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ir.szxytkj.cn

[R69] 生成随机密码
来源：http://rh.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://bp.bjjhwx.cn

[R70] 时间戳与互转
来源：http://se.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://zn.huanxung.cn

[R71] 日期格式化
来源：http://dm.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ic.panjiajie.cn

[R72] 等待端口就绪
来源：http://du.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vt.wgjwhj.cn

[R73] 分割大日志
来源：http://hz.chemitech.net.cn


<!-- 参考信息 -->