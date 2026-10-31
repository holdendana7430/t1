代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dp.chemitech.net.cn

[Q05] 重命名列
来源：http://br.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kq.panjiajie.cn

[Q06] 删除列
来源：http://fh.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kl.chemitech.net.cn

[Q07] 删除表
来源：http://ty.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://fk.newstarts.cn

[Q08] 创建普通索引
来源：http://gx.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lg.shxzukj.cn

[Q09] 创建唯一索引
来源：http://yj.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xe.huixiangedu.cn

[Q10] 插入单行
来源：http://ss.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zl.haigaiapp.cn

[Q11] 一次插入多行
来源：http://om.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qt.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://bd.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yg.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pb.shxzukj.cn

[Q13] 忽略重复插入
来源：http://rt.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lo.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://cq.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://br.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fl.hahajie.cn

[Q15] 查询全部
来源：http://iw.newstarts.cn

SELECT * FROM users;
来源：http://rb.shxzukj.cn

[Q16] 查询指定列
来源：http://ks.shxzukj.cn

SELECT id, name FROM users;
来源：http://nl.nszjky.cn

[Q17] 条件查询
来源：http://cn.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ou.yuexingan06.cn

[Q18] 模糊匹配
来源：http://lt.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mo.muxihuayi.cn

[Q19] 范围查询
来源：http://iv.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fb.bookmarksfly.cn

[Q20] IN 列表
来源：http://ym.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bj.huanxung.cn

[Q21] 空值判断
来源：http://ur.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://no.panjiajie.cn

[Q22] 排序
来源：http://uo.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://co.huanxung.cn

[Q23] 分页
来源：http://tj.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://re.hnjuh.cn

[Q24] 去重
来源：http://ib.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://cw.asd995.cn

[Q25] 只取前 N 条
来源：http://lk.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://td.shtwfgs.cn

[Q26] 计数
来源：http://uw.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://zq.bjjhwx.cn

[Q27] 条件计数
来源：http://vc.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lb.bjjhwx.cn

[Q28] 求和与平均
来源：http://fe.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mp.huixiangedu.cn

[Q29] 最大最小值
来源：http://an.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tt.wgjwhj.cn

[Q30] 分组统计
来源：http://tk.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oe.hnjuh.cn

[Q31] 分组后过滤
来源：http://kn.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zs.hahajie.cn

[Q32] 分组拼接字符串
来源：http://hh.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ez.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ti.szsharing.cn

[Q33] 多列分组
来源：http://jv.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nk.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://ey.gzmigu.cn

SELECT * FROM (
来源：http://ij.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hy.nszjky.cn

) t WHERE rn = 1;
来源：http://hl.nicolike.cn

[Q35] 内连接
来源：http://jh.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ix.9csxet.cn

[Q36] 左连接
来源：http://vv.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gr.wgjwhj.cn

[Q37] 右连接
来源：http://ah.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dw.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hs.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pu.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://zr.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bl.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xh.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nb.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wm.yuntaijiaju.cn

[Q41] 多表连接
来源：http://bm.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ip.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://at.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://is.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://fz.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://oz.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pu.chemitech.net.cn

[Q43] 标量子查询
来源：http://pi.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gg.panjiajie.cn

[Q44] IN 子查询
来源：http://tn.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vi.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://bd.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mz.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vv.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ve.newstarts.cn

[Q47] 与平均值比较
来源：http://gx.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eb.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://vu.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bg.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://kr.szsharing.cn

[Q49] 更新单行
来源：http://hb.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rf.hahajie.cn

[Q50] 批量更新
来源：http://bw.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mq.hnjuh.cn

[Q51] 用子查询更新
来源：http://ov.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://df.hnjuh.cn

[Q52] 删除指定行
来源：http://vb.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://fa.yuexingan06.cn

[Q53] 按条件删除
来源：http://hv.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qm.wgjwhj.cn

[Q54] 清空表
来源：http://ne.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://dp.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://nf.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jw.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://ig.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cf.521024.cn

