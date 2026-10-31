代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://df.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vr.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://de.lnxyls.cn

[Q15] 查询全部
来源：http://wa.nicolike.cn

SELECT * FROM users;
来源：http://yk.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://dz.huanxung.cn

SELECT id, name FROM users;
来源：http://is.nszjky.cn

[Q17] 条件查询
来源：http://sk.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xv.nszjky.cn

[Q18] 模糊匹配
来源：http://ud.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lh.yuexingan06.cn

[Q19] 范围查询
来源：http://pb.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uy.huixinmuqiang.cn

[Q20] IN 列表
来源：http://dr.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mm.asd995.cn

[Q21] 空值判断
来源：http://er.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nb.szsharing.cn

[Q22] 排序
来源：http://oc.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://my.newstarts.cn

[Q23] 分页
来源：http://di.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ns.521024.cn

[Q24] 去重
来源：http://wi.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://lw.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://va.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pb.gzmigu.cn

[Q26] 计数
来源：http://me.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://ee.jianghongdianzi.cn

[Q27] 条件计数
来源：http://gv.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ep.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://xq.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zp.9csxet.cn

[Q29] 最大最小值
来源：http://it.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jf.jctech888.com.cn

[Q30] 分组统计
来源：http://yg.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nk.hnjuh.cn

[Q31] 分组后过滤
来源：http://vp.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iw.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://lq.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fs.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ov.panjiajie.cn

[Q33] 多列分组
来源：http://gi.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jz.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://si.yuexingan06.cn

SELECT * FROM (
来源：http://ay.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rx.jctech888.com.cn

) t WHERE rn = 1;
来源：http://cv.chemitech.net.cn

[Q35] 内连接
来源：http://ex.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xr.lnxyls.cn

[Q36] 左连接
来源：http://yt.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ig.asd995.cn

[Q37] 右连接
来源：http://ni.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xh.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ag.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://us.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://ni.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://py.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ay.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rj.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nh.wgjwhj.cn

[Q41] 多表连接
来源：http://eu.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bm.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://ya.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://kv.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://zw.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://wj.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fn.chemitech.net.cn

[Q43] 标量子查询
来源：http://wx.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ni.shxzukj.cn

[Q44] IN 子查询
来源：http://op.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dk.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://iw.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qe.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jy.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mu.bjjhwx.cn

[Q47] 与平均值比较
来源：http://th.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dj.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://ay.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wp.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://yl.asd995.cn

[Q49] 更新单行
来源：http://ho.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kq.panjiajie.cn

[Q50] 批量更新
来源：http://lb.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vx.chemitech.net.cn

[Q51] 用子查询更新
来源：http://jw.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pz.9csxet.cn

[Q52] 删除指定行
来源：http://si.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://aj.jctech888.com.cn

[Q53] 按条件删除
来源：http://rm.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pr.nszjky.cn

[Q54] 清空表
来源：http://sx.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://zj.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://pu.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wo.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://vj.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dx.newstarts.cn

[Q57] 行号
来源：http://tq.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vl.huanxung.cn

[Q58] 累计求和
来源：http://mu.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rs.huixiangedu.cn

[Q59] 分组内累计
来源：http://pk.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hk.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://rs.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ho.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pt.9csxet.cn

[Q61] 移动平均
来源：http://bp.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fw.wgjwhj.cn

[Q62] 分组占比
来源：http://bc.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ol.9csxet.cn

[Q63] 开启事务
来源：http://cp.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gf.nicolike.cn

[Q64] 提交事务
来源：http://am.szsharing.cn

COMMIT;
来源：http://zq.haigaiapp.cn

[Q65] 回滚事务
来源：http://ti.haigaiapp.cn

ROLLBACK;
来源：http://jx.nszjky.cn

[Q66] 行锁查询
来源：http://ik.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cx.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://rn.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kz.shxzukj.cn

[Q68] 保存点
来源：http://me.nszjky.cn

SAVEPOINT sp1;
来源：http://oq.521024.cn

ROLLBACK TO sp1;
来源：http://rf.nszjky.cn

[Q69] 查看执行计划
来源：http://ex.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nt.521024.cn

[Q70] 更新统计信息
来源：http://ql.nicolike.cn

ANALYZE TABLE users;
来源：http://zq.shtwfgs.cn

[Q71] 查看建表语句
来源：http://dz.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dp.hnjuh.cn

[Q72] 查看索引
来源：http://lq.hnjuh.cn

SHOW INDEX FROM users;
来源：http://kf.panjiajie.cn

[Q73] 查看表状态
来源：http://ax.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qu.colortex.cn

[Q74] 强制使用索引
来源：http://vx.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ht.9csxet.cn

[Q75] 日期格式化
来源：http://ll.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jl.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eo.muxihuayi.cn

[Q76] 按天统计
来源：http://co.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qi.panjiajie.cn

[Q77] 时间加减
来源：http://rv.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bz.shxzskj.cn

[Q78] 当前时间
来源：http://op.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dm.newstarts.cn

[Q79] 字符串拼接
来源：http://jp.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zt.haigaiapp.cn

[Q80] 字符串截取
来源：http://kz.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uz.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://ml.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bh.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://fg.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zs.huixiangedu.cn

[Q83] 大小写转换
来源：http://ua.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fr.panjiajie.cn

[Q84] 去除首尾空格
来源：http://py.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://da.nszjky.cn

[Q85] 数值取整
来源：http://ur.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ig.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://uq.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cs.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://ew.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dk.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://qt.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sc.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fj.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://wt.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xj.bookmarksfly.cn

[Q90] 生成序号列
来源：http://me.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xj.shtwfgs.cn

================================================================================
来源：http://aa.yuntaijiaju.cn

R. Bash 专题
来源：http://ex.521024.cn

