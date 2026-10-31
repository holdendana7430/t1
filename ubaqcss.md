代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://wl.hahajie.cn

[Q09] 创建唯一索引
来源：http://fm.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mm.yuexingan06.cn

[Q10] 插入单行
来源：http://gb.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xs.nszjky.cn

[Q11] 一次插入多行
来源：http://bl.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://db.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://tb.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://za.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ht.gzmigu.cn

[Q13] 忽略重复插入
来源：http://op.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fq.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://lb.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ng.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yv.yuexingan06.cn

[Q15] 查询全部
来源：http://gu.muxihuayi.cn

SELECT * FROM users;
来源：http://pj.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://na.shtwfgs.cn

SELECT id, name FROM users;
来源：http://mq.huixinmuqiang.cn

[Q17] 条件查询
来源：http://ka.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://of.gzmigu.cn

[Q18] 模糊匹配
来源：http://ua.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mk.hnjuh.cn

[Q19] 范围查询
来源：http://qh.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ha.wgjwhj.cn

[Q20] IN 列表
来源：http://we.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://za.newstarts.cn

[Q21] 空值判断
来源：http://yv.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rk.yuntaijiaju.cn

[Q22] 排序
来源：http://gr.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sc.muxihuayi.cn

[Q23] 分页
来源：http://nq.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tu.9csxet.cn

[Q24] 去重
来源：http://qy.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://ko.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://ui.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ei.shxzskj.cn

[Q26] 计数
来源：http://ka.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://su.yuexingan06.cn

[Q27] 条件计数
来源：http://sy.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jj.huanxung.cn

[Q28] 求和与平均
来源：http://pp.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bn.hnjuh.cn

[Q29] 最大最小值
来源：http://uj.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mg.nszjky.cn

[Q30] 分组统计
来源：http://to.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ac.shxzukj.cn

[Q31] 分组后过滤
来源：http://ww.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cm.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://vh.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ap.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mx.newstarts.cn

[Q33] 多列分组
来源：http://ns.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rn.521024.cn

[Q34] 每组取第一条
来源：http://af.huanxung.cn

SELECT * FROM (
来源：http://pt.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://so.newstarts.cn

) t WHERE rn = 1;
来源：http://rd.szxytkj.cn

[Q35] 内连接
来源：http://gv.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gy.gzmigu.cn

[Q36] 左连接
来源：http://xj.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gr.gzmigu.cn

[Q37] 右连接
来源：http://ux.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wh.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jb.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://op.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://is.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sn.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rv.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fi.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gb.lnxyls.cn

[Q41] 多表连接
来源：http://id.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fl.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://fz.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://tl.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://lp.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://yy.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ts.huanxung.cn

[Q43] 标量子查询
来源：http://ya.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ir.jctech888.com.cn

[Q44] IN 子查询
来源：http://rp.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ny.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://tx.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nj.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fu.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bq.521024.cn

[Q47] 与平均值比较
来源：http://vw.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yc.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://hi.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xl.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://lv.huanxung.cn

[Q49] 更新单行
来源：http://io.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ci.colortex.cn

[Q50] 批量更新
来源：http://zl.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vr.shtwfgs.cn

[Q51] 用子查询更新
来源：http://tu.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fb.szxytkj.cn

[Q52] 删除指定行
来源：http://jp.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://nf.bjjhwx.cn

[Q53] 按条件删除
来源：http://yf.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ck.hnjuh.cn

[Q54] 清空表
来源：http://le.9csxet.cn

TRUNCATE TABLE logs;
来源：http://sh.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://kv.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hc.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://ch.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nk.huanxung.cn

[Q57] 行号
来源：http://iz.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ls.szsharing.cn

[Q58] 累计求和
来源：http://cj.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uw.huixiangedu.cn

[Q59] 分组内累计
来源：http://le.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qs.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://yu.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://km.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yw.nszjky.cn

[Q61] 移动平均
来源：http://uz.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xr.shxzukj.cn

[Q62] 分组占比
来源：http://ke.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ns.hnjuh.cn