[Q57] 行号
来源：http://qi.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qp.shxzukj.cn

[Q58] 累计求和
来源：http://yk.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uu.lnxyls.cn

[Q59] 分组内累计
来源：http://el.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ze.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://zc.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jf.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dc.huixiangedu.cn

[Q61] 移动平均
来源：http://xj.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bn.yuexingan06.cn

[Q62] 分组占比
来源：http://ou.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ap.9csxet.cn

[Q63] 开启事务
来源：http://ki.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ac.hnjuh.cn

[Q64] 提交事务
来源：http://of.wgjwhj.cn

COMMIT;
来源：http://rp.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://ii.hnjuh.cn

ROLLBACK;
来源：http://hp.hnjuh.cn

[Q66] 行锁查询
来源：http://lg.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rf.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://oz.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://he.bjjhwx.cn

[Q68] 保存点
来源：http://vb.hnjuh.cn

SAVEPOINT sp1;
来源：http://kh.hnjuh.cn

ROLLBACK TO sp1;
来源：http://kq.wgjwhj.cn

[Q69] 查看执行计划
来源：http://gx.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cu.panjiajie.cn

[Q70] 更新统计信息
来源：http://ka.asd995.cn

ANALYZE TABLE users;
来源：http://gh.shxzukj.cn

[Q71] 查看建表语句
来源：http://hl.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yl.panjiajie.cn

[Q72] 查看索引
来源：http://gq.521024.cn

SHOW INDEX FROM users;
来源：http://ha.muxihuayi.cn

[Q73] 查看表状态
来源：http://nl.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gh.colortex.cn

[Q74] 强制使用索引
来源：http://gc.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://db.asd995.cn

[Q75] 日期格式化
来源：http://cg.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zs.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://me.szxytkj.cn

[Q76] 按天统计
来源：http://ct.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nn.hahajie.cn

[Q77] 时间加减
来源：http://wm.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hx.asd995.cn

[Q78] 当前时间
来源：http://jm.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ow.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://tw.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pi.szsharing.cn

[Q80] 字符串截取
来源：http://dg.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qc.szsharing.cn

[Q81] 字符串替换
来源：http://se.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gy.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://ol.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yf.shtwfgs.cn

[Q83] 大小写转换
来源：http://rn.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lt.shxzukj.cn

[Q84] 去除首尾空格
来源：http://dc.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://mc.hahajie.cn

[Q85] 数值取整
来源：http://eg.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://je.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://op.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pq.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://px.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zy.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://sq.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cg.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wt.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://on.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xu.shxzukj.cn

[Q90] 生成序号列
来源：http://om.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ez.huixinmuqiang.cn

================================================================================
来源：http://xe.huixiangedu.cn

R. Bash 专题
来源：http://tv.521024.cn

================================================================================
来源：http://ew.hahajie.cn

[R01] shebang 与严格模式
来源：http://yk.lnxyls.cn

#!/usr/bin/env bash
来源：http://sp.muxihuayi.cn

set -euo pipefail
来源：http://ll.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://gw.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://yu.shxzukj.cn

[R03] 只读变量
来源：http://yq.panjiajie.cn

readonly PI=3.14
来源：http://uy.huixiangedu.cn

[R04] 位置参数
来源：http://ju.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pc.wgjwhj.cn

[R05] 参数默认值
来源：http://is.bjjhwx.cn

name="${1:-default}"
来源：http://kr.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://ho.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bv.chemitech.net.cn

[R07] if 判断文件
来源：http://yj.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gb.haigaiapp.cn

[R08] 数值比较
来源：http://ro.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mg.shtwfgs.cn

[R09] 字符串比较
来源：http://qw.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vo.bjjhwx.cn

[R10] 正则匹配
来源：http://pu.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kc.bjjhwx.cn

[R11] case 多分支
来源：http://fe.yuexingan06.cn

case "$1" in
来源：http://ay.shxzskj.cn

start) echo "启动" ;;
来源：http://vd.9csxet.cn

stop)  echo "停止" ;;
来源：http://ua.9csxet.cn

