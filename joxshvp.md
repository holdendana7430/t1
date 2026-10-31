代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://hi.wgjwhj.cn

[Q07] 删除表
来源：http://et.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://br.chemitech.net.cn

[Q08] 创建普通索引
来源：http://yx.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kj.521024.cn

[Q09] 创建唯一索引
来源：http://el.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jx.nicolike.cn

[Q10] 插入单行
来源：http://la.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rt.hahajie.cn

[Q11] 一次插入多行
来源：http://vb.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hv.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://ca.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pl.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://je.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://tw.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gi.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://et.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nz.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ci.shxzskj.cn

[Q15] 查询全部
来源：http://hx.muxihuayi.cn

SELECT * FROM users;
来源：http://he.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://av.shtwfgs.cn

SELECT id, name FROM users;
来源：http://rw.shxzskj.cn

[Q17] 条件查询
来源：http://hi.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gg.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://sw.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qg.colortex.cn

[Q19] 范围查询
来源：http://pf.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dd.hnjuh.cn

[Q20] IN 列表
来源：http://nh.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ce.9csxet.cn

[Q21] 空值判断
来源：http://jx.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ls.bookmarksfly.cn

[Q22] 排序
来源：http://au.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ir.9csxet.cn

[Q23] 分页
来源：http://yv.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ax.huanxung.cn

[Q24] 去重
来源：http://hl.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://xs.gzmigu.cn

[Q25] 只取前 N 条
来源：http://dp.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mp.jctech888.com.cn

[Q26] 计数
来源：http://qn.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://qh.bookmarksfly.cn

[Q27] 条件计数
来源：http://sg.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gj.haigaiapp.cn

[Q28] 求和与平均
来源：http://sw.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wi.9csxet.cn

[Q29] 最大最小值
来源：http://jg.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hk.colortex.cn

[Q30] 分组统计
来源：http://ta.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qd.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://sv.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nm.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://pv.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://le.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pp.hnjuh.cn

[Q33] 多列分组
来源：http://kv.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cx.muxihuayi.cn

[Q34] 每组取第一条
来源：http://lm.bjjhwx.cn

SELECT * FROM (
来源：http://ix.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wj.huixiangedu.cn

) t WHERE rn = 1;
来源：http://km.gzmigu.cn

[Q35] 内连接
来源：http://nv.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://st.shxzukj.cn

[Q36] 左连接
来源：http://ru.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dw.chemitech.net.cn

[Q37] 右连接
来源：http://gq.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://or.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bo.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ve.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://mq.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dr.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cd.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pl.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zl.9csxet.cn

[Q41] 多表连接
来源：http://qz.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ap.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://cj.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://vc.521024.cn

[Q42] 连接条件附加过滤
来源：http://jk.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://oc.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ta.haigaiapp.cn

[Q43] 标量子查询
来源：http://nt.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dj.wgjwhj.cn

[Q44] IN 子查询
来源：http://xa.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://to.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://wy.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fe.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wj.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://is.yuexingan06.cn

[Q47] 与平均值比较
来源：http://qm.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uk.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://fz.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://df.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://vi.szsharing.cn

[Q49] 更新单行
来源：http://jl.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ni.521024.cn

[Q50] 批量更新
来源：http://nr.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dm.haigaiapp.cn

[Q51] 用子查询更新
来源：http://ge.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bs.bjjhwx.cn

[Q52] 删除指定行
来源：http://xd.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://vj.asd995.cn

[Q53] 按条件删除
来源：http://ff.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fd.shxzukj.cn

[Q54] 清空表
来源：http://kx.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://bo.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://hg.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ln.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://pn.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ea.asd995.cn

[Q57] 行号
来源：http://vq.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uv.szsharing.cn

[Q58] 累计求和
来源：http://li.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tz.shxzukj.cn

[Q59] 分组内累计
来源：http://yw.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xh.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://uv.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ev.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pr.nszjky.cn

[Q61] 移动平均
来源：http://vt.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xi.yuexingan06.cn

[Q62] 分组占比
来源：http://op.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kd.nicolike.cn

[Q63] 开启事务
来源：http://ni.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qv.huixiangedu.cn

[Q64] 提交事务
来源：http://ts.gzmigu.cn

COMMIT;
来源：http://fq.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://iq.wgjwhj.cn

ROLLBACK;
来源：http://tn.huanxung.cn

[Q66] 行锁查询
来源：http://xu.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bq.lnxyls.cn

[Q67] 设置隔离级别
来源：http://ri.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://re.hnjuh.cn

[Q68] 保存点
来源：http://lc.nszjky.cn

SAVEPOINT sp1;
来源：http://yv.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://xx.szsharing.cn

[Q69] 查看执行计划
来源：http://in.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qk.wgjwhj.cn

[Q70] 更新统计信息
来源：http://dx.colortex.cn

ANALYZE TABLE users;
来源：http://vc.wgjwhj.cn

[Q71] 查看建表语句
来源：http://mp.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://li.asd995.cn

[Q72] 查看索引
来源：http://qc.gzmigu.cn

SHOW INDEX FROM users;
来源：http://or.huanxung.cn

[Q73] 查看表状态
来源：http://ln.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qq.shxzskj.cn

[Q74] 强制使用索引
来源：http://zf.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pq.newstarts.cn

[Q75] 日期格式化
来源：http://om.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ov.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zg.hnjuh.cn

[Q76] 按天统计
来源：http://cq.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://il.nszjky.cn

[Q77] 时间加减
来源：http://cx.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://re.nszjky.cn

[Q78] 当前时间
来源：http://lr.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qb.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://zj.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yb.haigaiapp.cn

[Q80] 字符串截取
来源：http://hs.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://de.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://cm.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sy.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://lt.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uv.hnjuh.cn

