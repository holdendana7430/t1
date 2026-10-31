代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://iu.jianghongdianzi.cn

[Q07] 删除表
来源：http://nh.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://xl.haigaiapp.cn

[Q08] 创建普通索引
来源：http://qp.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://da.521024.cn

[Q09] 创建唯一索引
来源：http://dy.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pu.haigaiapp.cn

[Q10] 插入单行
来源：http://lx.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ze.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://on.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ts.colortex.cn

[Q12] 插入后取自增 ID
来源：http://cx.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ib.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ld.panjiajie.cn

[Q13] 忽略重复插入
来源：http://nl.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ea.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://dd.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dp.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bd.szsharing.cn

[Q15] 查询全部
来源：http://xa.newstarts.cn

SELECT * FROM users;
来源：http://hu.szsharing.cn

[Q16] 查询指定列
来源：http://vl.shxzukj.cn

SELECT id, name FROM users;
来源：http://eq.chemitech.net.cn

[Q17] 条件查询
来源：http://wj.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zg.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://xm.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yz.nszjky.cn

[Q19] 范围查询
来源：http://kk.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fy.muxihuayi.cn

[Q20] IN 列表
来源：http://tf.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gs.szsharing.cn

[Q21] 空值判断
来源：http://iy.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yd.wgjwhj.cn

[Q22] 排序
来源：http://qk.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ss.shxzukj.cn

[Q23] 分页
来源：http://ho.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ak.yuexingan06.cn

[Q24] 去重
来源：http://qs.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://rn.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://sk.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xz.lnxyls.cn

[Q26] 计数
来源：http://zt.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://zk.shxzskj.cn

[Q27] 条件计数
来源：http://sm.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://by.bjjhwx.cn

[Q28] 求和与平均
来源：http://fo.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ux.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://ju.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zx.bjjhwx.cn

[Q30] 分组统计
来源：http://rq.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://id.szxytkj.cn

[Q31] 分组后过滤
来源：http://iw.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vu.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://yi.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ca.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yn.newstarts.cn

[Q33] 多列分组
来源：http://qf.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wn.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://cs.shtwfgs.cn

SELECT * FROM (
来源：http://tz.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iu.panjiajie.cn

) t WHERE rn = 1;
来源：http://ue.asd995.cn

[Q35] 内连接
来源：http://uy.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ar.gzmigu.cn

[Q36] 左连接
来源：http://ds.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yp.bjjhwx.cn

[Q37] 右连接
来源：http://pk.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wq.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fq.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://do.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://li.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tk.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fy.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tk.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tu.huixiangedu.cn

[Q41] 多表连接
来源：http://ef.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nr.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://ie.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ku.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://nr.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://oe.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ar.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://zr.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ay.hnjuh.cn

[Q44] IN 子查询
来源：http://pk.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://np.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://ui.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wu.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xc.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gr.gzmigu.cn

[Q47] 与平均值比较
来源：http://da.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dy.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://tc.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rm.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://uo.szxytkj.cn

[Q49] 更新单行
来源：http://qw.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ij.wgjwhj.cn

[Q50] 批量更新
来源：http://tc.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lh.shxzskj.cn

[Q51] 用子查询更新
来源：http://cf.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qm.huanxung.cn

[Q52] 删除指定行
来源：http://hl.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://cv.asd995.cn

[Q53] 按条件删除
来源：http://gs.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eq.9csxet.cn

[Q54] 清空表
来源：http://an.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://iz.asd995.cn

[Q55] 排名（并列占位）
来源：http://sk.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://on.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://mr.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://em.yuntaijiaju.cn

[Q57] 行号
来源：http://xx.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xv.521024.cn

[Q58] 累计求和
来源：http://lc.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ft.chemitech.net.cn

[Q59] 分组内累计
来源：http://tq.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ch.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://kd.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://do.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://po.chemitech.net.cn

[Q61] 移动平均
来源：http://gu.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lc.colortex.cn

[Q62] 分组占比
来源：http://dc.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hp.bookmarksfly.cn

[Q63] 开启事务
来源：http://au.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ee.shtwfgs.cn

