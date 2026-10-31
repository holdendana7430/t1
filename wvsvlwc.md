代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://ub.panjiajie.cn

[Q09] 创建唯一索引
来源：http://iw.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xf.colortex.cn

[Q10] 插入单行
来源：http://vo.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://er.szxytkj.cn

[Q11] 一次插入多行
来源：http://ne.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eb.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://my.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yy.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dj.hahajie.cn

[Q13] 忽略重复插入
来源：http://ku.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mw.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://yv.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gt.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ia.shtwfgs.cn

[Q15] 查询全部
来源：http://nv.jctech888.com.cn

SELECT * FROM users;
来源：http://cm.hnjuh.cn

[Q16] 查询指定列
来源：http://qm.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://bn.szxytkj.cn

[Q17] 条件查询
来源：http://hf.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eb.nszjky.cn

[Q18] 模糊匹配
来源：http://pa.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yz.nicolike.cn

[Q19] 范围查询
来源：http://fw.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cu.521024.cn

[Q20] IN 列表
来源：http://zn.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ru.colortex.cn

[Q21] 空值判断
来源：http://xq.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cp.lnxyls.cn

[Q22] 排序
来源：http://hb.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://da.newstarts.cn

[Q23] 分页
来源：http://gy.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ws.shtwfgs.cn

[Q24] 去重
来源：http://wz.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://az.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://pc.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ko.shxzukj.cn

[Q26] 计数
来源：http://cg.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://un.huixiangedu.cn

[Q27] 条件计数
来源：http://tn.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iq.521024.cn

[Q28] 求和与平均
来源：http://gd.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ge.asd995.cn

[Q29] 最大最小值
来源：http://ls.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pf.colortex.cn

[Q30] 分组统计
来源：http://ws.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://no.9csxet.cn

[Q31] 分组后过滤
来源：http://ro.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://it.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://iy.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ut.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nz.huixinmuqiang.cn

[Q33] 多列分组
来源：http://dv.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pr.9csxet.cn

[Q34] 每组取第一条
来源：http://yv.gzmigu.cn

