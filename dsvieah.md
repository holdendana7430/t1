代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ul.shxzskj.cn

);
来源：http://ai.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://yj.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://gx.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sq.newstarts.cn

user_id INT NOT NULL,
来源：http://wg.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://kr.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lr.9csxet.cn

);
来源：http://nz.jctech888.com.cn

[Q03] 增加列
来源：http://yn.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://to.wgjwhj.cn

[Q04] 修改列类型
来源：http://sj.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sl.panjiajie.cn

[Q05] 重命名列
来源：http://fa.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nc.gzmigu.cn

[Q06] 删除列
来源：http://yq.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://al.shtwfgs.cn

[Q07] 删除表
来源：http://da.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://vg.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://fe.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bo.colortex.cn

[Q09] 创建唯一索引
来源：http://ob.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ve.jianghongdianzi.cn

[Q10] 插入单行
来源：http://dq.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dj.shxzukj.cn

[Q11] 一次插入多行
来源：http://ic.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qu.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://of.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qb.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nx.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://xr.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xq.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://yg.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uz.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://di.huanxung.cn

[Q15] 查询全部
来源：http://dg.9csxet.cn

SELECT * FROM users;
来源：http://xs.shtwfgs.cn

[Q16] 查询指定列
来源：http://mk.hnjuh.cn

SELECT id, name FROM users;
来源：http://rs.panjiajie.cn

[Q17] 条件查询
来源：http://qd.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tj.chemitech.net.cn

[Q18] 模糊匹配
来源：http://hh.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sh.hnjuh.cn

[Q19] 范围查询
来源：http://cx.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ub.haigaiapp.cn

[Q20] IN 列表
来源：http://yg.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://an.nicolike.cn

[Q21] 空值判断
来源：http://hu.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zo.huixiangedu.cn

[Q22] 排序
来源：http://jn.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xj.hahajie.cn

[Q23] 分页
来源：http://oj.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rs.yuexingan06.cn

[Q24] 去重
来源：http://si.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://vg.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://rk.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rh.huixiangedu.cn

[Q26] 计数
来源：http://jn.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://ou.yuntaijiaju.cn

[Q27] 条件计数
来源：http://jm.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gc.newstarts.cn

[Q28] 求和与平均
来源：http://ic.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rd.szxytkj.cn

[Q29] 最大最小值
来源：http://xl.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uk.lnxyls.cn

[Q30] 分组统计
来源：http://eu.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://li.szxytkj.cn

[Q31] 分组后过滤
来源：http://br.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vv.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://xi.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ln.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gv.haigaiapp.cn

[Q33] 多列分组
来源：http://tb.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bj.shtwfgs.cn

[Q34] 每组取第一条
来源：http://pt.szsharing.cn

SELECT * FROM (
来源：http://pl.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pn.haigaiapp.cn

) t WHERE rn = 1;
来源：http://bo.szsharing.cn

[Q35] 内连接
来源：http://qs.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pd.gzmigu.cn

[Q36] 左连接
来源：http://ra.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pb.gzmigu.cn

[Q37] 右连接
来源：http://bg.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tz.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ly.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xg.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://uh.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ew.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zf.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tg.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cv.panjiajie.cn

[Q41] 多表连接
来源：http://cr.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ns.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://ln.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://uh.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://bh.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://ip.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hi.gzmigu.cn

[Q43] 标量子查询
来源：http://jm.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bv.chemitech.net.cn

[Q44] IN 子查询
来源：http://rp.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xb.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://tz.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fh.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mz.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dp.9csxet.cn

[Q47] 与平均值比较
来源：http://lm.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qs.asd995.cn

[Q48] CTE 公用表表达式
来源：http://dd.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dq.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://ym.newstarts.cn

[Q49] 更新单行
来源：http://sw.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tl.szxytkj.cn

[Q50] 批量更新
来源：http://lc.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gb.colortex.cn

[Q51] 用子查询更新
来源：http://ko.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ep.9csxet.cn

[Q52] 删除指定行
来源：http://hv.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://no.chemitech.net.cn

[Q53] 按条件删除
来源：http://it.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ru.nszjky.cn

[Q54] 清空表
来源：http://zs.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://ni.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://sz.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fh.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://lj.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ue.jianghongdianzi.cn

[Q57] 行号
来源：http://gl.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lf.szxytkj.cn

[Q58] 累计求和
来源：http://fm.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://br.shtwfgs.cn

[Q59] 分组内累计
来源：http://co.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xs.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://vs.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qf.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uc.shxzskj.cn

[Q61] 移动平均
来源：http://io.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ot.9csxet.cn

[Q62] 分组占比
来源：http://df.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ww.yuexingan06.cn

[Q63] 开启事务
来源：http://hv.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kh.nicolike.cn

[Q64] 提交事务
来源：http://kz.huixiangedu.cn

COMMIT;
来源：http://xt.haigaiapp.cn

[Q65] 回滚事务
来源：http://cf.yuexingan06.cn

ROLLBACK;
来源：http://kq.muxihuayi.cn

[Q66] 行锁查询
来源：http://pa.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qx.nicolike.cn

[Q67] 设置隔离级别
来源：http://kr.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mx.panjiajie.cn

[Q68] 保存点
来源：http://el.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://xo.asd995.cn

ROLLBACK TO sp1;
来源：http://uw.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://yz.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ar.szxytkj.cn

[Q70] 更新统计信息
来源：http://dh.panjiajie.cn

ANALYZE TABLE users;
来源：http://bu.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://ix.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iu.newstarts.cn

[Q72] 查看索引
来源：http://vl.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://bt.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://yc.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oh.lnxyls.cn

