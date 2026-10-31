代发 wailian999

);
来源：http://ra.shtwfgs.cn

[Q03] 增加列
来源：http://gl.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yl.9csxet.cn

[Q04] 修改列类型
来源：http://ao.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fu.shxzskj.cn

[Q05] 重命名列
来源：http://dw.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jd.asd995.cn

[Q06] 删除列
来源：http://mt.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://am.colortex.cn

[Q07] 删除表
来源：http://mr.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://hv.huixiangedu.cn

[Q08] 创建普通索引
来源：http://ab.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uk.gzmigu.cn

[Q09] 创建唯一索引
来源：http://lx.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gm.gzmigu.cn

[Q10] 插入单行
来源：http://qp.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sf.newstarts.cn

[Q11] 一次插入多行
来源：http://pc.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zr.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://bh.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nm.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mb.nicolike.cn

[Q13] 忽略重复插入
来源：http://zl.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gx.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://xa.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xu.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ra.jianghongdianzi.cn

[Q15] 查询全部
来源：http://pu.wgjwhj.cn

SELECT * FROM users;
来源：http://yo.asd995.cn

[Q16] 查询指定列
来源：http://we.hnjuh.cn

SELECT id, name FROM users;
来源：http://ma.newstarts.cn

[Q17] 条件查询
来源：http://ot.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fa.panjiajie.cn

[Q18] 模糊匹配
来源：http://iu.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bs.hnjuh.cn

[Q19] 范围查询
来源：http://aw.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ea.521024.cn

[Q20] IN 列表
来源：http://qc.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sy.szsharing.cn

[Q21] 空值判断
来源：http://yq.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zu.jianghongdianzi.cn

[Q22] 排序
来源：http://me.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oi.hnjuh.cn

[Q23] 分页
来源：http://sh.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yw.huanxung.cn

[Q24] 去重
来源：http://kx.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://in.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://li.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://da.hahajie.cn

[Q26] 计数
来源：http://sh.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://zj.lnxyls.cn

[Q27] 条件计数
来源：http://ph.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bf.muxihuayi.cn

[Q28] 求和与平均
来源：http://nv.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ex.9csxet.cn

[Q29] 最大最小值
来源：http://ts.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dq.colortex.cn

[Q30] 分组统计
来源：http://ho.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gr.colortex.cn

[Q31] 分组后过滤
来源：http://pv.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nz.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://zx.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qy.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sz.hnjuh.cn

[Q33] 多列分组
来源：http://yc.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ze.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://wk.szsharing.cn

SELECT * FROM (
来源：http://qf.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ks.panjiajie.cn

) t WHERE rn = 1;
来源：http://jw.521024.cn

[Q35] 内连接
来源：http://jk.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kb.asd995.cn

[Q36] 左连接
来源：http://du.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yw.shxzukj.cn

[Q37] 右连接
来源：http://wz.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kj.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yv.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zp.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://yv.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xk.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ot.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xf.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iq.jctech888.com.cn

[Q41] 多表连接
来源：http://zv.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fz.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://ec.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://os.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://so.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://pt.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fr.nicolike.cn

[Q43] 标量子查询
来源：http://xn.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iv.shxzukj.cn

[Q44] IN 子查询
来源：http://dn.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nu.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://rs.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://su.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vb.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pu.szxytkj.cn

[Q47] 与平均值比较
来源：http://iw.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yx.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://jt.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://de.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://go.521024.cn

[Q49] 更新单行
来源：http://yu.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gg.huixinmuqiang.cn

[Q50] 批量更新
来源：http://as.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pf.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://tp.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kq.shxzskj.cn

[Q52] 删除指定行
来源：http://yv.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://ha.haigaiapp.cn

[Q53] 按条件删除
来源：http://jq.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ng.hahajie.cn

[Q54] 清空表
来源：http://ox.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://kt.nicolike.cn

[Q55] 排名（并列占位）
来源：http://fh.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ie.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://ss.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ko.9csxet.cn

