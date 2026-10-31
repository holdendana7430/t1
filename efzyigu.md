代发 wailian999

);
来源：http://dt.huanxung.cn

[Q03] 增加列
来源：http://ef.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ob.hnjuh.cn

[Q04] 修改列类型
来源：http://vc.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ug.szsharing.cn

[Q05] 重命名列
来源：http://pc.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zf.huixinmuqiang.cn

[Q06] 删除列
来源：http://qo.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cr.wgjwhj.cn

[Q07] 删除表
来源：http://qi.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://vh.shxzukj.cn

[Q08] 创建普通索引
来源：http://zv.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xm.hnjuh.cn

[Q09] 创建唯一索引
来源：http://rs.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vu.9csxet.cn

[Q10] 插入单行
来源：http://ax.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tq.nicolike.cn

[Q11] 一次插入多行
来源：http://wk.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kd.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://kv.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ke.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bu.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://ck.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://me.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://ha.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lp.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ku.yuexingan06.cn

[Q15] 查询全部
来源：http://vm.gzmigu.cn

SELECT * FROM users;
来源：http://ef.haigaiapp.cn

[Q16] 查询指定列
来源：http://rk.gzmigu.cn

SELECT id, name FROM users;
来源：http://ef.szxytkj.cn

[Q17] 条件查询
来源：http://pa.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ik.muxihuayi.cn

[Q18] 模糊匹配
来源：http://qd.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wc.colortex.cn

[Q19] 范围查询
来源：http://aw.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cx.newstarts.cn

[Q20] IN 列表
来源：http://fe.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://do.shxzukj.cn

[Q21] 空值判断
来源：http://qc.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cm.newstarts.cn

[Q22] 排序
来源：http://ab.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vh.wgjwhj.cn

[Q23] 分页
来源：http://ca.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sw.jianghongdianzi.cn

[Q24] 去重
来源：http://ji.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://jh.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://zf.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aa.szsharing.cn

[Q26] 计数
来源：http://dh.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://ol.shtwfgs.cn

[Q27] 条件计数
来源：http://wl.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wb.szxytkj.cn

[Q28] 求和与平均
来源：http://yd.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fd.shtwfgs.cn

[Q29] 最大最小值
来源：http://lo.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qp.nszjky.cn

[Q30] 分组统计
来源：http://ny.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ct.szsharing.cn

[Q31] 分组后过滤
来源：http://gd.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zs.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://yz.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lu.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pe.colortex.cn

[Q33] 多列分组
来源：http://ve.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tm.asd995.cn

[Q34] 每组取第一条
来源：http://oz.colortex.cn

SELECT * FROM (
来源：http://dm.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://df.jctech888.com.cn

) t WHERE rn = 1;
来源：http://fr.haigaiapp.cn

[Q35] 内连接
来源：http://wl.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vw.nicolike.cn

[Q36] 左连接
来源：http://ae.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pe.shxzukj.cn

[Q37] 右连接
来源：http://li.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xu.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wh.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hk.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://ml.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ur.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pf.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sw.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lo.szxytkj.cn

[Q41] 多表连接
来源：http://fc.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uf.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://bm.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://uu.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://tf.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://hw.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nc.wgjwhj.cn

[Q43] 标量子查询
来源：http://xj.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qq.huanxung.cn

[Q44] IN 子查询
来源：http://ih.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sq.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://bi.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://go.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ov.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sx.bjjhwx.cn

[Q47] 与平均值比较
来源：http://gl.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jt.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://dz.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uz.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://st.jianghongdianzi.cn

[Q49] 更新单行
来源：http://ng.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qq.lnxyls.cn

[Q50] 批量更新
来源：http://zy.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hg.yuexingan06.cn

[Q51] 用子查询更新
来源：http://zn.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sm.bookmarksfly.cn

[Q52] 删除指定行
来源：http://sl.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://un.chemitech.net.cn

[Q53] 按条件删除
来源：http://da.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iz.hnjuh.cn

[Q54] 清空表
来源：http://qw.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://it.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://lq.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://of.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://ik.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ny.wgjwhj.cn

