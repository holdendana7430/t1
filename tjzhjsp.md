代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://ff.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pb.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bf.jianghongdianzi.cn

[Q15] 查询全部
来源：http://oe.nszjky.cn

SELECT * FROM users;
来源：http://sc.asd995.cn

[Q16] 查询指定列
来源：http://cc.wgjwhj.cn

SELECT id, name FROM users;
来源：http://gx.hahajie.cn

[Q17] 条件查询
来源：http://np.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qf.9csxet.cn

[Q18] 模糊匹配
来源：http://od.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zj.521024.cn

[Q19] 范围查询
来源：http://gk.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zz.shtwfgs.cn

[Q20] IN 列表
来源：http://ql.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fo.yuntaijiaju.cn

[Q21] 空值判断
来源：http://fy.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://op.jctech888.com.cn

[Q22] 排序
来源：http://zd.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zl.lnxyls.cn

[Q23] 分页
来源：http://ku.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://av.9csxet.cn

[Q24] 去重
来源：http://jm.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://tk.9csxet.cn

[Q25] 只取前 N 条
来源：http://gv.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ae.521024.cn

[Q26] 计数
来源：http://tt.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://sb.newstarts.cn

[Q27] 条件计数
来源：http://op.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nf.chemitech.net.cn

[Q28] 求和与平均
来源：http://qg.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nv.bjjhwx.cn

[Q29] 最大最小值
来源：http://qd.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gr.huanxung.cn

[Q30] 分组统计
来源：http://yy.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://do.521024.cn

[Q31] 分组后过滤
来源：http://tv.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ci.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://fs.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tk.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bm.shxzukj.cn

[Q33] 多列分组
来源：http://cq.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pp.huanxung.cn

[Q34] 每组取第一条
来源：http://pl.muxihuayi.cn

