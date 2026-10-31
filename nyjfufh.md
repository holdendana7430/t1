代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dz.haigaiapp.cn

user_id INT NOT NULL,
来源：http://ke.9csxet.cn

amount DECIMAL(10, 2),
来源：http://hr.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rm.gzmigu.cn

);
来源：http://os.lnxyls.cn

[Q03] 增加列
来源：http://lm.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sy.panjiajie.cn

[Q04] 修改列类型
来源：http://hv.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ww.huixinmuqiang.cn

[Q05] 重命名列
来源：http://de.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gq.jctech888.com.cn

[Q06] 删除列
来源：http://sv.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gq.shtwfgs.cn

[Q07] 删除表
来源：http://hh.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://cd.9csxet.cn

[Q08] 创建普通索引
来源：http://bc.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fl.hahajie.cn

[Q09] 创建唯一索引
来源：http://zi.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qs.wgjwhj.cn

[Q10] 插入单行
来源：http://jr.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dz.szsharing.cn

[Q11] 一次插入多行
来源：http://ll.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tg.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://yu.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dd.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://co.shxzukj.cn

[Q13] 忽略重复插入
来源：http://fp.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nd.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://bi.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ys.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rq.nszjky.cn

[Q15] 查询全部
来源：http://zd.asd995.cn

SELECT * FROM users;
来源：http://db.szxytkj.cn

[Q16] 查询指定列
来源：http://lm.szsharing.cn

SELECT id, name FROM users;
来源：http://df.nicolike.cn

[Q17] 条件查询
来源：http://bg.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sy.muxihuayi.cn

[Q18] 模糊匹配
来源：http://rr.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mq.bookmarksfly.cn

[Q19] 范围查询
来源：http://ir.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fi.chemitech.net.cn

[Q20] IN 列表
来源：http://ea.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sl.yuntaijiaju.cn

[Q21] 空值判断
来源：http://gw.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zn.huanxung.cn

[Q22] 排序
来源：http://dc.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cj.shxzskj.cn

[Q23] 分页
来源：http://so.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qa.bjjhwx.cn

[Q24] 去重
来源：http://cl.521024.cn

SELECT DISTINCT city FROM users;
来源：http://sx.521024.cn

[Q25] 只取前 N 条
来源：http://dk.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wb.chemitech.net.cn

[Q26] 计数
来源：http://rj.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://kh.bjjhwx.cn

[Q27] 条件计数
来源：http://tw.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kl.haigaiapp.cn

[Q28] 求和与平均
来源：http://pg.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uw.9csxet.cn

[Q29] 最大最小值
来源：http://wz.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ju.asd995.cn

[Q30] 分组统计
来源：http://lx.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://di.521024.cn

[Q31] 分组后过滤
来源：http://vt.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ir.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://uv.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wt.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://an.lnxyls.cn

[Q33] 多列分组
来源：http://wu.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hx.jctech888.com.cn

[Q34] 每组取第一条
来源：http://xo.asd995.cn

SELECT * FROM (
来源：http://fm.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://au.hnjuh.cn

) t WHERE rn = 1;
来源：http://cq.521024.cn

[Q35] 内连接
来源：http://gb.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://df.yuexingan06.cn

[Q36] 左连接
来源：http://yo.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://as.asd995.cn

[Q37] 右连接
来源：http://zm.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kw.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ug.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tp.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://fc.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mx.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wm.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sn.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ys.yuexingan06.cn

[Q41] 多表连接
来源：http://bx.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ii.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://yv.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://qb.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://qc.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://vm.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ho.huixiangedu.cn

[Q43] 标量子查询
来源：http://fy.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://br.shtwfgs.cn

[Q44] IN 子查询
来源：http://ss.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fy.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://jd.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ux.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pe.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wz.shtwfgs.cn

[Q47] 与平均值比较
来源：http://kw.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jt.asd995.cn

[Q48] CTE 公用表表达式
来源：http://wt.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://io.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://za.gzmigu.cn

[Q49] 更新单行
来源：http://ca.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://po.521024.cn

[Q50] 批量更新
来源：http://oj.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ej.haigaiapp.cn