SELECT * FROM (
来源：http://vq.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lj.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://pu.lnxyls.cn

[Q35] 内连接
来源：http://jo.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://id.shxzskj.cn

[Q36] 左连接
来源：http://gw.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hb.shtwfgs.cn

[Q37] 右连接
来源：http://zc.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vk.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ee.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kn.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://bn.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ag.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zc.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ud.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ww.asd995.cn

[Q41] 多表连接
来源：http://oe.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dt.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://uh.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://yp.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://as.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://uv.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dm.nszjky.cn

[Q43] 标量子查询
来源：http://ha.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://px.jctech888.com.cn

[Q44] IN 子查询
来源：http://wr.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://so.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://ga.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://en.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qr.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bc.yuexingan06.cn

[Q47] 与平均值比较
来源：http://uy.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://no.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://al.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://un.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://oe.jianghongdianzi.cn

[Q49] 更新单行
来源：http://dv.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yg.gzmigu.cn

[Q50] 批量更新
来源：http://mg.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uf.nszjky.cn

[Q51] 用子查询更新
来源：http://ct.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cj.haigaiapp.cn

[Q52] 删除指定行
来源：http://ng.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://ay.nicolike.cn

[Q53] 按条件删除
来源：http://qw.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oe.521024.cn

[Q54] 清空表
来源：http://rr.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://nz.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://lt.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fg.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://qi.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wj.lnxyls.cn

[Q57] 行号
来源：http://aw.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fh.yuntaijiaju.cn

[Q58] 累计求和
来源：http://he.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ss.hahajie.cn

[Q59] 分组内累计
来源：http://kh.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zq.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://fk.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tk.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kq.asd995.cn

[Q61] 移动平均
来源：http://oq.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qd.jianghongdianzi.cn

[Q62] 分组占比
来源：http://jr.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ki.bookmarksfly.cn

[Q63] 开启事务
来源：http://qm.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://in.nszjky.cn

[Q64] 提交事务
来源：http://ie.colortex.cn

COMMIT;
来源：http://sf.chemitech.net.cn

[Q65] 回滚事务
来源：http://jx.hnjuh.cn

ROLLBACK;
来源：http://hk.hnjuh.cn

[Q66] 行锁查询
来源：http://rw.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fh.huanxung.cn

[Q67] 设置隔离级别
来源：http://jv.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://au.colortex.cn

[Q68] 保存点
来源：http://vx.jctech888.com.cn

SAVEPOINT sp1;
来源：http://uj.szxytkj.cn

ROLLBACK TO sp1;
来源：http://rd.shxzukj.cn

[Q69] 查看执行计划
来源：http://cw.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://el.bjjhwx.cn

[Q70] 更新统计信息
来源：http://jt.bjjhwx.cn

ANALYZE TABLE users;
来源：http://nf.bjjhwx.cn

[Q71] 查看建表语句
来源：http://tv.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hx.nicolike.cn

[Q72] 查看索引
来源：http://fi.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://tc.asd995.cn

[Q73] 查看表状态
来源：http://ie.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vb.colortex.cn

[Q74] 强制使用索引
来源：http://pd.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jl.panjiajie.cn

[Q75] 日期格式化
来源：http://yb.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://av.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://st.huanxung.cn

[Q76] 按天统计
来源：http://ez.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xm.wgjwhj.cn

[Q77] 时间加减
来源：http://os.hahajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jh.newstarts.cn

[Q78] 当前时间
来源：http://jf.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sp.haigaiapp.cn

[Q79] 字符串拼接
来源：http://dv.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iz.panjiajie.cn

[Q80] 字符串截取
来源：http://hn.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mp.hnjuh.cn

[Q81] 字符串替换
来源：http://id.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://di.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://my.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wu.shxzskj.cn

[Q83] 大小写转换
来源：http://fc.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://in.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://ob.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://su.hahajie.cn

[Q85] 数值取整
来源：http://vv.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yv.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://vw.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vp.hahajie.cn

[Q87] JSON 字段做条件
来源：http://ly.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yl.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://xk.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yu.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ks.9csxet.cn

[Q89] 判断表是否存在
来源：http://pr.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ya.lnxyls.cn

[Q90] 生成序号列
来源：http://km.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jy.jianghongdianzi.cn

================================================================================
来源：http://ym.szsharing.cn

R. Bash 专题
来源：http://ks.9csxet.cn

================================================================================
来源：http://ik.521024.cn

[R01] shebang 与严格模式
来源：http://mj.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://bc.nicolike.cn

set -euo pipefail
来源：http://yl.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://ew.gzmigu.cn

name="Tom"; echo "$name"
来源：http://zs.panjiajie.cn

[R03] 只读变量
来源：http://fj.huixinmuqiang.cn

readonly PI=3.14
来源：http://vv.newstarts.cn

[R04] 位置参数
来源：http://hl.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oh.bjjhwx.cn

[R05] 参数默认值
来源：http://ao.shxzskj.cn

name="${1:-default}"
来源：http://nr.9csxet.cn

[R06] 判断命令是否存在
来源：http://zi.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nd.colortex.cn

[R07] if 判断文件
来源：http://sq.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gr.yuexingan06.cn

[R08] 数值比较
来源：http://lo.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oq.yuexingan06.cn

[R09] 字符串比较
来源：http://ov.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qu.panjiajie.cn

[R10] 正则匹配
来源：http://zi.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ef.szxytkj.cn

[R11] case 多分支
来源：http://tg.9csxet.cn

case "$1" in
来源：http://rm.szxytkj.cn

start) echo "启动" ;;
来源：http://zt.521024.cn

stop)  echo "停止" ;;
来源：http://rh.521024.cn

*)     echo "未知命令" ;;
来源：http://zb.szxytkj.cn

esac
来源：http://kd.wgjwhj.cn

[R12] for 遍历文件
来源：http://uy.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://mi.chemitech.net.cn

[R13] for 计数循环
来源：http://bw.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://pf.shtwfgs.cn

