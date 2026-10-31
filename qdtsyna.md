代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://sx.lnxyls.cn

[Q09] 创建唯一索引
来源：http://zp.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qi.wgjwhj.cn

[Q10] 插入单行
来源：http://nx.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gf.newstarts.cn

[Q11] 一次插入多行
来源：http://bz.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wt.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://rm.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://by.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vs.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://ph.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ca.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://qj.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eg.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://id.9csxet.cn

[Q15] 查询全部
来源：http://zh.shxzukj.cn

SELECT * FROM users;
来源：http://rt.lnxyls.cn

[Q16] 查询指定列
来源：http://cx.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://mm.521024.cn

[Q17] 条件查询
来源：http://ac.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ho.panjiajie.cn

[Q18] 模糊匹配
来源：http://rw.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ka.gzmigu.cn

[Q19] 范围查询
来源：http://uy.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lh.chemitech.net.cn

[Q20] IN 列表
来源：http://nx.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wk.shtwfgs.cn

[Q21] 空值判断
来源：http://xp.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wj.lnxyls.cn

[Q22] 排序
来源：http://zm.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mo.newstarts.cn

[Q23] 分页
来源：http://vt.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pv.panjiajie.cn

[Q24] 去重
来源：http://nu.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://yj.colortex.cn

[Q25] 只取前 N 条
来源：http://va.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cc.shxzskj.cn

[Q26] 计数
来源：http://cc.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://xl.szxytkj.cn

[Q27] 条件计数
来源：http://ke.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ql.shxzukj.cn

[Q28] 求和与平均
来源：http://tj.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vy.gzmigu.cn

[Q29] 最大最小值
来源：http://ik.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aj.hnjuh.cn

[Q30] 分组统计
来源：http://iv.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eh.colortex.cn

[Q31] 分组后过滤
来源：http://wa.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ko.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://ud.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jt.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gm.wgjwhj.cn

[Q33] 多列分组
来源：http://zq.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ym.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://ni.bjjhwx.cn

SELECT * FROM (
来源：http://qc.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://as.newstarts.cn

) t WHERE rn = 1;
来源：http://oa.hahajie.cn

[Q35] 内连接
来源：http://mb.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cp.huanxung.cn

[Q36] 左连接
来源：http://we.szxytkj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zl.yuntaijiaju.cn

[Q37] 右连接
来源：http://jk.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wz.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ma.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iu.asd995.cn

[Q39] 自连接（查上下级）
来源：http://lx.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ch.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://va.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zc.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ff.huixiangedu.cn

[Q41] 多表连接
来源：http://qy.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ja.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://kv.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://kh.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://bj.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://ke.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qb.gzmigu.cn

[Q43] 标量子查询
来源：http://hu.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wi.9csxet.cn

[Q44] IN 子查询
来源：http://dm.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mr.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://dw.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cf.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hu.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bg.nicolike.cn

[Q47] 与平均值比较
来源：http://od.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bh.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://zi.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://it.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://vu.chemitech.net.cn

[Q49] 更新单行
来源：http://st.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pn.newstarts.cn

[Q50] 批量更新
来源：http://eg.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pf.szxytkj.cn

[Q51] 用子查询更新
来源：http://ly.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nb.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://cf.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://jb.shxzukj.cn

[Q53] 按条件删除
来源：http://fd.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oq.lnxyls.cn

[Q54] 清空表
来源：http://ea.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://jo.nszjky.cn

[Q55] 排名（并列占位）
来源：http://pv.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gp.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://xp.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iu.jctech888.com.cn

[Q57] 行号
来源：http://js.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jl.yuntaijiaju.cn

[Q58] 累计求和
来源：http://kz.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xf.nicolike.cn

[Q59] 分组内累计
来源：http://if.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mq.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://kf.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ij.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gw.haigaiapp.cn

[Q61] 移动平均
来源：http://yd.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ob.gzmigu.cn

[Q62] 分组占比
来源：http://jw.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wp.panjiajie.cn