[Q57] 行号
来源：http://ch.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aq.panjiajie.cn

[Q58] 累计求和
来源：http://do.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qm.panjiajie.cn

[Q59] 分组内累计
来源：http://ww.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://km.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://qe.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ut.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qo.521024.cn

[Q61] 移动平均
来源：http://fu.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bt.haigaiapp.cn

[Q62] 分组占比
来源：http://zz.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gv.panjiajie.cn

[Q63] 开启事务
来源：http://yq.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cp.huixiangedu.cn

[Q64] 提交事务
来源：http://xh.shtwfgs.cn

COMMIT;
来源：http://db.asd995.cn

[Q65] 回滚事务
来源：http://lh.nicolike.cn

ROLLBACK;
来源：http://xo.jctech888.com.cn

[Q66] 行锁查询
来源：http://ou.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eu.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://uv.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wd.yuexingan06.cn

[Q68] 保存点
来源：http://xi.shxzukj.cn

SAVEPOINT sp1;
来源：http://ql.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://gz.chemitech.net.cn

[Q69] 查看执行计划
来源：http://qx.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ek.9csxet.cn

[Q70] 更新统计信息
来源：http://xu.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://as.huixiangedu.cn

[Q71] 查看建表语句
来源：http://al.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hb.9csxet.cn

[Q72] 查看索引
来源：http://aj.szsharing.cn

SHOW INDEX FROM users;
来源：http://oj.huanxung.cn

[Q73] 查看表状态
来源：http://mo.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ke.jctech888.com.cn

[Q74] 强制使用索引
来源：http://jj.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cu.yuexingan06.cn

[Q75] 日期格式化
来源：http://ef.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fs.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ee.szxytkj.cn

[Q76] 按天统计
来源：http://pp.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nf.lnxyls.cn

[Q77] 时间加减
来源：http://kk.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fc.jianghongdianzi.cn

[Q78] 当前时间
来源：http://lb.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mq.hahajie.cn

[Q79] 字符串拼接
来源：http://gj.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nc.bookmarksfly.cn

[Q80] 字符串截取
来源：http://iu.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zs.bjjhwx.cn

[Q81] 字符串替换
来源：http://zz.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pp.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://gl.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yc.bookmarksfly.cn

[Q83] 大小写转换
来源：http://jh.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pt.lnxyls.cn

[Q84] 去除首尾空格
来源：http://yg.521024.cn

SELECT TRIM(name) FROM users;
来源：http://fu.9csxet.cn

[Q85] 数值取整
来源：http://dr.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wd.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://hm.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://io.nszjky.cn

[Q87] JSON 字段做条件
来源：http://ft.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kz.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://wm.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mg.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bu.lnxyls.cn

[Q89] 判断表是否存在
来源：http://pw.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dw.shxzukj.cn

[Q90] 生成序号列
来源：http://ab.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yb.hahajie.cn

================================================================================
来源：http://ru.gzmigu.cn

R. Bash 专题
来源：http://eu.jctech888.com.cn

================================================================================
来源：http://zn.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://eb.chemitech.net.cn

#!/usr/bin/env bash
来源：http://mf.muxihuayi.cn

set -euo pipefail
来源：http://tw.asd995.cn

[R02] 变量赋值与使用
来源：http://db.521024.cn

name="Tom"; echo "$name"
来源：http://dc.shxzukj.cn

[R03] 只读变量
来源：http://te.haigaiapp.cn

readonly PI=3.14
来源：http://sq.haigaiapp.cn

[R04] 位置参数
来源：http://gc.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tx.huixinmuqiang.cn

[R05] 参数默认值
来源：http://mh.jianghongdianzi.cn

name="${1:-default}"
来源：http://km.shxzskj.cn

[R06] 判断命令是否存在
来源：http://cb.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ac.newstarts.cn

[R07] if 判断文件
来源：http://le.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://au.bookmarksfly.cn

[R08] 数值比较
来源：http://pt.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rr.chemitech.net.cn