[Q51] 用子查询更新
来源：http://no.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wg.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://if.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://be.hnjuh.cn

[Q53] 按条件删除
来源：http://mb.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zt.shxzukj.cn

[Q54] 清空表
来源：http://wj.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://ji.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://mv.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hw.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://bo.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wd.bookmarksfly.cn

[Q57] 行号
来源：http://iy.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xs.jctech888.com.cn

[Q58] 累计求和
来源：http://qn.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ct.bjjhwx.cn

[Q59] 分组内累计
来源：http://rg.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wf.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://jp.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yj.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rg.hnjuh.cn

[Q61] 移动平均
来源：http://wj.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vz.jctech888.com.cn

[Q62] 分组占比
来源：http://yz.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mz.jctech888.com.cn

[Q63] 开启事务
来源：http://hh.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nj.huixiangedu.cn

[Q64] 提交事务
来源：http://jy.gzmigu.cn

COMMIT;
来源：http://zk.newstarts.cn

[Q65] 回滚事务
来源：http://px.nicolike.cn

ROLLBACK;
来源：http://nc.yuexingan06.cn

[Q66] 行锁查询
来源：http://tl.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://td.hnjuh.cn

[Q67] 设置隔离级别
来源：http://ua.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gf.wgjwhj.cn

[Q68] 保存点
来源：http://xn.huanxung.cn

SAVEPOINT sp1;
来源：http://vd.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://gw.shxzukj.cn

[Q69] 查看执行计划
来源：http://ni.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ze.chemitech.net.cn

[Q70] 更新统计信息
来源：http://yb.521024.cn

ANALYZE TABLE users;
来源：http://hy.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://el.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://or.bookmarksfly.cn

[Q72] 查看索引
来源：http://ob.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://rc.hahajie.cn

[Q73] 查看表状态
来源：http://sa.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zg.panjiajie.cn

[Q74] 强制使用索引
来源：http://rl.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tn.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://no.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ay.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://no.yuntaijiaju.cn

[Q76] 按天统计
来源：http://gl.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jk.szxytkj.cn

[Q77] 时间加减
来源：http://bd.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ds.shxzskj.cn

[Q78] 当前时间
来源：http://je.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://po.gzmigu.cn

[Q79] 字符串拼接
来源：http://bg.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zx.panjiajie.cn

[Q80] 字符串截取
来源：http://zn.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zx.asd995.cn

[Q81] 字符串替换
来源：http://uf.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ch.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://ja.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kq.9csxet.cn

[Q83] 大小写转换
来源：http://ke.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lb.hahajie.cn

[Q84] 去除首尾空格
来源：http://ut.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://xj.shxzukj.cn

[Q85] 数值取整
来源：http://vc.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jn.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://zi.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uw.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://tj.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nm.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://sw.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qk.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ds.hahajie.cn

[Q89] 判断表是否存在
来源：http://ba.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vo.huixiangedu.cn

[Q90] 生成序号列
来源：http://js.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ef.huixinmuqiang.cn

================================================================================
来源：http://wc.jianghongdianzi.cn

R. Bash 专题
来源：http://rm.hahajie.cn

================================================================================
来源：http://fm.szsharing.cn

[R01] shebang 与严格模式
来源：http://ne.nicolike.cn

#!/usr/bin/env bash
来源：http://gu.yuntaijiaju.cn

set -euo pipefail
来源：http://dw.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://mp.shxzukj.cn

name="Tom"; echo "$name"
来源：http://gj.huixinmuqiang.cn

[R03] 只读变量
来源：http://pk.hahajie.cn

readonly PI=3.14
来源：http://sc.asd995.cn

[R04] 位置参数
来源：http://bz.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oc.nicolike.cn

[R05] 参数默认值
来源：http://xl.nszjky.cn

name="${1:-default}"
来源：http://ib.newstarts.cn

[R06] 判断命令是否存在
来源：http://xe.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fm.muxihuayi.cn

[R07] if 判断文件
来源：http://gs.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qn.shxzskj.cn

