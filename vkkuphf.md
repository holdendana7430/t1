代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://yh.colortex.cn

[Q09] 创建唯一索引
来源：http://sb.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hh.bjjhwx.cn

[Q10] 插入单行
来源：http://qj.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://td.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://mh.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pr.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://zd.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ng.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jc.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://qs.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hi.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://zx.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ds.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jl.jctech888.com.cn

[Q15] 查询全部
来源：http://gr.panjiajie.cn

SELECT * FROM users;
来源：http://ak.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://sa.yuexingan06.cn

SELECT id, name FROM users;
来源：http://yj.chemitech.net.cn

[Q17] 条件查询
来源：http://fv.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pw.hnjuh.cn

[Q18] 模糊匹配
来源：http://mw.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hq.shxzukj.cn

[Q19] 范围查询
来源：http://gy.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zk.9csxet.cn

[Q20] IN 列表
来源：http://dh.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zj.wgjwhj.cn

[Q21] 空值判断
来源：http://in.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sr.bjjhwx.cn

[Q22] 排序
来源：http://or.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xm.hahajie.cn

[Q23] 分页
来源：http://kx.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xs.gzmigu.cn

[Q24] 去重
来源：http://bt.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://ls.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://ac.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ar.jctech888.com.cn

[Q26] 计数
来源：http://ai.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://fl.muxihuayi.cn

[Q27] 条件计数
来源：http://rz.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kx.nicolike.cn

[Q28] 求和与平均
来源：http://iz.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pp.asd995.cn

[Q29] 最大最小值
来源：http://co.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pm.gzmigu.cn

[Q30] 分组统计
来源：http://cn.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fw.haigaiapp.cn

[Q31] 分组后过滤
来源：http://wf.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cf.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://pj.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yv.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tf.wgjwhj.cn

[Q33] 多列分组
来源：http://zv.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cq.haigaiapp.cn

[Q34] 每组取第一条
来源：http://dj.nszjky.cn

SELECT * FROM (
来源：http://ai.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jb.chemitech.net.cn

) t WHERE rn = 1;
来源：http://ff.9csxet.cn

[Q35] 内连接
来源：http://by.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sp.panjiajie.cn

[Q36] 左连接
来源：http://oc.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bj.shtwfgs.cn

[Q37] 右连接
来源：http://fa.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qs.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rv.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ah.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://vg.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kb.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kr.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://re.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fc.jctech888.com.cn

[Q41] 多表连接
来源：http://th.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hl.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://iz.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://ex.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://gd.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://nl.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fn.nicolike.cn

[Q43] 标量子查询
来源：http://ia.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ek.9csxet.cn

[Q44] IN 子查询
来源：http://ja.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fd.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://fu.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jk.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gd.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ku.yuexingan06.cn

[Q47] 与平均值比较
来源：http://qb.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://an.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://zr.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ov.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://qi.haigaiapp.cn

[Q49] 更新单行
来源：http://nt.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ek.muxihuayi.cn

[Q50] 批量更新
来源：http://co.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://as.haigaiapp.cn

[Q51] 用子查询更新
来源：http://oa.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ua.panjiajie.cn

[Q52] 删除指定行
来源：http://ft.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://vq.gzmigu.cn

[Q53] 按条件删除
来源：http://ix.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vz.yuexingan06.cn

[Q54] 清空表
来源：http://qo.nszjky.cn

TRUNCATE TABLE logs;
来源：http://ci.521024.cn

[Q55] 排名（并列占位）
来源：http://ez.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iq.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://ae.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tr.hnjuh.cn

[Q57] 行号
来源：http://qp.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nx.lnxyls.cn

[Q58] 累计求和
来源：http://ce.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bw.huixiangedu.cn

[Q59] 分组内累计
来源：http://in.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qe.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://fa.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ak.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aw.asd995.cn

[Q61] 移动平均
来源：http://ds.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hm.newstarts.cn