SELECT * FROM (
来源：http://xt.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qn.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://ww.shtwfgs.cn

[Q35] 内连接
来源：http://im.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oo.szxytkj.cn

[Q36] 左连接
来源：http://wm.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iw.jianghongdianzi.cn

[Q37] 右连接
来源：http://ka.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vg.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ce.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yo.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://tp.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cj.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jp.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qx.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://si.shxzukj.cn

[Q41] 多表连接
来源：http://xy.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sq.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://yl.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://jn.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ad.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://pu.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fr.huixiangedu.cn

[Q43] 标量子查询
来源：http://bt.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gm.bookmarksfly.cn

[Q44] IN 子查询
来源：http://io.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ea.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://vn.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ec.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yv.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eq.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://co.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bb.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://hk.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pt.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://as.9csxet.cn

[Q49] 更新单行
来源：http://ci.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uj.gzmigu.cn

[Q50] 批量更新
来源：http://ha.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qg.gzmigu.cn

[Q51] 用子查询更新
来源：http://iz.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ad.panjiajie.cn

[Q52] 删除指定行
来源：http://ue.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://jt.szsharing.cn

[Q53] 按条件删除
来源：http://xg.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ve.colortex.cn

[Q54] 清空表
来源：http://hw.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://dn.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://hq.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mz.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://kj.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lg.gzmigu.cn

[Q57] 行号
来源：http://hy.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ij.huanxung.cn

[Q58] 累计求和
来源：http://yl.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oo.huixiangedu.cn

[Q59] 分组内累计
来源：http://yj.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cv.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://pa.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fh.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tc.hnjuh.cn

[Q61] 移动平均
来源：http://tp.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hg.szxytkj.cn

[Q62] 分组占比
来源：http://cr.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hf.newstarts.cn

[Q63] 开启事务
来源：http://bv.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cw.newstarts.cn

[Q64] 提交事务
来源：http://jq.shxzskj.cn

COMMIT;
来源：http://ad.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://jt.shxzukj.cn

ROLLBACK;
来源：http://zz.521024.cn

[Q66] 行锁查询
来源：http://ag.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://as.hnjuh.cn

[Q67] 设置隔离级别
来源：http://hf.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ya.shtwfgs.cn

[Q68] 保存点
来源：http://dc.colortex.cn

SAVEPOINT sp1;
来源：http://ek.9csxet.cn

ROLLBACK TO sp1;
来源：http://nv.shxzukj.cn

[Q69] 查看执行计划
来源：http://lo.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bs.wgjwhj.cn

[Q70] 更新统计信息
来源：http://rn.nicolike.cn

ANALYZE TABLE users;
来源：http://fs.lnxyls.cn

[Q71] 查看建表语句
来源：http://yl.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mb.szsharing.cn

[Q72] 查看索引
来源：http://gl.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://bz.hahajie.cn

[Q73] 查看表状态
来源：http://rh.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lt.shtwfgs.cn

[Q74] 强制使用索引
来源：http://kv.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cn.huanxung.cn

[Q75] 日期格式化
来源：http://jb.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dc.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zl.huanxung.cn

[Q76] 按天统计
来源：http://cb.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ur.9csxet.cn

[Q77] 时间加减
来源：http://jm.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tc.asd995.cn

[Q78] 当前时间
来源：http://zb.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cp.shxzukj.cn

[Q79] 字符串拼接
来源：http://pp.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ly.wgjwhj.cn

[Q80] 字符串截取
来源：http://xk.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://in.haigaiapp.cn

[Q81] 字符串替换
来源：http://kh.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rl.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://sr.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tv.hahajie.cn

[Q83] 大小写转换
来源：http://xr.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tc.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://id.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://qo.9csxet.cn

[Q85] 数值取整
来源：http://mo.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nv.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://uj.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vi.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://qx.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vt.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://vc.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sb.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bl.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://dn.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wr.szsharing.cn

[Q90] 生成序号列
来源：http://lp.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lm.muxihuayi.cn

================================================================================
来源：http://pf.521024.cn

R. Bash 专题
来源：http://pb.huanxung.cn

================================================================================
来源：http://mo.colortex.cn

[R01] shebang 与严格模式
来源：http://xd.hahajie.cn

#!/usr/bin/env bash
来源：http://ob.huixinmuqiang.cn

set -euo pipefail
来源：http://zv.hnjuh.cn

[R02] 变量赋值与使用
来源：http://ll.nszjky.cn

name="Tom"; echo "$name"
来源：http://tz.nszjky.cn

[R03] 只读变量
来源：http://gm.shtwfgs.cn

readonly PI=3.14
来源：http://wc.asd995.cn

[R04] 位置参数
来源：http://tw.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rz.colortex.cn

[R05] 参数默认值
来源：http://am.bookmarksfly.cn

name="${1:-default}"
来源：http://kn.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://kx.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vw.asd995.cn

[R07] if 判断文件
来源：http://jr.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cx.nszjky.cn

[R08] 数值比较
来源：http://po.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ri.shxzukj.cn

[R09] 字符串比较
来源：http://pj.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dw.shxzukj.cn

[R10] 正则匹配
来源：http://oz.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gs.gzmigu.cn

[R11] case 多分支
来源：http://cc.nszjky.cn

case "$1" in
来源：http://rt.chemitech.net.cn

start) echo "启动" ;;
来源：http://pg.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://qf.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://yi.muxihuayi.cn

esac
来源：http://ww.wgjwhj.cn

[R12] for 遍历文件
来源：http://xk.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://ja.hnjuh.cn

[R13] for 计数循环
来源：http://oq.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://ee.shxzukj.cn

[R14] C 风格 for
来源：http://kj.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lx.szsharing.cn

[R15] while 逐行读文件
来源：http://tz.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ci.panjiajie.cn

[R16] until 等待条件
来源：http://ev.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nw.jctech888.com.cn

[R17] 数组定义与取值
来源：http://sl.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pa.panjiajie.cn

[R18] 遍历数组
来源：http://pi.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hd.huixinmuqiang.cn

[R19] 数组长度
来源：http://dd.hnjuh.cn

echo "${#arr[@]}"
来源：http://ll.hahajie.cn

[R20] 关联数组（字典）
来源：http://mx.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://af.jctech888.com.cn