[Q64] 提交事务
来源：http://gn.newstarts.cn

COMMIT;
来源：http://ef.shxzukj.cn

[Q65] 回滚事务
来源：http://xl.huixinmuqiang.cn

ROLLBACK;
来源：http://mv.huanxung.cn

[Q66] 行锁查询
来源：http://pf.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jb.nicolike.cn

[Q67] 设置隔离级别
来源：http://xq.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uv.nicolike.cn

[Q68] 保存点
来源：http://ra.huanxung.cn

SAVEPOINT sp1;
来源：http://wu.nszjky.cn

ROLLBACK TO sp1;
来源：http://qi.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://vb.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sr.hahajie.cn

[Q70] 更新统计信息
来源：http://fz.9csxet.cn

ANALYZE TABLE users;
来源：http://ca.bjjhwx.cn

[Q71] 查看建表语句
来源：http://xq.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tb.hahajie.cn

[Q72] 查看索引
来源：http://fa.nszjky.cn

SHOW INDEX FROM users;
来源：http://vz.bjjhwx.cn

[Q73] 查看表状态
来源：http://xd.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://us.asd995.cn

[Q74] 强制使用索引
来源：http://zq.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tn.newstarts.cn

[Q75] 日期格式化
来源：http://lk.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fs.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kt.gzmigu.cn

[Q76] 按天统计
来源：http://rp.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gu.szxytkj.cn

[Q77] 时间加减
来源：http://rw.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cv.shtwfgs.cn

[Q78] 当前时间
来源：http://wo.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vf.huixiangedu.cn

[Q79] 字符串拼接
来源：http://ne.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aq.nszjky.cn

[Q80] 字符串截取
来源：http://og.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bw.shtwfgs.cn

[Q81] 字符串替换
来源：http://vd.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pw.colortex.cn

[Q82] 字符长度与字节长度
来源：http://cn.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://au.panjiajie.cn

[Q83] 大小写转换
来源：http://wd.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xr.shxzskj.cn

[Q84] 去除首尾空格
来源：http://dt.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://gu.panjiajie.cn

[Q85] 数值取整
来源：http://pq.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ah.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://la.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ts.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://yi.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ff.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://hg.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oj.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ip.newstarts.cn

[Q89] 判断表是否存在
来源：http://zk.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ld.shtwfgs.cn

[Q90] 生成序号列
来源：http://in.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gu.szxytkj.cn

================================================================================
来源：http://eg.yuexingan06.cn

R. Bash 专题
来源：http://hs.lnxyls.cn

================================================================================
来源：http://gs.huanxung.cn

[R01] shebang 与严格模式
来源：http://xy.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://ar.bjjhwx.cn

set -euo pipefail
来源：http://we.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://ss.lnxyls.cn

name="Tom"; echo "$name"
来源：http://ry.gzmigu.cn

[R03] 只读变量
来源：http://js.muxihuayi.cn

readonly PI=3.14
来源：http://ty.jctech888.com.cn

[R04] 位置参数
来源：http://cn.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pr.panjiajie.cn

[R05] 参数默认值
来源：http://rs.muxihuayi.cn

name="${1:-default}"
来源：http://hp.nicolike.cn

[R06] 判断命令是否存在
来源：http://yz.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bi.yuntaijiaju.cn

[R07] if 判断文件
来源：http://dn.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wb.szxytkj.cn

[R08] 数值比较
来源：http://sc.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://us.bookmarksfly.cn

[R09] 字符串比较
来源：http://tp.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://op.jctech888.com.cn

[R10] 正则匹配
来源：http://ff.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ha.bookmarksfly.cn

[R11] case 多分支
来源：http://gy.haigaiapp.cn

case "$1" in
来源：http://ut.szxytkj.cn

start) echo "启动" ;;
来源：http://jr.colortex.cn

stop)  echo "停止" ;;
来源：http://zv.hahajie.cn

*)     echo "未知命令" ;;
来源：http://lp.panjiajie.cn

esac
来源：http://td.lnxyls.cn