[Q62] 分组占比
来源：http://dd.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bp.shtwfgs.cn

[Q63] 开启事务
来源：http://op.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dg.shxzukj.cn

[Q64] 提交事务
来源：http://me.521024.cn

COMMIT;
来源：http://mb.bookmarksfly.cn

[Q65] 回滚事务
来源：http://hi.bookmarksfly.cn

ROLLBACK;
来源：http://kd.hahajie.cn

[Q66] 行锁查询
来源：http://ao.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tj.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://cg.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gc.shxzskj.cn

[Q68] 保存点
来源：http://lb.wgjwhj.cn

SAVEPOINT sp1;
来源：http://hd.huanxung.cn

ROLLBACK TO sp1;
来源：http://lf.9csxet.cn

[Q69] 查看执行计划
来源：http://tw.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xz.shxzukj.cn

[Q70] 更新统计信息
来源：http://eb.nszjky.cn

ANALYZE TABLE users;
来源：http://pa.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://bl.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ns.lnxyls.cn

[Q72] 查看索引
来源：http://bk.colortex.cn

SHOW INDEX FROM users;
来源：http://kx.yuexingan06.cn

[Q73] 查看表状态
来源：http://dp.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rd.huixiangedu.cn

[Q74] 强制使用索引
来源：http://um.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ag.gzmigu.cn

[Q75] 日期格式化
来源：http://sl.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cu.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vs.yuntaijiaju.cn

[Q76] 按天统计
来源：http://yw.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://db.nszjky.cn

[Q77] 时间加减
来源：http://tl.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xw.521024.cn

[Q78] 当前时间
来源：http://kl.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uh.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://bn.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mm.bookmarksfly.cn

[Q80] 字符串截取
来源：http://bx.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ux.hnjuh.cn

[Q81] 字符串替换
来源：http://ek.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wr.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://iq.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qp.szxytkj.cn

[Q83] 大小写转换
来源：http://hq.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fb.shxzukj.cn

[Q84] 去除首尾空格
来源：http://yz.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://xk.panjiajie.cn

[Q85] 数值取整
来源：http://qh.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kk.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://ss.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://js.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://mf.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zi.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://no.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://on.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://il.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://ql.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gd.hahajie.cn

[Q90] 生成序号列
来源：http://jh.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mi.muxihuayi.cn

================================================================================
来源：http://kp.huixiangedu.cn

R. Bash 专题
来源：http://fh.huixinmuqiang.cn

================================================================================
来源：http://rt.shxzukj.cn

[R01] shebang 与严格模式
来源：http://ww.haigaiapp.cn

#!/usr/bin/env bash
来源：http://mb.bookmarksfly.cn

set -euo pipefail
来源：http://gl.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://th.colortex.cn

name="Tom"; echo "$name"
来源：http://zl.haigaiapp.cn

[R03] 只读变量
来源：http://wy.panjiajie.cn

readonly PI=3.14
来源：http://tt.yuntaijiaju.cn

[R04] 位置参数
来源：http://gu.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jk.shtwfgs.cn

[R05] 参数默认值
来源：http://xz.nszjky.cn

name="${1:-default}"
来源：http://sb.gzmigu.cn

[R06] 判断命令是否存在
来源：http://og.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xw.jctech888.com.cn

[R07] if 判断文件
来源：http://ka.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uy.yuntaijiaju.cn

[R08] 数值比较
来源：http://pj.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bn.szsharing.cn

[R09] 字符串比较
来源：http://ib.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bj.huanxung.cn

[R10] 正则匹配
来源：http://dc.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ia.huixiangedu.cn

[R11] case 多分支
来源：http://ze.panjiajie.cn

case "$1" in
来源：http://xy.nicolike.cn

start) echo "启动" ;;
来源：http://qf.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://mg.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://ef.panjiajie.cn

esac
来源：http://dw.newstarts.cn

[R12] for 遍历文件
来源：http://do.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://pp.shxzukj.cn