[R21] 字符串长度
来源：http://ql.szxytkj.cn

echo "${#s}"
来源：http://wb.nicolike.cn

[R22] 截取子串
来源：http://hn.colortex.cn

echo "${s:0:5}"
来源：http://qb.521024.cn

[R23] 字符串替换
来源：http://pr.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iq.newstarts.cn

[R24] 大小写转换
来源：http://wd.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gw.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://kq.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mg.chemitech.net.cn

[R26] 命令替换
来源：http://kh.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://za.jctech888.com.cn

[R27] 算术展开
来源：http://qb.hahajie.cn

echo $((1 + 2 * 3))
来源：http://wk.chemitech.net.cn

[R28] 浮点运算
来源：http://lb.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://hy.jianghongdianzi.cn

[R29] 定义函数
来源：http://pp.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gm.nszjky.cn

[R30] 函数返回状态码
来源：http://rx.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://dl.lnxyls.cn

[R31] 局部变量
来源：http://tk.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://zv.szsharing.cn

[R32] 参数个数校验
来源：http://kb.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qi.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://td.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cw.huixinmuqiang.cn

[R34] 退出时清理
来源：http://hv.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://no.gzmigu.cn

[R35] 后台执行并等待
来源：http://je.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kv.9csxet.cn

[R36] 并发执行多个任务
来源：http://yo.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ev.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://ck.nicolike.cn

files=$(ls -1)
来源：http://xr.panjiajie.cn

[R38] 管道串联
来源：http://jc.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://fq.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://iq.szsharing.cn

cmd > out.log 2>&1
来源：http://xg.shxzukj.cn

[R40] 追加写日志
来源：http://wl.huixinmuqiang.cn

echo "log" >> out.log
来源：http://aw.huixiangedu.cn

[R41] 丢弃输出
来源：http://dn.asd995.cn

cmd >/dev/null 2>&1
来源：http://sz.huixinmuqiang.cn

[R42] 输入重定向
来源：http://dt.shxzskj.cn

wc -l < a.txt
来源：http://gs.wgjwhj.cn

[R43] 按名字查找文件
来源：http://bh.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://wd.nicolike.cn

[R44] 按修改时间查找
来源：http://jb.haigaiapp.cn

find . -mtime -7 -type f
来源：http://dx.jctech888.com.cn

[R45] 批量删除
来源：http://ru.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://rh.colortex.cn

[R46] 递归替换文件内容
来源：http://fz.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yo.bjjhwx.cn

[R47] sed 单行替换
来源：http://ik.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dh.muxihuayi.cn

[R48] awk 取指定列
来源：http://we.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://tj.hnjuh.cn

[R49] awk 带条件
来源：http://pj.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wd.jctech888.com.cn

[R50] awk 求和
来源：http://uc.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bu.asd995.cn

[R51] 排序去重取前几
来源：http://qd.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bo.bookmarksfly.cn

[R52] 统计行数
来源：http://gf.shxzukj.cn

wc -l a.txt
来源：http://xc.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://fd.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zg.521024.cn

[R54] 比较两个文件
来源：http://gm.hnjuh.cn

diff a.txt b.txt
来源：http://fz.9csxet.cn

[R55] 压缩与解压
来源：http://cx.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sg.wgjwhj.cn

[R56] 远程拷贝
来源：http://xn.colortex.cn

scp file user@host:/path/
来源：http://xt.shxzskj.cn

[R57] 远程执行命令
来源：http://iv.szsharing.cn

ssh user@host 'uptime'
来源：http://ou.bjjhwx.cn

[R58] 下载文件
来源：http://yt.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jq.nszjky.cn

[R59] 发 POST JSON
来源：http://bb.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cm.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://qi.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zb.panjiajie.cn

[R61] 磁盘占用
来源：http://iw.9csxet.cn

df -h;  du -sh *
来源：http://cx.colortex.cn

[R62] 找最占空间的文件
来源：http://sl.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://ju.chemitech.net.cn

[R63] 内存与进程
来源：http://yh.gzmigu.cn


<!-- 参考信息 -->