================================================================================
来源：http://zm.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://tz.hnjuh.cn

#!/usr/bin/env bash
来源：http://jv.shxzukj.cn

set -euo pipefail
来源：http://gi.shxzskj.cn

[R02] 变量赋值与使用
来源：http://ab.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://kh.huanxung.cn

[R03] 只读变量
来源：http://sn.nszjky.cn

readonly PI=3.14
来源：http://tw.wgjwhj.cn

[R04] 位置参数
来源：http://mq.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wu.521024.cn

[R05] 参数默认值
来源：http://ee.lnxyls.cn

name="${1:-default}"
来源：http://so.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://pg.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kj.newstarts.cn

[R07] if 判断文件
来源：http://mp.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pi.hnjuh.cn

[R08] 数值比较
来源：http://fa.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zu.szxytkj.cn

[R09] 字符串比较
来源：http://rx.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zm.huixinmuqiang.cn

[R10] 正则匹配
来源：http://gs.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kj.9csxet.cn

[R11] case 多分支
来源：http://ao.asd995.cn

case "$1" in
来源：http://vc.521024.cn

start) echo "启动" ;;
来源：http://qq.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://wv.szsharing.cn

*)     echo "未知命令" ;;
来源：http://ik.lnxyls.cn

esac
来源：http://kc.shtwfgs.cn

[R12] for 遍历文件
来源：http://ne.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://dc.jianghongdianzi.cn

[R13] for 计数循环
来源：http://zk.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://sg.newstarts.cn

[R14] C 风格 for
来源：http://yx.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.huanxung.cn

[R15] while 逐行读文件
来源：http://ug.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rj.yuexingan06.cn

[R16] until 等待条件
来源：http://du.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bo.huanxung.cn

[R17] 数组定义与取值
来源：http://vk.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oo.panjiajie.cn

[R18] 遍历数组
来源：http://zf.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ro.jctech888.com.cn

[R19] 数组长度
来源：http://kc.huixiangedu.cn

echo "${#arr[@]}"
来源：http://bz.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://og.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://im.nicolike.cn

[R21] 字符串长度
来源：http://fw.muxihuayi.cn

echo "${#s}"
来源：http://ug.huixiangedu.cn

[R22] 截取子串
来源：http://tj.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://dn.shxzskj.cn

[R23] 字符串替换
来源：http://vs.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sk.newstarts.cn

[R24] 大小写转换
来源：http://js.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lr.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://mf.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ir.newstarts.cn

[R26] 命令替换
来源：http://bu.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://fn.wgjwhj.cn

[R27] 算术展开
来源：http://ph.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://rv.jianghongdianzi.cn

[R28] 浮点运算
来源：http://im.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://zl.huixinmuqiang.cn

[R29] 定义函数
来源：http://rs.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tz.muxihuayi.cn

[R30] 函数返回状态码
来源：http://um.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://eo.shxzskj.cn

[R31] 局部变量
来源：http://bk.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://ds.nicolike.cn

[R32] 参数个数校验
来源：http://ar.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jo.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://dl.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uo.lnxyls.cn

[R34] 退出时清理
来源：http://nv.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lr.shxzskj.cn

[R35] 后台执行并等待
来源：http://lf.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yj.panjiajie.cn

[R36] 并发执行多个任务
来源：http://fk.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nn.gzmigu.cn

[R37] 把输出赋给变量
来源：http://zj.hnjuh.cn

files=$(ls -1)
来源：http://hg.hahajie.cn

[R38] 管道串联
来源：http://ki.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://gl.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://vc.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://ww.jctech888.com.cn

[R40] 追加写日志
来源：http://if.nicolike.cn

echo "log" >> out.log
来源：http://dw.asd995.cn

[R41] 丢弃输出
来源：http://zw.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://bo.jianghongdianzi.cn

[R42] 输入重定向
来源：http://km.szsharing.cn

wc -l < a.txt
来源：http://ha.asd995.cn

[R43] 按名字查找文件
来源：http://so.huanxung.cn

find . -name "*.log" -type f
来源：http://rw.yuexingan06.cn

[R44] 按修改时间查找
来源：http://kb.panjiajie.cn

find . -mtime -7 -type f
来源：http://xx.hahajie.cn

[R45] 批量删除
来源：http://lk.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://nr.hahajie.cn

[R46] 递归替换文件内容
来源：http://st.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fe.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://ix.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nk.wgjwhj.cn

[R48] awk 取指定列
来源：http://lp.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://hd.jianghongdianzi.cn

[R49] awk 带条件
来源：http://ip.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fb.yuntaijiaju.cn

[R50] awk 求和
来源：http://ey.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nr.jctech888.com.cn

[R51] 排序去重取前几
来源：http://pw.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yi.lnxyls.cn

[R52] 统计行数
来源：http://ma.521024.cn

wc -l a.txt
来源：http://rp.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://po.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://do.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://oo.521024.cn

diff a.txt b.txt
来源：http://sw.lnxyls.cn

[R55] 压缩与解压
来源：http://ja.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iz.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ak.bjjhwx.cn

scp file user@host:/path/
来源：http://dp.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://qr.bjjhwx.cn

ssh user@host 'uptime'
来源：http://cv.huanxung.cn

[R58] 下载文件
来源：http://kd.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fe.newstarts.cn

[R59] 发 POST JSON
来源：http://av.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fm.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://rg.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://js.shxzskj.cn

[R61] 磁盘占用
来源：http://hx.jctech888.com.cn

df -h;  du -sh *
来源：http://so.hnjuh.cn

[R62] 找最占空间的文件
来源：http://zm.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://uo.szxytkj.cn

[R63] 内存与进程
来源：http://uk.wgjwhj.cn


<!-- 参考信息 -->