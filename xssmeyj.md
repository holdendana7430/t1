代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hu.nicolike.cn

[Q05] 重命名列
来源：http://qs.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sj.szsharing.cn

[Q06] 删除列
来源：http://zv.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mp.panjiajie.cn

[Q07] 删除表
来源：http://hc.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://tn.shtwfgs.cn

[Q08] 创建普通索引
来源：http://ck.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ou.newstarts.cn

[Q09] 创建唯一索引
来源：http://ft.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nr.yuexingan06.cn

[Q10] 插入单行
来源：http://pl.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mj.newstarts.cn

[Q11] 一次插入多行
来源：http://ew.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dk.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://vs.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://io.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bn.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://xa.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vu.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://lg.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wq.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dp.9csxet.cn

[Q15] 查询全部
来源：http://yt.jianghongdianzi.cn

SELECT * FROM users;
来源：http://ot.jctech888.com.cn

[Q16] 查询指定列
来源：http://dc.bjjhwx.cn

SELECT id, name FROM users;
来源：http://pc.haigaiapp.cn

[Q17] 条件查询
来源：http://yy.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://un.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://ui.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ls.szxytkj.cn

[Q19] 范围查询
来源：http://cn.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://po.szsharing.cn

[Q20] IN 列表
来源：http://no.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zx.shxzskj.cn

[Q21] 空值判断
来源：http://nw.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tr.hahajie.cn

[Q22] 排序
来源：http://fv.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tf.nicolike.cn

[Q23] 分页
来源：http://kv.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ii.szsharing.cn

[Q24] 去重
来源：http://iq.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://vv.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://wv.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oy.yuntaijiaju.cn

[Q26] 计数
来源：http://wv.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://he.jctech888.com.cn

[Q27] 条件计数
来源：http://ac.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hp.wgjwhj.cn

[Q28] 求和与平均
来源：http://ih.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sv.jctech888.com.cn

[Q29] 最大最小值
来源：http://fn.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jo.hahajie.cn

[Q30] 分组统计
来源：http://sz.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sz.szsharing.cn

[Q31] 分组后过滤
来源：http://ym.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fx.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://ks.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cx.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dm.yuexingan06.cn

[Q33] 多列分组
来源：http://cz.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bo.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://jq.shxzskj.cn

SELECT * FROM (
来源：http://ru.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xx.newstarts.cn

) t WHERE rn = 1;
来源：http://jk.hnjuh.cn

[Q35] 内连接
来源：http://ye.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mr.wgjwhj.cn

[Q36] 左连接
来源：http://mw.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nj.shxzukj.cn

[Q37] 右连接
来源：http://iz.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xa.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bd.shxzukj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xx.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://qz.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ot.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pi.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qa.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iv.nszjky.cn

[Q41] 多表连接
来源：http://hd.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nx.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://yk.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://by.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://xl.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://bp.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://li.asd995.cn

[Q43] 标量子查询
来源：http://pz.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://md.newstarts.cn

[Q44] IN 子查询
来源：http://gy.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nj.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://jh.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vl.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bf.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cg.hahajie.cn

[Q47] 与平均值比较
来源：http://op.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kc.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://nf.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bq.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://mr.lnxyls.cn

[Q49] 更新单行
来源：http://sj.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qi.jianghongdianzi.cn

[Q50] 批量更新
来源：http://ha.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ny.nicolike.cn

[Q51] 用子查询更新
来源：http://me.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://om.asd995.cn

[Q52] 删除指定行
来源：http://iw.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://dy.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://uq.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nb.yuntaijiaju.cn

[Q54] 清空表
来源：http://xx.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://xf.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://ab.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://se.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://op.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gv.huixiangedu.cn

[Q57] 行号
来源：http://eg.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pz.yuntaijiaju.cn

[Q58] 累计求和
来源：http://bt.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jr.panjiajie.cn

[Q59] 分组内累计
来源：http://jv.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qe.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://iw.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sh.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vo.panjiajie.cn