[Q63] 开启事务
来源：http://px.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ry.chemitech.net.cn

[Q64] 提交事务
来源：http://uy.haigaiapp.cn

COMMIT;
来源：http://bm.521024.cn

[Q65] 回滚事务
来源：http://lp.huanxung.cn

ROLLBACK;
来源：http://kz.hnjuh.cn

[Q66] 行锁查询
来源：http://ar.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tr.lnxyls.cn

[Q67] 设置隔离级别
来源：http://wv.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://by.jianghongdianzi.cn

[Q68] 保存点
来源：http://wg.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://yw.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://jg.huixiangedu.cn

[Q69] 查看执行计划
来源：http://np.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yi.newstarts.cn

[Q70] 更新统计信息
来源：http://cp.szxytkj.cn

ANALYZE TABLE users;
来源：http://fv.muxihuayi.cn

[Q71] 查看建表语句
来源：http://kt.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bp.shtwfgs.cn

[Q72] 查看索引
来源：http://ft.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://ya.huanxung.cn

[Q73] 查看表状态
来源：http://ke.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bi.shtwfgs.cn

[Q74] 强制使用索引
来源：http://it.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vc.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://xs.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kp.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ok.colortex.cn

[Q76] 按天统计
来源：http://wk.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dy.colortex.cn

[Q77] 时间加减
来源：http://gw.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ri.jianghongdianzi.cn

[Q78] 当前时间
来源：http://ef.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://in.huixiangedu.cn

[Q79] 字符串拼接
来源：http://ck.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://im.yuexingan06.cn

[Q80] 字符串截取
来源：http://qo.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ee.chemitech.net.cn

[Q81] 字符串替换
来源：http://nb.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ya.asd995.cn

[Q82] 字符长度与字节长度
来源：http://hf.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yh.wgjwhj.cn

[Q83] 大小写转换
来源：http://ig.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ez.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://ix.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://ob.bookmarksfly.cn

[Q85] 数值取整
来源：http://zg.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://op.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://as.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cg.9csxet.cn

[Q87] JSON 字段做条件
来源：http://jv.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ji.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://ji.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hh.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ts.lnxyls.cn

[Q89] 判断表是否存在
来源：http://pl.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://th.jctech888.com.cn

[Q90] 生成序号列
来源：http://wr.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ou.shtwfgs.cn

================================================================================
来源：http://ku.9csxet.cn

R. Bash 专题
来源：http://rd.newstarts.cn

================================================================================
来源：http://zm.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://or.muxihuayi.cn

#!/usr/bin/env bash
来源：http://ip.wgjwhj.cn

set -euo pipefail
来源：http://yd.shxzukj.cn

[R02] 变量赋值与使用
来源：http://lo.nicolike.cn

name="Tom"; echo "$name"
来源：http://sw.521024.cn

[R03] 只读变量
来源：http://wr.szsharing.cn

readonly PI=3.14
来源：http://le.szsharing.cn

[R04] 位置参数
来源：http://bi.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vp.nicolike.cn

[R05] 参数默认值
来源：http://hx.haigaiapp.cn

name="${1:-default}"
来源：http://hk.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://cw.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uo.muxihuayi.cn

[R07] if 判断文件
来源：http://rk.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mb.huanxung.cn

[R08] 数值比较
来源：http://xu.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vg.jctech888.com.cn

[R09] 字符串比较
来源：http://zi.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ca.yuntaijiaju.cn

[R10] 正则匹配
来源：http://sa.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jh.haigaiapp.cn

[R11] case 多分支
来源：http://rb.yuexingan06.cn

case "$1" in
来源：http://ac.521024.cn

start) echo "启动" ;;
来源：http://qi.szxytkj.cn

stop)  echo "停止" ;;
来源：http://fh.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://qe.hahajie.cn

esac
来源：http://we.szxytkj.cn

[R12] for 遍历文件
来源：http://hy.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://ky.haigaiapp.cn

[R13] for 计数循环
来源：http://ec.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://xm.yuexingan06.cn