[Q57] 行号
来源：http://jo.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://px.jianghongdianzi.cn

[Q58] 累计求和
来源：http://vn.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://it.shtwfgs.cn

[Q59] 分组内累计
来源：http://cu.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dv.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://oq.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qb.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://il.haigaiapp.cn

[Q61] 移动平均
来源：http://rw.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qz.asd995.cn

[Q62] 分组占比
来源：http://iw.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gl.huixinmuqiang.cn

[Q63] 开启事务
来源：http://jh.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fd.jianghongdianzi.cn

[Q64] 提交事务
来源：http://lx.shxzskj.cn

COMMIT;
来源：http://wk.muxihuayi.cn

[Q65] 回滚事务
来源：http://kw.yuntaijiaju.cn

ROLLBACK;
来源：http://sz.521024.cn

[Q66] 行锁查询
来源：http://qw.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dz.gzmigu.cn

[Q67] 设置隔离级别
来源：http://oq.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sd.hahajie.cn

[Q68] 保存点
来源：http://af.chemitech.net.cn

SAVEPOINT sp1;
来源：http://db.nszjky.cn

ROLLBACK TO sp1;
来源：http://qj.haigaiapp.cn

[Q69] 查看执行计划
来源：http://kv.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wi.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://am.huanxung.cn

ANALYZE TABLE users;
来源：http://yh.colortex.cn

[Q71] 查看建表语句
来源：http://le.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zb.lnxyls.cn

[Q72] 查看索引
来源：http://rh.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://hs.muxihuayi.cn

[Q73] 查看表状态
来源：http://dq.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mz.szsharing.cn

[Q74] 强制使用索引
来源：http://qw.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xu.wgjwhj.cn

[Q75] 日期格式化
来源：http://dr.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://de.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ap.haigaiapp.cn

[Q76] 按天统计
来源：http://qi.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yc.shtwfgs.cn

[Q77] 时间加减
来源：http://za.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://px.newstarts.cn

[Q78] 当前时间
来源：http://hh.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://um.szxytkj.cn

[Q79] 字符串拼接
来源：http://cb.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gh.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://qu.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shtwfgs.cn

[Q81] 字符串替换
来源：http://rb.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tx.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://qa.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jg.jctech888.com.cn

[Q83] 大小写转换
来源：http://bo.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ns.hnjuh.cn

[Q84] 去除首尾空格
来源：http://gg.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://hd.huixiangedu.cn

[Q85] 数值取整
来源：http://xn.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ra.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://bk.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xv.9csxet.cn

[Q87] JSON 字段做条件
来源：http://xa.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vi.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://av.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nm.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ax.szxytkj.cn

[Q89] 判断表是否存在
来源：http://xw.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rf.nicolike.cn

[Q90] 生成序号列
来源：http://ps.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kt.jianghongdianzi.cn

================================================================================
来源：http://nq.wgjwhj.cn

R. Bash 专题
来源：http://is.9csxet.cn

================================================================================
来源：http://pj.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://xe.hnjuh.cn

#!/usr/bin/env bash
来源：http://ms.hahajie.cn

set -euo pipefail
来源：http://vk.521024.cn

[R02] 变量赋值与使用
来源：http://kg.shxzukj.cn

name="Tom"; echo "$name"
来源：http://lm.szsharing.cn

[R03] 只读变量
来源：http://ri.gzmigu.cn

readonly PI=3.14
来源：http://cr.hahajie.cn

[R04] 位置参数
来源：http://eb.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xy.szxytkj.cn

[R05] 参数默认值
来源：http://io.jianghongdianzi.cn

name="${1:-default}"
来源：http://ux.hahajie.cn

[R06] 判断命令是否存在
来源：http://kz.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yq.newstarts.cn

[R07] if 判断文件
来源：http://bd.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kl.newstarts.cn

[R08] 数值比较
来源：http://op.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gz.huixiangedu.cn

[R09] 字符串比较
来源：http://tz.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pb.asd995.cn