[Q83] 大小写转换
来源：http://lv.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ai.huanxung.cn

[Q84] 去除首尾空格
来源：http://wc.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://ia.huixiangedu.cn

[Q85] 数值取整
来源：http://xn.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wi.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://sj.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dl.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://rv.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mx.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://zx.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nm.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ie.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://ux.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wn.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://bh.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ih.panjiajie.cn

================================================================================
来源：http://ei.jianghongdianzi.cn

R. Bash 专题
来源：http://um.gzmigu.cn

================================================================================
来源：http://rh.hahajie.cn

[R01] shebang 与严格模式
来源：http://cv.newstarts.cn

#!/usr/bin/env bash
来源：http://af.hahajie.cn

set -euo pipefail
来源：http://ba.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://pg.9csxet.cn

name="Tom"; echo "$name"
来源：http://ht.chemitech.net.cn

[R03] 只读变量
来源：http://me.colortex.cn

readonly PI=3.14
来源：http://jp.9csxet.cn

[R04] 位置参数
来源：http://py.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oy.gzmigu.cn

[R05] 参数默认值
来源：http://pf.bjjhwx.cn

name="${1:-default}"
来源：http://qf.szsharing.cn

[R06] 判断命令是否存在
来源：http://yf.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wt.szsharing.cn

[R07] if 判断文件
来源：http://gn.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qq.haigaiapp.cn

[R08] 数值比较
来源：http://bz.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wl.gzmigu.cn

[R09] 字符串比较
来源：http://fq.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ip.nszjky.cn

[R10] 正则匹配
来源：http://ux.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rj.wgjwhj.cn

[R11] case 多分支
来源：http://vx.chemitech.net.cn

case "$1" in
来源：http://iw.shtwfgs.cn

start) echo "启动" ;;
来源：http://ir.shxzukj.cn

stop)  echo "停止" ;;
来源：http://lq.huanxung.cn

*)     echo "未知命令" ;;
来源：http://qn.bookmarksfly.cn

esac
来源：http://el.colortex.cn

[R12] for 遍历文件
来源：http://rk.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://ax.nicolike.cn

[R13] for 计数循环
来源：http://xc.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://hf.newstarts.cn

[R14] C 风格 for
来源：http://mq.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://om.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://wh.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jo.bjjhwx.cn

[R16] until 等待条件
来源：http://hc.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ve.shtwfgs.cn

[R17] 数组定义与取值
来源：http://og.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oe.hnjuh.cn

[R18] 遍历数组
来源：http://ye.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fs.521024.cn

[R19] 数组长度
来源：http://ez.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://wy.521024.cn

[R20] 关联数组（字典）
来源：http://qv.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cc.shxzukj.cn

[R21] 字符串长度
来源：http://zn.asd995.cn

echo "${#s}"
来源：http://zw.shxzskj.cn

[R22] 截取子串
来源：http://yh.nszjky.cn

echo "${s:0:5}"
来源：http://dh.muxihuayi.cn

[R23] 字符串替换
来源：http://jm.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gz.yuexingan06.cn

[R24] 大小写转换
来源：http://im.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tw.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://aw.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://aw.jctech888.com.cn

[R26] 命令替换
来源：http://tr.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://ib.yuexingan06.cn

[R27] 算术展开
来源：http://mg.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://re.jctech888.com.cn

[R28] 浮点运算
来源：http://ro.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://el.lnxyls.cn

[R29] 定义函数
来源：http://dl.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nk.hnjuh.cn

[R30] 函数返回状态码
来源：http://tg.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://ar.gzmigu.cn

[R31] 局部变量
来源：http://dm.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://ot.nicolike.cn

[R32] 参数个数校验
来源：http://cz.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yf.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://fo.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sm.shxzskj.cn

[R34] 退出时清理
来源：http://fd.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xh.521024.cn

[R35] 后台执行并等待
来源：http://fi.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xm.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://oz.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ty.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://sf.shxzukj.cn

files=$(ls -1)
来源：http://by.bjjhwx.cn

[R38] 管道串联
来源：http://gd.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://pb.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://mn.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://vm.shxzukj.cn

[R40] 追加写日志
来源：http://xs.yuexingan06.cn

echo "log" >> out.log
来源：http://ki.shxzukj.cn

[R41] 丢弃输出
来源：http://ng.colortex.cn

cmd >/dev/null 2>&1
来源：http://bk.bookmarksfly.cn

[R42] 输入重定向
来源：http://ko.9csxet.cn

wc -l < a.txt
来源：http://ox.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://ic.asd995.cn

find . -name "*.log" -type f
来源：http://ha.wgjwhj.cn

[R44] 按修改时间查找
来源：http://lk.panjiajie.cn

find . -mtime -7 -type f
来源：http://aa.hnjuh.cn

[R45] 批量删除
来源：http://cc.521024.cn

find . -name "*.tmp" -delete
来源：http://ii.panjiajie.cn

[R46] 递归替换文件内容
来源：http://rk.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tc.szsharing.cn

[R47] sed 单行替换
来源：http://bw.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ha.hahajie.cn

[R48] awk 取指定列
来源：http://wv.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://gv.shtwfgs.cn

[R49] awk 带条件
来源：http://up.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ws.panjiajie.cn

[R50] awk 求和
来源：http://sd.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aj.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://uz.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ma.521024.cn

[R52] 统计行数
来源：http://bn.9csxet.cn

wc -l a.txt
来源：http://vf.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://sc.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://se.haigaiapp.cn

[R54] 比较两个文件
来源：http://iv.nszjky.cn

diff a.txt b.txt
来源：http://hu.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://zn.huanxung.cn


<!-- 参考信息 -->