[R09] 字符串比较
来源：http://iu.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ff.jianghongdianzi.cn

[R10] 正则匹配
来源：http://kf.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vq.muxihuayi.cn

[R11] case 多分支
来源：http://pw.nicolike.cn

case "$1" in
来源：http://tk.asd995.cn

start) echo "启动" ;;
来源：http://lf.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://xw.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://yz.muxihuayi.cn

esac
来源：http://id.shtwfgs.cn

[R12] for 遍历文件
来源：http://bg.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://ze.yuntaijiaju.cn

[R13] for 计数循环
来源：http://ig.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://mz.szsharing.cn

[R14] C 风格 for
来源：http://oa.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://of.hnjuh.cn

[R15] while 逐行读文件
来源：http://sv.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dr.nicolike.cn

[R16] until 等待条件
来源：http://pe.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eq.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://xq.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sa.9csxet.cn

[R18] 遍历数组
来源：http://zr.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fb.szsharing.cn

[R19] 数组长度
来源：http://uu.yuexingan06.cn

echo "${#arr[@]}"
来源：http://fg.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://nc.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ay.bjjhwx.cn

[R21] 字符串长度
来源：http://qz.haigaiapp.cn

echo "${#s}"
来源：http://hx.hnjuh.cn

[R22] 截取子串
来源：http://yr.gzmigu.cn

echo "${s:0:5}"
来源：http://fl.muxihuayi.cn

[R23] 字符串替换
来源：http://uw.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ff.chemitech.net.cn

[R24] 大小写转换
来源：http://ir.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wo.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://pg.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gi.nicolike.cn

[R26] 命令替换
来源：http://hk.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://xd.huanxung.cn

[R27] 算术展开
来源：http://qp.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://qm.newstarts.cn

[R28] 浮点运算
来源：http://zj.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://nb.huixiangedu.cn

[R29] 定义函数
来源：http://nf.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xv.muxihuayi.cn

[R30] 函数返回状态码
来源：http://fq.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://cj.yuntaijiaju.cn

[R31] 局部变量
来源：http://dz.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://ep.bjjhwx.cn

[R32] 参数个数校验
来源：http://hn.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dt.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://wa.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kl.jctech888.com.cn

[R34] 退出时清理
来源：http://ug.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lf.szxytkj.cn

[R35] 后台执行并等待
来源：http://qs.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fw.colortex.cn

[R36] 并发执行多个任务
来源：http://wb.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gv.hahajie.cn

[R37] 把输出赋给变量
来源：http://cs.szxytkj.cn

files=$(ls -1)
来源：http://tw.wgjwhj.cn

[R38] 管道串联
来源：http://vv.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://qd.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://cx.wgjwhj.cn

cmd > out.log 2>&1
来源：http://vi.colortex.cn

[R40] 追加写日志
来源：http://tl.asd995.cn

echo "log" >> out.log
来源：http://qv.521024.cn

[R41] 丢弃输出
来源：http://vw.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://ns.yuntaijiaju.cn

[R42] 输入重定向
来源：http://lq.gzmigu.cn

wc -l < a.txt
来源：http://qc.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://oh.hnjuh.cn

find . -name "*.log" -type f
来源：http://tw.panjiajie.cn

[R44] 按修改时间查找
来源：http://qw.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://jk.bookmarksfly.cn

[R45] 批量删除
来源：http://kt.huanxung.cn

find . -name "*.tmp" -delete
来源：http://tv.nszjky.cn

[R46] 递归替换文件内容
来源：http://dd.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://py.shtwfgs.cn

[R47] sed 单行替换
来源：http://ys.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qx.chemitech.net.cn

[R48] awk 取指定列
来源：http://wg.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://vd.yuntaijiaju.cn

[R49] awk 带条件
来源：http://qw.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cw.shxzskj.cn

[R50] awk 求和
来源：http://xx.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pe.chemitech.net.cn

[R51] 排序去重取前几
来源：http://cu.9csxet.cn


<!-- 参考信息 -->