*)     echo "未知命令" ;;
来源：http://hq.9csxet.cn

esac
来源：http://qt.hahajie.cn

[R12] for 遍历文件
来源：http://ye.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://kt.shtwfgs.cn

[R13] for 计数循环
来源：http://oj.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://ex.szxytkj.cn

[R14] C 风格 for
来源：http://tp.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sx.shxzukj.cn

[R15] while 逐行读文件
来源：http://dp.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nb.nszjky.cn

[R16] until 等待条件
来源：http://ce.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qu.szsharing.cn

[R17] 数组定义与取值
来源：http://af.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mf.lnxyls.cn

[R18] 遍历数组
来源：http://cq.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pc.asd995.cn

[R19] 数组长度
来源：http://or.wgjwhj.cn

echo "${#arr[@]}"
来源：http://rr.nicolike.cn

[R20] 关联数组（字典）
来源：http://hk.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dm.huixinmuqiang.cn

[R21] 字符串长度
来源：http://bo.nszjky.cn

echo "${#s}"
来源：http://ct.hnjuh.cn

[R22] 截取子串
来源：http://da.nszjky.cn

echo "${s:0:5}"
来源：http://ev.chemitech.net.cn

[R23] 字符串替换
来源：http://ry.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zt.bjjhwx.cn

[R24] 大小写转换
来源：http://ty.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://no.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://mq.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://io.huixiangedu.cn

[R26] 命令替换
来源：http://ud.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://gs.huixiangedu.cn

[R27] 算术展开
来源：http://vz.huanxung.cn

echo $((1 + 2 * 3))
来源：http://tz.panjiajie.cn

[R28] 浮点运算
来源：http://pv.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://ky.szsharing.cn

[R29] 定义函数
来源：http://yd.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lf.shxzskj.cn

[R30] 函数返回状态码
来源：http://ng.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://rq.szxytkj.cn

[R31] 局部变量
来源：http://zs.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://wi.panjiajie.cn

[R32] 参数个数校验
来源：http://cb.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yg.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://lf.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://te.gzmigu.cn

[R34] 退出时清理
来源：http://kf.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ux.panjiajie.cn

[R35] 后台执行并等待
来源：http://zo.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xe.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://pi.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qp.szxytkj.cn

[R37] 把输出赋给变量
来源：http://bp.huixinmuqiang.cn

files=$(ls -1)
来源：http://cl.hnjuh.cn

[R38] 管道串联
来源：http://qi.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://cq.521024.cn

[R39] 重定向标准输出与错误
来源：http://hm.hahajie.cn

cmd > out.log 2>&1
来源：http://ep.hahajie.cn

[R40] 追加写日志
来源：http://rk.shxzskj.cn

echo "log" >> out.log
来源：http://dw.gzmigu.cn

[R41] 丢弃输出
来源：http://cd.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://sf.gzmigu.cn

[R42] 输入重定向
来源：http://nu.bjjhwx.cn

wc -l < a.txt
来源：http://rk.huixiangedu.cn

[R43] 按名字查找文件
来源：http://uj.huixiangedu.cn

find . -name "*.log" -type f
来源：http://hz.panjiajie.cn

[R44] 按修改时间查找
来源：http://gt.szxytkj.cn

find . -mtime -7 -type f
来源：http://zi.nicolike.cn

[R45] 批量删除
来源：http://oe.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://xy.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://wk.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sb.nicolike.cn

[R47] sed 单行替换
来源：http://xe.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cd.shtwfgs.cn

[R48] awk 取指定列
来源：http://cg.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://ic.colortex.cn

[R49] awk 带条件
来源：http://ac.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jh.bookmarksfly.cn

[R50] awk 求和
来源：http://xf.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yl.huixiangedu.cn

[R51] 排序去重取前几
来源：http://gu.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pq.muxihuayi.cn

[R52] 统计行数
来源：http://nd.haigaiapp.cn

wc -l a.txt
来源：http://jr.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://ff.newstarts.cn


<!-- 参考信息 -->