[R12] for 遍历文件
来源：http://gr.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://jf.lnxyls.cn

[R13] for 计数循环
来源：http://sv.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://zy.panjiajie.cn

[R14] C 风格 for
来源：http://jg.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ic.szxytkj.cn

[R15] while 逐行读文件
来源：http://gu.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sj.huixiangedu.cn

[R16] until 等待条件
来源：http://dg.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vj.wgjwhj.cn

[R17] 数组定义与取值
来源：http://fj.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aj.wgjwhj.cn

[R18] 遍历数组
来源：http://vn.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rm.hahajie.cn

[R19] 数组长度
来源：http://oc.szxytkj.cn

echo "${#arr[@]}"
来源：http://nm.nicolike.cn

[R20] 关联数组（字典）
来源：http://yc.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yi.newstarts.cn

[R21] 字符串长度
来源：http://tw.haigaiapp.cn

echo "${#s}"
来源：http://qo.newstarts.cn

[R22] 截取子串
来源：http://ss.yuexingan06.cn

echo "${s:0:5}"
来源：http://rn.lnxyls.cn

[R23] 字符串替换
来源：http://dq.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bp.bjjhwx.cn

[R24] 大小写转换
来源：http://db.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ky.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://kg.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://by.shxzskj.cn

[R26] 命令替换
来源：http://gs.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://vp.chemitech.net.cn

[R27] 算术展开
来源：http://ac.9csxet.cn

echo $((1 + 2 * 3))
来源：http://nf.colortex.cn

[R28] 浮点运算
来源：http://lz.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://ml.yuntaijiaju.cn

[R29] 定义函数
来源：http://fe.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yv.yuexingan06.cn

[R30] 函数返回状态码
来源：http://ok.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://yy.newstarts.cn

[R31] 局部变量
来源：http://ol.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://rd.shxzukj.cn

[R32] 参数个数校验
来源：http://px.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vr.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://ia.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gm.nicolike.cn

[R34] 退出时清理
来源：http://wz.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pc.haigaiapp.cn

[R35] 后台执行并等待
来源：http://en.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yv.shxzukj.cn

[R36] 并发执行多个任务
来源：http://wd.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qh.panjiajie.cn

[R37] 把输出赋给变量
来源：http://uo.jctech888.com.cn

files=$(ls -1)
来源：http://ik.asd995.cn

[R38] 管道串联
来源：http://dr.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://sb.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://zv.haigaiapp.cn

cmd > out.log 2>&1
来源：http://wu.shxzskj.cn

[R40] 追加写日志
来源：http://bk.lnxyls.cn

echo "log" >> out.log
来源：http://tg.colortex.cn

[R41] 丢弃输出
来源：http://wc.nszjky.cn

cmd >/dev/null 2>&1
来源：http://jk.haigaiapp.cn

[R42] 输入重定向
来源：http://ed.9csxet.cn

wc -l < a.txt
来源：http://yf.wgjwhj.cn

[R43] 按名字查找文件
来源：http://ci.haigaiapp.cn

find . -name "*.log" -type f
来源：http://dv.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://ip.szsharing.cn

find . -mtime -7 -type f
来源：http://yb.shtwfgs.cn

[R45] 批量删除
来源：http://aj.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://ek.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://yx.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uu.szxytkj.cn

[R47] sed 单行替换
来源：http://if.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vl.shtwfgs.cn

[R48] awk 取指定列
来源：http://pa.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://uv.shxzukj.cn

[R49] awk 带条件
来源：http://wr.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kb.jctech888.com.cn

[R50] awk 求和
来源：http://rd.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uw.hahajie.cn

[R51] 排序去重取前几
来源：http://ut.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kv.hahajie.cn

[R52] 统计行数
来源：http://km.lnxyls.cn

wc -l a.txt
来源：http://jg.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://je.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gc.huanxung.cn

[R54] 比较两个文件
来源：http://pu.shxzukj.cn

diff a.txt b.txt
来源：http://bh.panjiajie.cn

[R55] 压缩与解压
来源：http://rx.lnxyls.cn


<!-- 参考信息 -->