[R08] 数值比较
来源：http://bi.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ps.wgjwhj.cn

[R09] 字符串比较
来源：http://tl.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ie.hnjuh.cn

[R10] 正则匹配
来源：http://io.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jk.yuntaijiaju.cn

[R11] case 多分支
来源：http://du.shxzskj.cn

case "$1" in
来源：http://sd.haigaiapp.cn

start) echo "启动" ;;
来源：http://ue.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://dx.hahajie.cn

*)     echo "未知命令" ;;
来源：http://su.gzmigu.cn

esac
来源：http://yw.bookmarksfly.cn

[R12] for 遍历文件
来源：http://ei.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://ff.huixinmuqiang.cn

[R13] for 计数循环
来源：http://jp.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://bc.yuexingan06.cn

[R14] C 风格 for
来源：http://et.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ob.huanxung.cn

[R15] while 逐行读文件
来源：http://ho.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ot.gzmigu.cn

[R16] until 等待条件
来源：http://ju.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qc.colortex.cn

[R17] 数组定义与取值
来源：http://kh.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kd.shtwfgs.cn

[R18] 遍历数组
来源：http://vb.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vb.shxzukj.cn

[R19] 数组长度
来源：http://ne.hnjuh.cn

echo "${#arr[@]}"
来源：http://po.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://nu.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ig.521024.cn

[R21] 字符串长度
来源：http://cv.yuntaijiaju.cn

echo "${#s}"
来源：http://ht.shxzukj.cn

[R22] 截取子串
来源：http://aa.newstarts.cn

echo "${s:0:5}"
来源：http://et.asd995.cn

[R23] 字符串替换
来源：http://wc.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ni.jctech888.com.cn

[R24] 大小写转换
来源：http://iv.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ew.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://cr.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bh.yuntaijiaju.cn

[R26] 命令替换
来源：http://ng.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://sv.nszjky.cn

[R27] 算术展开
来源：http://mq.hahajie.cn

echo $((1 + 2 * 3))
来源：http://iw.chemitech.net.cn

[R28] 浮点运算
来源：http://uj.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://ru.shtwfgs.cn

[R29] 定义函数
来源：http://zw.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ez.huanxung.cn

[R30] 函数返回状态码
来源：http://di.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://da.nszjky.cn

[R31] 局部变量
来源：http://tv.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://uc.colortex.cn

[R32] 参数个数校验
来源：http://uz.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kv.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://ki.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bk.nicolike.cn

[R34] 退出时清理
来源：http://du.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://od.nicolike.cn

[R35] 后台执行并等待
来源：http://rl.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fl.huanxung.cn

[R36] 并发执行多个任务
来源：http://zu.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tk.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://uy.colortex.cn

files=$(ls -1)
来源：http://uc.hahajie.cn

[R38] 管道串联
来源：http://qs.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://uq.colortex.cn

[R39] 重定向标准输出与错误
来源：http://pn.muxihuayi.cn

cmd > out.log 2>&1
来源：http://mr.szsharing.cn

[R40] 追加写日志
来源：http://nw.szxytkj.cn

echo "log" >> out.log
来源：http://jw.521024.cn

[R41] 丢弃输出
来源：http://xj.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://lc.huixiangedu.cn

[R42] 输入重定向
来源：http://gj.huixinmuqiang.cn

wc -l < a.txt
来源：http://ek.chemitech.net.cn

[R43] 按名字查找文件
来源：http://ni.chemitech.net.cn

find . -name "*.log" -type f
来源：http://au.muxihuayi.cn

[R44] 按修改时间查找
来源：http://ux.gzmigu.cn

find . -mtime -7 -type f
来源：http://ps.huixiangedu.cn

[R45] 批量删除
来源：http://kq.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://el.panjiajie.cn

[R46] 递归替换文件内容
来源：http://hi.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xz.chemitech.net.cn

[R47] sed 单行替换
来源：http://oc.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uj.colortex.cn

[R48] awk 取指定列
来源：http://dt.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://qo.nszjky.cn

[R49] awk 带条件
来源：http://oz.shxzskj.cn


<!-- 参考信息 -->