代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://gw.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bu.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://az.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zt.521024.cn

[Q14] 存在则更新（upsert）
来源：http://zq.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mp.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cs.wgjwhj.cn

[Q15] 查询全部
来源：http://xn.colortex.cn

SELECT * FROM users;
来源：http://oy.panjiajie.cn

[Q16] 查询指定列
来源：http://ml.szsharing.cn

SELECT id, name FROM users;
来源：http://fl.asd995.cn

[Q17] 条件查询
来源：http://kl.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qr.nszjky.cn

[Q18] 模糊匹配
来源：http://hc.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sx.szsharing.cn

[Q19] 范围查询
来源：http://mu.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zf.yuexingan06.cn

[Q20] IN 列表
来源：http://px.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wu.chemitech.net.cn

[Q21] 空值判断
来源：http://hm.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jg.lnxyls.cn

[Q22] 排序
来源：http://os.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nd.bookmarksfly.cn

[Q23] 分页
来源：http://cp.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jw.lnxyls.cn

[Q24] 去重
来源：http://yy.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://uv.huanxung.cn

[Q25] 只取前 N 条
来源：http://gg.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yh.nicolike.cn

[Q26] 计数
来源：http://vt.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://ph.jianghongdianzi.cn

[Q27] 条件计数
来源：http://hw.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kl.yuexingan06.cn

[Q28] 求和与平均
来源：http://ol.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://if.nszjky.cn

[Q29] 最大最小值
来源：http://yu.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kp.newstarts.cn

[Q30] 分组统计
来源：http://jw.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tb.chemitech.net.cn

[Q31] 分组后过滤
来源：http://qd.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://al.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://vt.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wl.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zx.lnxyls.cn

[Q33] 多列分组
来源：http://ap.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zx.chemitech.net.cn

[Q34] 每组取第一条
来源：http://ji.shxzukj.cn

SELECT * FROM (
来源：http://ns.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fk.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://wt.shxzukj.cn

[Q35] 内连接
来源：http://kh.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wf.nicolike.cn

[Q36] 左连接
来源：http://hn.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jr.shtwfgs.cn

[Q37] 右连接
来源：http://ei.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yt.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://he.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://px.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://ox.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gh.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bu.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cr.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tc.nszjky.cn

[Q41] 多表连接
来源：http://iv.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dx.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://tw.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://xp.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://zp.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://rh.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://du.bjjhwx.cn

[Q43] 标量子查询
来源：http://ij.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oh.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://bx.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qo.colortex.cn

[Q45] EXISTS 判断存在
来源：http://lj.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://io.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sg.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jn.colortex.cn

[Q47] 与平均值比较
来源：http://kx.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qx.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://nd.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fx.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://hs.chemitech.net.cn

[Q49] 更新单行
来源：http://zn.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pm.colortex.cn

[Q50] 批量更新
来源：http://ol.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mq.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://bq.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hd.gzmigu.cn

[Q52] 删除指定行
来源：http://yy.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://hd.9csxet.cn

[Q53] 按条件删除
来源：http://gy.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fv.asd995.cn

[Q54] 清空表
来源：http://cp.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://cp.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://dt.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wo.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://sl.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qp.yuexingan06.cn

[Q57] 行号
来源：http://kn.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aj.bookmarksfly.cn

[Q58] 累计求和
来源：http://yw.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dr.asd995.cn

[Q59] 分组内累计
来源：http://yy.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pq.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://ez.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pw.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vb.9csxet.cn

[Q61] 移动平均
来源：http://pz.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vz.szxytkj.cn

[Q62] 分组占比
来源：http://al.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wy.hahajie.cn

[Q63] 开启事务
来源：http://gn.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://he.nicolike.cn

[Q64] 提交事务
来源：http://jk.yuexingan06.cn

COMMIT;
来源：http://bz.lnxyls.cn

[Q65] 回滚事务
来源：http://ed.asd995.cn

ROLLBACK;
来源：http://uy.bjjhwx.cn

[Q66] 行锁查询
来源：http://gi.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hp.9csxet.cn

[Q67] 设置隔离级别
来源：http://dq.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xy.hahajie.cn

[Q68] 保存点
来源：http://cv.asd995.cn

SAVEPOINT sp1;
来源：http://eq.gzmigu.cn

ROLLBACK TO sp1;
来源：http://jb.chemitech.net.cn

[Q69] 查看执行计划
来源：http://xl.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ri.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://vv.9csxet.cn

ANALYZE TABLE users;
来源：http://gr.asd995.cn

[Q71] 查看建表语句
来源：http://yd.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dq.huanxung.cn

[Q72] 查看索引
来源：http://hs.szsharing.cn

SHOW INDEX FROM users;
来源：http://av.shxzskj.cn

[Q73] 查看表状态
来源：http://dx.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cs.521024.cn

[Q74] 强制使用索引
来源：http://yi.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kp.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://lt.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ga.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://je.jctech888.com.cn

[Q76] 按天统计
来源：http://ff.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ir.huixinmuqiang.cn

[Q77] 时间加减
来源：http://wp.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bd.gzmigu.cn

[Q78] 当前时间
来源：http://ux.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cz.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://hd.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ct.muxihuayi.cn

[Q80] 字符串截取
来源：http://lw.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yv.shtwfgs.cn

[Q81] 字符串替换
来源：http://hb.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xh.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://fh.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://or.newstarts.cn

[Q83] 大小写转换
来源：http://dg.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://id.gzmigu.cn

[Q84] 去除首尾空格
来源：http://ek.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://ul.jctech888.com.cn

[Q85] 数值取整
来源：http://zg.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aw.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://gd.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lr.newstarts.cn

[Q87] JSON 字段做条件
来源：http://bb.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://am.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://zb.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lz.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ba.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://yp.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ot.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://ug.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rq.jianghongdianzi.cn

================================================================================
来源：http://ue.wgjwhj.cn

R. Bash 专题
来源：http://ws.yuexingan06.cn

================================================================================
来源：http://ny.hahajie.cn

[R01] shebang 与严格模式
来源：http://yj.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://fv.9csxet.cn

set -euo pipefail
来源：http://rz.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://oz.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://yt.nicolike.cn

[R03] 只读变量
来源：http://qx.newstarts.cn

readonly PI=3.14
来源：http://jr.jctech888.com.cn

[R04] 位置参数
来源：http://pz.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jy.muxihuayi.cn

[R05] 参数默认值
来源：http://vh.panjiajie.cn

name="${1:-default}"
来源：http://sg.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://ia.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fl.shxzukj.cn

[R07] if 判断文件
来源：http://hp.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sy.newstarts.cn

[R08] 数值比较
来源：http://wh.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ii.yuexingan06.cn

[R09] 字符串比较
来源：http://cr.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hi.nicolike.cn

[R10] 正则匹配
来源：http://zn.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sa.bjjhwx.cn

[R11] case 多分支
来源：http://ij.asd995.cn

case "$1" in
来源：http://cq.hnjuh.cn

start) echo "启动" ;;
来源：http://ug.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://tj.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://jg.hahajie.cn