[Q74] 强制使用索引
来源：http://zt.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cl.shxzukj.cn

[Q75] 日期格式化
来源：http://ss.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tl.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ji.nicolike.cn

[Q76] 按天统计
来源：http://yn.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iv.haigaiapp.cn

[Q77] 时间加减
来源：http://yh.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fs.hahajie.cn

[Q78] 当前时间
来源：http://cx.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pn.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://nv.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hw.huanxung.cn

[Q80] 字符串截取
来源：http://sz.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ih.shtwfgs.cn

[Q81] 字符串替换
来源：http://ju.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gw.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://ac.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lh.szxytkj.cn

[Q83] 大小写转换
来源：http://er.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mo.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://bq.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://nk.bookmarksfly.cn

[Q85] 数值取整
来源：http://dx.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vs.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://bc.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tk.9csxet.cn

[Q87] JSON 字段做条件
来源：http://ss.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://st.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://qy.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qc.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jr.lnxyls.cn

[Q89] 判断表是否存在
来源：http://de.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cr.muxihuayi.cn

[Q90] 生成序号列
来源：http://vs.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tv.shxzukj.cn

================================================================================
来源：http://gc.bookmarksfly.cn

R. Bash 专题
来源：http://xd.nicolike.cn

================================================================================
来源：http://tm.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://al.521024.cn

#!/usr/bin/env bash
来源：http://lc.nszjky.cn

set -euo pipefail
来源：http://jb.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://xf.nicolike.cn

name="Tom"; echo "$name"
来源：http://jy.muxihuayi.cn

[R03] 只读变量
来源：http://ym.jctech888.com.cn

readonly PI=3.14
来源：http://mf.bjjhwx.cn

[R04] 位置参数
来源：http://uy.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qu.panjiajie.cn

[R05] 参数默认值
来源：http://tt.bjjhwx.cn

name="${1:-default}"
来源：http://fj.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://ph.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://if.9csxet.cn

[R07] if 判断文件
来源：http://sd.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cn.hahajie.cn

[R08] 数值比较
来源：http://un.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sl.huanxung.cn

[R09] 字符串比较
来源：http://bd.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jh.jctech888.com.cn

[R10] 正则匹配
来源：http://gu.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rn.asd995.cn

[R11] case 多分支
来源：http://lb.shtwfgs.cn

case "$1" in
来源：http://pa.haigaiapp.cn

start) echo "启动" ;;
来源：http://iy.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://qc.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://bd.521024.cn

esac
来源：http://jt.colortex.cn

[R12] for 遍历文件
来源：http://sk.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://rp.521024.cn

[R13] for 计数循环
来源：http://oi.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://hi.szsharing.cn

[R14] C 风格 for
来源：http://vt.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cj.shxzukj.cn

[R15] while 逐行读文件
来源：http://fe.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cv.shxzukj.cn

[R16] until 等待条件
来源：http://nr.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dk.gzmigu.cn

[R17] 数组定义与取值
来源：http://vl.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wg.huanxung.cn

[R18] 遍历数组
来源：http://op.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iy.huixinmuqiang.cn

[R19] 数组长度
来源：http://js.hnjuh.cn

echo "${#arr[@]}"
来源：http://vi.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://dc.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sd.szxytkj.cn

[R21] 字符串长度
来源：http://wr.yuntaijiaju.cn

echo "${#s}"
来源：http://nv.haigaiapp.cn

[R22] 截取子串
来源：http://rv.asd995.cn

echo "${s:0:5}"
来源：http://oa.haigaiapp.cn

[R23] 字符串替换
来源：http://mk.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pf.yuntaijiaju.cn

[R24] 大小写转换
来源：http://pe.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yh.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://eo.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ix.gzmigu.cn

[R26] 命令替换
来源：http://re.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://tf.hahajie.cn

[R27] 算术展开
来源：http://kg.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://df.bjjhwx.cn

[R28] 浮点运算
来源：http://zo.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://un.wgjwhj.cn

[R29] 定义函数
来源：http://cr.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mn.bjjhwx.cn

[R30] 函数返回状态码
来源：http://hf.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://ht.shtwfgs.cn

[R31] 局部变量
来源：http://vi.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://su.shxzukj.cn

[R32] 参数个数校验
来源：http://kn.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xk.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://fw.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qh.nszjky.cn

[R34] 退出时清理
来源：http://eg.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yw.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://hd.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xt.gzmigu.cn

[R36] 并发执行多个任务
来源：http://zh.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://va.szxytkj.cn

[R37] 把输出赋给变量
来源：http://lg.shxzskj.cn

files=$(ls -1)
来源：http://ae.panjiajie.cn

[R38] 管道串联
来源：http://gk.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://td.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://fz.9csxet.cn

cmd > out.log 2>&1
来源：http://xa.muxihuayi.cn

[R40] 追加写日志
来源：http://rj.colortex.cn

echo "log" >> out.log
来源：http://vg.haigaiapp.cn

[R41] 丢弃输出
来源：http://tg.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://dx.szxytkj.cn

[R42] 输入重定向
来源：http://td.shxzskj.cn

wc -l < a.txt
来源：http://sk.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://oq.lnxyls.cn

find . -name "*.log" -type f
来源：http://rd.panjiajie.cn

[R44] 按修改时间查找
来源：http://ek.bjjhwx.cn

find . -mtime -7 -type f
来源：http://vf.hnjuh.cn

[R45] 批量删除
来源：http://sb.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://qj.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://up.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ai.nszjky.cn

[R47] sed 单行替换
来源：http://si.yuexingan06.cn


<!-- 参考信息 -->