[Q61] 移动平均
来源：http://lz.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://if.jctech888.com.cn

[Q62] 分组占比
来源：http://tq.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fr.chemitech.net.cn

[Q63] 开启事务
来源：http://qs.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oz.wgjwhj.cn

[Q64] 提交事务
来源：http://ta.colortex.cn

COMMIT;
来源：http://kk.haigaiapp.cn

[Q65] 回滚事务
来源：http://eu.colortex.cn

ROLLBACK;
来源：http://vm.bjjhwx.cn

[Q66] 行锁查询
来源：http://yo.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ei.shxzukj.cn

[Q67] 设置隔离级别
来源：http://wt.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://il.szxytkj.cn

[Q68] 保存点
来源：http://fx.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://af.szsharing.cn

ROLLBACK TO sp1;
来源：http://co.haigaiapp.cn

[Q69] 查看执行计划
来源：http://fu.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ki.gzmigu.cn

[Q70] 更新统计信息
来源：http://aj.muxihuayi.cn

ANALYZE TABLE users;
来源：http://kj.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://fr.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fy.huixinmuqiang.cn

[Q72] 查看索引
来源：http://as.gzmigu.cn

SHOW INDEX FROM users;
来源：http://na.shtwfgs.cn

[Q73] 查看表状态
来源：http://ya.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uo.panjiajie.cn

[Q74] 强制使用索引
来源：http://pt.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kx.jctech888.com.cn

[Q75] 日期格式化
来源：http://kf.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uc.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vl.shxzukj.cn

[Q76] 按天统计
来源：http://zc.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://js.huixiangedu.cn

[Q77] 时间加减
来源：http://bw.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lv.9csxet.cn

[Q78] 当前时间
来源：http://df.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lb.colortex.cn

[Q79] 字符串拼接
来源：http://ld.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oi.newstarts.cn

[Q80] 字符串截取
来源：http://dc.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dj.hahajie.cn

[Q81] 字符串替换
来源：http://xw.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jo.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://kw.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dr.szsharing.cn

[Q83] 大小写转换
来源：http://zs.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cd.panjiajie.cn

[Q84] 去除首尾空格
来源：http://tc.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://am.shtwfgs.cn

[Q85] 数值取整
来源：http://oo.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yp.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://ci.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uu.nszjky.cn

[Q87] JSON 字段做条件
来源：http://ma.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ea.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://ji.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yf.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ou.asd995.cn

[Q89] 判断表是否存在
来源：http://oy.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yo.jctech888.com.cn

[Q90] 生成序号列
来源：http://qh.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lh.bookmarksfly.cn

================================================================================
来源：http://rc.bjjhwx.cn

R. Bash 专题
来源：http://hr.asd995.cn

================================================================================
来源：http://qh.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://dt.haigaiapp.cn

#!/usr/bin/env bash
来源：http://xg.panjiajie.cn

set -euo pipefail
来源：http://hu.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://bc.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://qg.yuntaijiaju.cn

[R03] 只读变量
来源：http://nn.shxzskj.cn

readonly PI=3.14
来源：http://sr.shxzskj.cn

[R04] 位置参数
来源：http://oq.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kv.jianghongdianzi.cn

[R05] 参数默认值
来源：http://zk.bjjhwx.cn

name="${1:-default}"
来源：http://sm.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://xi.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lj.shxzskj.cn

[R07] if 判断文件
来源：http://fh.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sx.shxzukj.cn

[R08] 数值比较
来源：http://hz.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uw.muxihuayi.cn

[R09] 字符串比较
来源：http://hf.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cu.panjiajie.cn

[R10] 正则匹配
来源：http://wj.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dz.bookmarksfly.cn

[R11] case 多分支
来源：http://uc.shtwfgs.cn

case "$1" in
来源：http://ew.9csxet.cn

start) echo "启动" ;;
来源：http://pa.9csxet.cn