[Q63] 开启事务
来源：http://qk.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vb.bookmarksfly.cn

[Q64] 提交事务
来源：http://jh.yuntaijiaju.cn

COMMIT;
来源：http://yg.bjjhwx.cn

[Q65] 回滚事务
来源：http://eh.huanxung.cn

ROLLBACK;
来源：http://pl.lnxyls.cn

[Q66] 行锁查询
来源：http://zm.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mf.asd995.cn

[Q67] 设置隔离级别
来源：http://dd.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vf.panjiajie.cn

[Q68] 保存点
来源：http://bk.wgjwhj.cn

SAVEPOINT sp1;
来源：http://zk.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://lv.jctech888.com.cn

[Q69] 查看执行计划
来源：http://oh.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hd.lnxyls.cn

[Q70] 更新统计信息
来源：http://yy.hahajie.cn

ANALYZE TABLE users;
来源：http://ki.shtwfgs.cn

[Q71] 查看建表语句
来源：http://jg.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fv.9csxet.cn

[Q72] 查看索引
来源：http://sm.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://fe.colortex.cn

[Q73] 查看表状态
来源：http://nr.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hw.jctech888.com.cn

[Q74] 强制使用索引
来源：http://on.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gx.hahajie.cn

[Q75] 日期格式化
来源：http://gw.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mn.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://co.szsharing.cn

[Q76] 按天统计
来源：http://vu.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ms.nicolike.cn

[Q77] 时间加减
来源：http://pq.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sz.jctech888.com.cn

[Q78] 当前时间
来源：http://mu.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sq.asd995.cn

[Q79] 字符串拼接
来源：http://qu.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rj.asd995.cn

[Q80] 字符串截取
来源：http://uh.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://li.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://iv.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vd.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://sb.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fb.hnjuh.cn

[Q83] 大小写转换
来源：http://gh.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ht.szsharing.cn

[Q84] 去除首尾空格
来源：http://ae.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://uo.colortex.cn

[Q85] 数值取整
来源：http://dv.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zd.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://yp.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vw.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://wr.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dt.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://mo.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mk.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ds.521024.cn

[Q89] 判断表是否存在
来源：http://pl.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pv.nicolike.cn

[Q90] 生成序号列
来源：http://hh.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rj.yuntaijiaju.cn

================================================================================
来源：http://ay.shxzskj.cn

R. Bash 专题
来源：http://mv.bookmarksfly.cn

================================================================================
来源：http://lp.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://ew.nicolike.cn

#!/usr/bin/env bash
来源：http://go.lnxyls.cn

set -euo pipefail
来源：http://wl.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://fe.szxytkj.cn

name="Tom"; echo "$name"
来源：http://aq.nszjky.cn

[R03] 只读变量
来源：http://ru.nszjky.cn

readonly PI=3.14
来源：http://oj.huixiangedu.cn

[R04] 位置参数
来源：http://ys.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://db.szxytkj.cn

[R05] 参数默认值
来源：http://jd.521024.cn

name="${1:-default}"
来源：http://oj.nszjky.cn

[R06] 判断命令是否存在
来源：http://jg.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eo.yuntaijiaju.cn

[R07] if 判断文件
来源：http://rv.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://se.shtwfgs.cn

[R08] 数值比较
来源：http://ci.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xb.jctech888.com.cn

[R09] 字符串比较
来源：http://kj.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tt.nszjky.cn

[R10] 正则匹配
来源：http://eb.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bz.yuexingan06.cn

[R11] case 多分支
来源：http://ux.chemitech.net.cn

case "$1" in
来源：http://kp.colortex.cn

start) echo "启动" ;;
来源：http://yf.lnxyls.cn

stop)  echo "停止" ;;
来源：http://kj.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://fd.nicolike.cn

esac
来源：http://st.shxzskj.cn

[R12] for 遍历文件
来源：http://xy.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://rh.yuntaijiaju.cn