[R14] C 风格 for
来源：http://vg.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qj.jctech888.com.cn

[R15] while 逐行读文件
来源：http://nc.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ds.yuntaijiaju.cn

[R16] until 等待条件
来源：http://pn.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://de.nicolike.cn

[R17] 数组定义与取值
来源：http://su.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cn.huixiangedu.cn

[R18] 遍历数组
来源：http://ow.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://om.521024.cn

[R19] 数组长度
来源：http://ib.shxzukj.cn

echo "${#arr[@]}"
来源：http://qr.asd995.cn

[R20] 关联数组（字典）
来源：http://qo.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pb.szxytkj.cn

[R21] 字符串长度
来源：http://ra.lnxyls.cn

echo "${#s}"
来源：http://yu.panjiajie.cn

[R22] 截取子串
来源：http://hc.newstarts.cn

echo "${s:0:5}"
来源：http://td.shxzukj.cn

[R23] 字符串替换
来源：http://hz.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hi.jctech888.com.cn

[R24] 大小写转换
来源：http://jo.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ml.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://wn.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jv.shtwfgs.cn

[R26] 命令替换
来源：http://kw.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://hr.lnxyls.cn

[R27] 算术展开
来源：http://iv.huanxung.cn

echo $((1 + 2 * 3))
来源：http://cj.bjjhwx.cn

[R28] 浮点运算
来源：http://up.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://gv.newstarts.cn

[R29] 定义函数
来源：http://wt.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zn.gzmigu.cn

[R30] 函数返回状态码
来源：http://ra.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://ur.newstarts.cn

[R31] 局部变量
来源：http://dx.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://lv.nicolike.cn

[R32] 参数个数校验
来源：http://qw.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vj.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://fw.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://np.hahajie.cn

[R34] 退出时清理
来源：http://jn.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ql.colortex.cn

[R35] 后台执行并等待
来源：http://kn.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dj.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://nh.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ym.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://kv.newstarts.cn

files=$(ls -1)
来源：http://hy.nszjky.cn

[R38] 管道串联
来源：http://kn.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://ze.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://tq.shtwfgs.cn

cmd > out.log 2>&1
来源：http://wj.shxzukj.cn

[R40] 追加写日志
来源：http://ov.chemitech.net.cn

echo "log" >> out.log
来源：http://jj.lnxyls.cn

[R41] 丢弃输出
来源：http://pt.9csxet.cn

cmd >/dev/null 2>&1
来源：http://yn.521024.cn

[R42] 输入重定向
来源：http://he.9csxet.cn

wc -l < a.txt
来源：http://qb.hahajie.cn

[R43] 按名字查找文件
来源：http://tz.jctech888.com.cn

find . -name "*.log" -type f
来源：http://vc.huanxung.cn

[R44] 按修改时间查找
来源：http://vb.asd995.cn

find . -mtime -7 -type f
来源：http://sq.shxzskj.cn

[R45] 批量删除
来源：http://jg.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://sa.nszjky.cn

[R46] 递归替换文件内容
来源：http://lw.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://px.lnxyls.cn

[R47] sed 单行替换
来源：http://zj.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jw.bjjhwx.cn

[R48] awk 取指定列
来源：http://fa.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://dt.jctech888.com.cn

[R49] awk 带条件
来源：http://ho.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qs.chemitech.net.cn

[R50] awk 求和
来源：http://dc.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jy.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://px.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fc.asd995.cn

[R52] 统计行数
来源：http://sd.shxzskj.cn

wc -l a.txt
来源：http://cz.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://of.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sc.newstarts.cn

[R54] 比较两个文件
来源：http://ti.panjiajie.cn

diff a.txt b.txt
来源：http://cs.nszjky.cn

[R55] 压缩与解压
来源：http://jh.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sz.bjjhwx.cn

[R56] 远程拷贝
来源：http://dj.bookmarksfly.cn

scp file user@host:/path/
来源：http://lx.colortex.cn

[R57] 远程执行命令
来源：http://pj.panjiajie.cn


<!-- 参考信息 -->