stop)  echo "停止" ;;
来源：http://fs.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://cx.shxzskj.cn

esac
来源：http://tb.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://ra.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://fc.panjiajie.cn

[R13] for 计数循环
来源：http://jh.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://yr.jianghongdianzi.cn

[R14] C 风格 for
来源：http://rc.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rt.szxytkj.cn

[R15] while 逐行读文件
来源：http://vw.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yx.muxihuayi.cn

[R16] until 等待条件
来源：http://wa.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hh.shtwfgs.cn

[R17] 数组定义与取值
来源：http://wo.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tz.muxihuayi.cn

[R18] 遍历数组
来源：http://jq.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zn.jianghongdianzi.cn

[R19] 数组长度
来源：http://kt.shxzukj.cn

echo "${#arr[@]}"
来源：http://zr.shxzukj.cn

[R20] 关联数组（字典）
来源：http://pb.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lm.huanxung.cn

[R21] 字符串长度
来源：http://dw.newstarts.cn

echo "${#s}"
来源：http://ly.yuexingan06.cn

[R22] 截取子串
来源：http://kz.haigaiapp.cn

echo "${s:0:5}"
来源：http://np.shtwfgs.cn

[R23] 字符串替换
来源：http://rh.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cj.9csxet.cn

[R24] 大小写转换
来源：http://sh.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wd.521024.cn

[R25] 去后缀 / 去前缀
来源：http://ca.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vj.9csxet.cn

[R26] 命令替换
来源：http://to.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://wm.shtwfgs.cn

[R27] 算术展开
来源：http://dl.szsharing.cn

echo $((1 + 2 * 3))
来源：http://se.nszjky.cn

[R28] 浮点运算
来源：http://rn.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://bh.asd995.cn

[R29] 定义函数
来源：http://yb.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://te.huanxung.cn

[R30] 函数返回状态码
来源：http://ny.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://cg.szxytkj.cn

[R31] 局部变量
来源：http://dd.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://ld.haigaiapp.cn

[R32] 参数个数校验
来源：http://ev.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bi.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://dg.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xf.gzmigu.cn

[R34] 退出时清理
来源：http://dd.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yj.szsharing.cn

[R35] 后台执行并等待
来源：http://mt.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lk.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://de.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zu.shxzukj.cn

[R37] 把输出赋给变量
来源：http://hi.hahajie.cn

files=$(ls -1)
来源：http://de.panjiajie.cn

[R38] 管道串联
来源：http://he.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://op.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://ms.shxzukj.cn

cmd > out.log 2>&1
来源：http://nf.shxzskj.cn

[R40] 追加写日志
来源：http://ze.huanxung.cn

echo "log" >> out.log
来源：http://cs.nszjky.cn

[R41] 丢弃输出
来源：http://lk.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://xz.9csxet.cn

[R42] 输入重定向
来源：http://sy.jctech888.com.cn

wc -l < a.txt
来源：http://ds.hahajie.cn

[R43] 按名字查找文件
来源：http://kq.colortex.cn

find . -name "*.log" -type f
来源：http://pi.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://uu.gzmigu.cn

find . -mtime -7 -type f
来源：http://vt.wgjwhj.cn

[R45] 批量删除
来源：http://zy.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://gl.shxzukj.cn

[R46] 递归替换文件内容
来源：http://hc.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dm.huanxung.cn

[R47] sed 单行替换
来源：http://oy.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pf.bookmarksfly.cn

[R48] awk 取指定列
来源：http://gy.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://gh.yuexingan06.cn

[R49] awk 带条件
来源：http://cu.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qq.yuexingan06.cn

[R50] awk 求和
来源：http://jv.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ok.lnxyls.cn

[R51] 排序去重取前几
来源：http://wh.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://um.521024.cn

[R52] 统计行数
来源：http://gj.wgjwhj.cn

wc -l a.txt
来源：http://cw.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://gk.panjiajie.cn


<!-- 参考信息 -->