[R13] for 计数循环
来源：http://cr.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://fw.szsharing.cn

[R14] C 风格 for
来源：http://ly.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://az.hahajie.cn

[R15] while 逐行读文件
来源：http://pb.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://la.szsharing.cn

[R16] until 等待条件
来源：http://rb.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ql.huanxung.cn

[R17] 数组定义与取值
来源：http://dp.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ji.newstarts.cn

[R18] 遍历数组
来源：http://bb.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wp.jctech888.com.cn

[R19] 数组长度
来源：http://ao.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://tx.colortex.cn

[R20] 关联数组（字典）
来源：http://qo.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cn.szxytkj.cn

[R21] 字符串长度
来源：http://jr.shxzskj.cn

echo "${#s}"
来源：http://ex.newstarts.cn

[R22] 截取子串
来源：http://lf.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://vm.yuexingan06.cn

[R23] 字符串替换
来源：http://om.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://we.9csxet.cn

[R24] 大小写转换
来源：http://fj.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rc.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://nf.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mb.shxzukj.cn

[R26] 命令替换
来源：http://le.521024.cn

now=$(date +%F); echo "$now"
来源：http://ge.newstarts.cn

[R27] 算术展开
来源：http://wj.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://id.521024.cn

[R28] 浮点运算
来源：http://dj.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://eo.shxzskj.cn

[R29] 定义函数
来源：http://iv.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gt.hnjuh.cn

[R30] 函数返回状态码
来源：http://iv.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://in.gzmigu.cn

[R31] 局部变量
来源：http://sm.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://ct.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://nh.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ib.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://ph.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vk.asd995.cn

[R34] 退出时清理
来源：http://cl.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://et.szxytkj.cn

[R35] 后台执行并等待
来源：http://aj.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lg.hnjuh.cn

[R36] 并发执行多个任务
来源：http://ir.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zu.newstarts.cn

[R37] 把输出赋给变量
来源：http://qc.bookmarksfly.cn

files=$(ls -1)
来源：http://ew.panjiajie.cn

[R38] 管道串联
来源：http://la.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://bx.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://bm.huixiangedu.cn

cmd > out.log 2>&1
来源：http://qu.panjiajie.cn

[R40] 追加写日志
来源：http://bt.yuexingan06.cn

echo "log" >> out.log
来源：http://ga.hahajie.cn

[R41] 丢弃输出
来源：http://yh.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://hj.huanxung.cn

[R42] 输入重定向
来源：http://ec.muxihuayi.cn

wc -l < a.txt
来源：http://gv.asd995.cn

[R43] 按名字查找文件
来源：http://lo.lnxyls.cn

find . -name "*.log" -type f
来源：http://vh.hnjuh.cn

[R44] 按修改时间查找
来源：http://nk.jctech888.com.cn

find . -mtime -7 -type f
来源：http://us.newstarts.cn

[R45] 批量删除
来源：http://ui.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://eq.hnjuh.cn

[R46] 递归替换文件内容
来源：http://de.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dl.shxzskj.cn

[R47] sed 单行替换
来源：http://xb.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vs.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://ar.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://fg.huanxung.cn

[R49] awk 带条件
来源：http://bf.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zt.bjjhwx.cn

[R50] awk 求和
来源：http://by.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mg.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://vp.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ut.shxzskj.cn

[R52] 统计行数
来源：http://hv.panjiajie.cn

wc -l a.txt
来源：http://ys.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://bk.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cx.shtwfgs.cn

[R54] 比较两个文件
来源：http://az.huixinmuqiang.cn

diff a.txt b.txt
来源：http://gh.shxzskj.cn

[R55] 压缩与解压
来源：http://pn.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kp.szxytkj.cn

[R56] 远程拷贝
来源：http://if.bookmarksfly.cn

scp file user@host:/path/
来源：http://it.lnxyls.cn

[R57] 远程执行命令
来源：http://cw.bjjhwx.cn


<!-- 参考信息 -->