[R13] for 计数循环
来源：http://uz.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://vf.shtwfgs.cn

[R14] C 风格 for
来源：http://tt.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pk.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://es.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qm.chemitech.net.cn

[R16] until 等待条件
来源：http://of.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gq.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://fl.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zn.huixinmuqiang.cn

[R18] 遍历数组
来源：http://mg.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dx.hahajie.cn

[R19] 数组长度
来源：http://ez.bjjhwx.cn

echo "${#arr[@]}"
来源：http://ut.szxytkj.cn

[R20] 关联数组（字典）
来源：http://zr.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cn.shtwfgs.cn

[R21] 字符串长度
来源：http://ib.gzmigu.cn

echo "${#s}"
来源：http://du.szsharing.cn

[R22] 截取子串
来源：http://ls.newstarts.cn

echo "${s:0:5}"
来源：http://oo.huixiangedu.cn

[R23] 字符串替换
来源：http://ym.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rl.wgjwhj.cn

[R24] 大小写转换
来源：http://vt.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ew.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://ia.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nr.9csxet.cn

[R26] 命令替换
来源：http://yx.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://lv.jianghongdianzi.cn

[R27] 算术展开
来源：http://hq.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ri.shtwfgs.cn

[R28] 浮点运算
来源：http://xq.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://zi.lnxyls.cn

[R29] 定义函数
来源：http://cp.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dw.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://db.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://kn.yuexingan06.cn

[R31] 局部变量
来源：http://sp.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://ql.huanxung.cn

[R32] 参数个数校验
来源：http://vs.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ja.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://gm.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jk.szxytkj.cn

[R34] 退出时清理
来源：http://qu.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wy.muxihuayi.cn

[R35] 后台执行并等待
来源：http://iq.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nq.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://ki.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ow.hahajie.cn

[R37] 把输出赋给变量
来源：http://is.colortex.cn

files=$(ls -1)
来源：http://if.asd995.cn

[R38] 管道串联
来源：http://tf.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://dv.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://by.huanxung.cn

cmd > out.log 2>&1
来源：http://wo.huixinmuqiang.cn

[R40] 追加写日志
来源：http://fh.9csxet.cn

echo "log" >> out.log
来源：http://jz.szsharing.cn

[R41] 丢弃输出
来源：http://ed.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://ns.asd995.cn

[R42] 输入重定向
来源：http://yq.newstarts.cn

wc -l < a.txt
来源：http://qs.gzmigu.cn

[R43] 按名字查找文件
来源：http://is.colortex.cn

find . -name "*.log" -type f
来源：http://ab.wgjwhj.cn

[R44] 按修改时间查找
来源：http://bh.yuexingan06.cn

find . -mtime -7 -type f
来源：http://fn.jctech888.com.cn

[R45] 批量删除
来源：http://tj.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://qk.szxytkj.cn

[R46] 递归替换文件内容
来源：http://ka.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lm.bookmarksfly.cn

[R47] sed 单行替换
来源：http://pe.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ic.haigaiapp.cn

[R48] awk 取指定列
来源：http://ua.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://dg.huanxung.cn

[R49] awk 带条件
来源：http://ab.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vo.yuexingan06.cn

[R50] awk 求和
来源：http://ex.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qx.9csxet.cn

[R51] 排序去重取前几
来源：http://pd.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mf.szsharing.cn

[R52] 统计行数
来源：http://hr.nszjky.cn

wc -l a.txt
来源：http://ju.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://xr.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lu.bookmarksfly.cn

[R54] 比较两个文件
来源：http://vd.muxihuayi.cn

diff a.txt b.txt
来源：http://yr.szsharing.cn

[R55] 压缩与解压
来源：http://di.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ac.panjiajie.cn

[R56] 远程拷贝
来源：http://gu.lnxyls.cn

scp file user@host:/path/
来源：http://pg.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://bt.yuexingan06.cn


<!-- 参考信息 -->