esac
来源：http://eo.bjjhwx.cn

[R12] for 遍历文件
来源：http://uj.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://or.nszjky.cn

[R13] for 计数循环
来源：http://vj.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://yt.panjiajie.cn

[R14] C 风格 for
来源：http://cs.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yp.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://rf.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cy.asd995.cn

[R16] until 等待条件
来源：http://io.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sa.szsharing.cn

[R17] 数组定义与取值
来源：http://qp.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ka.panjiajie.cn

[R18] 遍历数组
来源：http://cj.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zh.huixinmuqiang.cn

[R19] 数组长度
来源：http://rq.shtwfgs.cn

echo "${#arr[@]}"
来源：http://vx.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://hw.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mf.jctech888.com.cn

[R21] 字符串长度
来源：http://kf.yuexingan06.cn

echo "${#s}"
来源：http://fk.shxzskj.cn

[R22] 截取子串
来源：http://yd.bookmarksfly.cn

echo "${s:0:5}"
来源：http://vc.shxzukj.cn

[R23] 字符串替换
来源：http://nv.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qk.shxzskj.cn

[R24] 大小写转换
来源：http://uk.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xt.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://ao.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fx.newstarts.cn

[R26] 命令替换
来源：http://pq.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://ox.nszjky.cn

[R27] 算术展开
来源：http://cw.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://wu.yuexingan06.cn

[R28] 浮点运算
来源：http://hl.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://mj.muxihuayi.cn

[R29] 定义函数
来源：http://zb.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gy.chemitech.net.cn

[R30] 函数返回状态码
来源：http://gb.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://ge.nszjky.cn

[R31] 局部变量
来源：http://ov.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://jo.newstarts.cn

[R32] 参数个数校验
来源：http://mp.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ix.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://vn.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qs.yuntaijiaju.cn

[R34] 退出时清理
来源：http://dv.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bl.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://yj.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hy.hahajie.cn

[R36] 并发执行多个任务
来源：http://kb.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qt.huanxung.cn

[R37] 把输出赋给变量
来源：http://jq.nicolike.cn

files=$(ls -1)
来源：http://sf.jianghongdianzi.cn

[R38] 管道串联
来源：http://na.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://di.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://bt.szsharing.cn

cmd > out.log 2>&1
来源：http://zx.newstarts.cn

[R40] 追加写日志
来源：http://ou.nicolike.cn

echo "log" >> out.log
来源：http://vm.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://tq.521024.cn

cmd >/dev/null 2>&1
来源：http://pt.chemitech.net.cn

[R42] 输入重定向
来源：http://tr.hnjuh.cn

wc -l < a.txt
来源：http://cu.szxytkj.cn

[R43] 按名字查找文件
来源：http://au.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://me.hahajie.cn

[R44] 按修改时间查找
来源：http://rt.szxytkj.cn

find . -mtime -7 -type f
来源：http://jt.yuntaijiaju.cn

[R45] 批量删除
来源：http://gy.colortex.cn

find . -name "*.tmp" -delete
来源：http://lp.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://ha.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pu.lnxyls.cn

[R47] sed 单行替换
来源：http://so.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zt.lnxyls.cn

[R48] awk 取指定列
来源：http://mb.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://ul.bjjhwx.cn

[R49] awk 带条件
来源：http://ms.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hy.huixiangedu.cn

[R50] awk 求和
来源：http://zn.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ea.chemitech.net.cn

[R51] 排序去重取前几
来源：http://wf.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wm.hahajie.cn

[R52] 统计行数
来源：http://ln.shxzukj.cn

wc -l a.txt
来源：http://ro.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://wx.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qt.nicolike.cn

[R54] 比较两个文件
来源：http://dr.nicolike.cn

diff a.txt b.txt
来源：http://pg.shtwfgs.cn

[R55] 压缩与解压
来源：http://jt.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fc.haigaiapp.cn

[R56] 远程拷贝
来源：http://uy.jianghongdianzi.cn

scp file user@host:/path/
来源：http://pz.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://qi.yuexingan06.cn

ssh user@host 'uptime'
来源：http://wr.huixinmuqiang.cn

[R58] 下载文件
来源：http://cn.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bs.yuexingan06.cn

[R59] 发 POST JSON
来源：http://ew.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yx.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://uw.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bk.yuexingan06.cn

[R61] 磁盘占用
来源：http://vz.huixiangedu.cn


<!-- 参考信息 -->