[R14] C 风格 for
来源：http://yy.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oj.lnxyls.cn

[R15] while 逐行读文件
来源：http://xx.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uh.panjiajie.cn

[R16] until 等待条件
来源：http://gy.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pc.szsharing.cn

[R17] 数组定义与取值
来源：http://tv.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rh.hnjuh.cn

[R18] 遍历数组
来源：http://ca.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bx.nicolike.cn

[R19] 数组长度
来源：http://iq.hahajie.cn

echo "${#arr[@]}"
来源：http://zn.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://ed.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ye.bjjhwx.cn

[R21] 字符串长度
来源：http://pb.szxytkj.cn

echo "${#s}"
来源：http://pn.huanxung.cn

[R22] 截取子串
来源：http://ku.bjjhwx.cn

echo "${s:0:5}"
来源：http://jt.huixiangedu.cn

[R23] 字符串替换
来源：http://wr.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sy.nicolike.cn

[R24] 大小写转换
来源：http://gs.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yi.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://ap.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cc.panjiajie.cn

[R26] 命令替换
来源：http://pf.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://uy.hahajie.cn

[R27] 算术展开
来源：http://bt.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://pq.bjjhwx.cn

[R28] 浮点运算
来源：http://fw.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://cp.nicolike.cn

[R29] 定义函数
来源：http://ja.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ba.nszjky.cn

[R30] 函数返回状态码
来源：http://br.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://mp.shtwfgs.cn

[R31] 局部变量
来源：http://qu.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://kk.chemitech.net.cn

[R32] 参数个数校验
来源：http://at.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nv.asd995.cn

[R33] 捕获错误并提示行号
来源：http://bw.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ln.gzmigu.cn

[R34] 退出时清理
来源：http://dq.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://as.panjiajie.cn

[R35] 后台执行并等待
来源：http://al.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rf.shxzukj.cn

[R36] 并发执行多个任务
来源：http://qz.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yp.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://se.huixiangedu.cn

files=$(ls -1)
来源：http://yy.jctech888.com.cn

[R38] 管道串联
来源：http://pi.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://bj.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://aq.shxzukj.cn

cmd > out.log 2>&1
来源：http://ts.hnjuh.cn

[R40] 追加写日志
来源：http://zq.panjiajie.cn

echo "log" >> out.log
来源：http://bj.wgjwhj.cn

[R41] 丢弃输出
来源：http://cj.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://jj.521024.cn

[R42] 输入重定向
来源：http://wc.9csxet.cn

wc -l < a.txt
来源：http://sc.gzmigu.cn

[R43] 按名字查找文件
来源：http://rf.hahajie.cn

find . -name "*.log" -type f
来源：http://pc.hahajie.cn

[R44] 按修改时间查找
来源：http://tr.nszjky.cn

find . -mtime -7 -type f
来源：http://nt.hnjuh.cn

[R45] 批量删除
来源：http://al.szsharing.cn

find . -name "*.tmp" -delete
来源：http://js.shxzskj.cn

[R46] 递归替换文件内容
来源：http://jw.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ow.szsharing.cn

[R47] sed 单行替换
来源：http://nq.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://li.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://ou.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://op.chemitech.net.cn

[R49] awk 带条件
来源：http://wu.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jl.lnxyls.cn

[R50] awk 求和
来源：http://tb.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bn.gzmigu.cn

[R51] 排序去重取前几
来源：http://cy.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://la.chemitech.net.cn

[R52] 统计行数
来源：http://io.yuexingan06.cn

wc -l a.txt
来源：http://xl.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://hb.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wb.szsharing.cn

[R54] 比较两个文件
来源：http://vu.szxytkj.cn

diff a.txt b.txt
来源：http://jr.muxihuayi.cn

[R55] 压缩与解压
来源：http://js.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ut.haigaiapp.cn

[R56] 远程拷贝
来源：http://ud.nszjky.cn

scp file user@host:/path/
来源：http://wu.shxzukj.cn

[R57] 远程执行命令
来源：http://qp.jianghongdianzi.cn


<!-- 参考信息 -->