[R10] 正则匹配
来源：http://ax.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vz.bjjhwx.cn

[R11] case 多分支
来源：http://jf.haigaiapp.cn

case "$1" in
来源：http://al.szsharing.cn

start) echo "启动" ;;
来源：http://ab.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://br.colortex.cn

*)     echo "未知命令" ;;
来源：http://na.haigaiapp.cn

esac
来源：http://ig.shxzukj.cn

[R12] for 遍历文件
来源：http://aj.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://ec.szsharing.cn

[R13] for 计数循环
来源：http://zs.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://mr.huixiangedu.cn

[R14] C 风格 for
来源：http://sk.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ws.521024.cn

[R15] while 逐行读文件
来源：http://sd.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mz.shtwfgs.cn

[R16] until 等待条件
来源：http://fu.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://is.szsharing.cn

[R17] 数组定义与取值
来源：http://kd.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qt.chemitech.net.cn

[R18] 遍历数组
来源：http://ku.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ud.bookmarksfly.cn

[R19] 数组长度
来源：http://ci.panjiajie.cn

echo "${#arr[@]}"
来源：http://sl.shxzskj.cn

[R20] 关联数组（字典）
来源：http://os.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tj.wgjwhj.cn

[R21] 字符串长度
来源：http://ic.muxihuayi.cn

echo "${#s}"
来源：http://jz.9csxet.cn

[R22] 截取子串
来源：http://lr.chemitech.net.cn

echo "${s:0:5}"
来源：http://tl.nicolike.cn

[R23] 字符串替换
来源：http://da.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lk.shtwfgs.cn

[R24] 大小写转换
来源：http://ds.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dy.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://cy.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jw.shxzskj.cn

[R26] 命令替换
来源：http://gf.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://mi.521024.cn

[R27] 算术展开
来源：http://ob.hahajie.cn

echo $((1 + 2 * 3))
来源：http://cb.huixinmuqiang.cn

[R28] 浮点运算
来源：http://dx.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://uw.yuntaijiaju.cn

[R29] 定义函数
来源：http://qz.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cg.521024.cn

[R30] 函数返回状态码
来源：http://ja.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://jq.bookmarksfly.cn

[R31] 局部变量
来源：http://nb.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://ev.lnxyls.cn

[R32] 参数个数校验
来源：http://xh.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cn.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://lj.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yb.jianghongdianzi.cn

[R34] 退出时清理
来源：http://mx.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dv.chemitech.net.cn

[R35] 后台执行并等待
来源：http://ne.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tp.nszjky.cn

[R36] 并发执行多个任务
来源：http://hn.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fb.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://cj.colortex.cn

files=$(ls -1)
来源：http://cc.haigaiapp.cn

[R38] 管道串联
来源：http://gm.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://qx.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://yj.shxzukj.cn

cmd > out.log 2>&1
来源：http://xj.panjiajie.cn

[R40] 追加写日志
来源：http://fd.colortex.cn

echo "log" >> out.log
来源：http://qp.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://ir.newstarts.cn

cmd >/dev/null 2>&1
来源：http://ok.bjjhwx.cn

[R42] 输入重定向
来源：http://rf.9csxet.cn

wc -l < a.txt
来源：http://wn.9csxet.cn

[R43] 按名字查找文件
来源：http://dc.huanxung.cn

find . -name "*.log" -type f
来源：http://zl.nicolike.cn

[R44] 按修改时间查找
来源：http://br.shxzukj.cn

find . -mtime -7 -type f
来源：http://oe.jianghongdianzi.cn

[R45] 批量删除
来源：http://ig.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://op.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://de.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ep.lnxyls.cn

[R47] sed 单行替换
来源：http://vp.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ud.asd995.cn

[R48] awk 取指定列
来源：http://mc.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://ud.huanxung.cn

[R49] awk 带条件
来源：http://wd.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nd.huixiangedu.cn

[R50] awk 求和
来源：http://dh.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jc.9csxet.cn

[R51] 排序去重取前几
来源：http://cu.yuntaijiaju.cn


<!-- 参考信息 -->