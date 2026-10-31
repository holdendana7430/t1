代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ec.shtwfgs.cn

);
来源：http://iw.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://mf.newstarts.cn

CREATE TABLE orders (
来源：http://st.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wy.hahajie.cn

user_id INT NOT NULL,
来源：http://sv.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://hg.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jt.bookmarksfly.cn

);
来源：http://sj.521024.cn

[Q03] 增加列
来源：http://uw.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wc.shxzskj.cn

[Q04] 修改列类型
来源：http://ng.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sc.asd995.cn

[Q05] 重命名列
来源：http://ly.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://am.szsharing.cn

[Q06] 删除列
来源：http://aw.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cg.shxzukj.cn

[Q07] 删除表
来源：http://zb.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://xn.hnjuh.cn

[Q08] 创建普通索引
来源：http://kw.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aj.lnxyls.cn

[Q09] 创建唯一索引
来源：http://hx.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gb.lnxyls.cn

[Q10] 插入单行
来源：http://lc.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://va.newstarts.cn

[Q11] 一次插入多行
来源：http://ln.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zl.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://qb.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ar.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zh.nicolike.cn

[Q13] 忽略重复插入
来源：http://kn.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pd.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://mt.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cx.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gz.bookmarksfly.cn

[Q15] 查询全部
来源：http://kv.bjjhwx.cn

SELECT * FROM users;
来源：http://mf.szxytkj.cn

[Q16] 查询指定列
来源：http://vi.szxytkj.cn

SELECT id, name FROM users;
来源：http://kv.wgjwhj.cn

[Q17] 条件查询
来源：http://vi.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://au.9csxet.cn

[Q18] 模糊匹配
来源：http://yc.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tz.haigaiapp.cn

[Q19] 范围查询
来源：http://rj.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ur.newstarts.cn

[Q20] IN 列表
来源：http://mw.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pn.panjiajie.cn

[Q21] 空值判断
来源：http://ht.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fj.hahajie.cn

[Q22] 排序
来源：http://fg.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wl.chemitech.net.cn

[Q23] 分页
来源：http://qe.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lk.lnxyls.cn

[Q24] 去重
来源：http://uy.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://am.colortex.cn

[Q25] 只取前 N 条
来源：http://hy.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mf.nszjky.cn

[Q26] 计数
来源：http://qp.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://wx.colortex.cn

[Q27] 条件计数
来源：http://ow.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dl.lnxyls.cn

[Q28] 求和与平均
来源：http://ce.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hn.asd995.cn

[Q29] 最大最小值
来源：http://rz.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gk.colortex.cn

[Q30] 分组统计
来源：http://yj.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jm.521024.cn

[Q31] 分组后过滤
来源：http://bv.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bw.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://ga.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ee.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qw.9csxet.cn

[Q33] 多列分组
来源：http://ni.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zo.jctech888.com.cn

[Q34] 每组取第一条
来源：http://lf.yuexingan06.cn

SELECT * FROM (
来源：http://if.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xy.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://ks.yuntaijiaju.cn

[Q35] 内连接
来源：http://yl.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sv.haigaiapp.cn

[Q36] 左连接
来源：http://se.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fg.gzmigu.cn

[Q37] 右连接
来源：http://xg.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gk.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ha.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://br.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://gi.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rz.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://io.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dy.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zp.huixinmuqiang.cn

[Q41] 多表连接
来源：http://pe.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dw.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://yv.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://qg.asd995.cn

[Q42] 连接条件附加过滤
来源：http://he.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://ha.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ci.szxytkj.cn

[Q43] 标量子查询
来源：http://kh.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://je.bookmarksfly.cn

[Q44] IN 子查询
来源：http://wr.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yi.asd995.cn

[Q45] EXISTS 判断存在
来源：http://py.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qj.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bj.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rl.haigaiapp.cn

[Q47] 与平均值比较
来源：http://rc.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dn.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://rv.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xi.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://tt.muxihuayi.cn

[Q49] 更新单行
来源：http://zg.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eo.muxihuayi.cn

[Q50] 批量更新
来源：http://cz.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fz.nszjky.cn

[Q51] 用子查询更新
来源：http://wg.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wp.nicolike.cn

[Q52] 删除指定行
来源：http://ir.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://rl.bjjhwx.cn

[Q53] 按条件删除
来源：http://xv.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ui.hahajie.cn

[Q54] 清空表
来源：http://nc.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://hn.nszjky.cn

[Q55] 排名（并列占位）
来源：http://qv.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zn.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://dz.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jq.newstarts.cn

[Q57] 行号
来源：http://co.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ma.9csxet.cn

[Q58] 累计求和
来源：http://by.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ln.panjiajie.cn

[Q59] 分组内累计
来源：http://he.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yn.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://pf.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lk.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wz.9csxet.cn

[Q61] 移动平均
来源：http://te.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tf.yuntaijiaju.cn

[Q62] 分组占比
来源：http://ea.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tw.haigaiapp.cn

[Q63] 开启事务
来源：http://lg.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fo.muxihuayi.cn

[Q64] 提交事务
来源：http://jn.huixiangedu.cn

COMMIT;
来源：http://xc.jctech888.com.cn

[Q65] 回滚事务
来源：http://sr.szsharing.cn

ROLLBACK;
来源：http://lt.newstarts.cn

[Q66] 行锁查询
来源：http://jy.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://au.szsharing.cn

[Q67] 设置隔离级别
来源：http://kj.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yt.szxytkj.cn

[Q68] 保存点
来源：http://bw.asd995.cn

SAVEPOINT sp1;
来源：http://nd.panjiajie.cn

ROLLBACK TO sp1;
来源：http://pl.wgjwhj.cn

[Q69] 查看执行计划
来源：http://fh.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lk.szxytkj.cn

[Q70] 更新统计信息
来源：http://kk.asd995.cn

ANALYZE TABLE users;
来源：http://yz.haigaiapp.cn

[Q71] 查看建表语句
来源：http://vk.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ps.nicolike.cn

[Q72] 查看索引
来源：http://ds.hnjuh.cn

SHOW INDEX FROM users;
来源：http://uq.chemitech.net.cn

[Q73] 查看表状态
来源：http://ds.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nz.colortex.cn

[Q74] 强制使用索引
来源：http://cr.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zj.jctech888.com.cn

[Q75] 日期格式化
来源：http://np.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xu.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tc.9csxet.cn

[Q76] 按天统计
来源：http://id.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mk.jianghongdianzi.cn

[Q77] 时间加减
来源：http://ly.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nu.lnxyls.cn

[Q78] 当前时间
来源：http://wu.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xp.shxzskj.cn

[Q79] 字符串拼接
来源：http://jw.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://um.521024.cn

[Q80] 字符串截取
来源：http://yf.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yw.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://nq.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mu.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://ao.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zd.panjiajie.cn

[Q83] 大小写转换
来源：http://qi.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ia.shxzskj.cn

[Q84] 去除首尾空格
来源：http://bd.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://bi.bookmarksfly.cn

[Q85] 数值取整
来源：http://zf.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ud.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://tg.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cn.nszjky.cn

[Q87] JSON 字段做条件
来源：http://wb.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nq.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://ns.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vt.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pk.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://gv.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kz.gzmigu.cn

[Q90] 生成序号列
来源：http://gm.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tp.nszjky.cn

================================================================================
来源：http://mh.yuexingan06.cn

R. Bash 专题
来源：http://sg.lnxyls.cn

================================================================================
来源：http://qa.szsharing.cn

[R01] shebang 与严格模式
来源：http://nk.521024.cn

#!/usr/bin/env bash
来源：http://eh.shxzukj.cn

set -euo pipefail
来源：http://vk.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://uv.asd995.cn

name="Tom"; echo "$name"
来源：http://li.shtwfgs.cn

[R03] 只读变量
来源：http://ok.muxihuayi.cn

readonly PI=3.14
来源：http://os.panjiajie.cn

[R04] 位置参数
来源：http://eo.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://or.hnjuh.cn

[R05] 参数默认值
来源：http://xm.newstarts.cn

name="${1:-default}"
来源：http://cx.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://cm.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qv.colortex.cn

[R07] if 判断文件
来源：http://vo.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://du.yuntaijiaju.cn

[R08] 数值比较
来源：http://lp.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fo.bjjhwx.cn

[R09] 字符串比较
来源：http://na.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lz.colortex.cn

[R10] 正则匹配
来源：http://hl.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hq.bookmarksfly.cn

[R11] case 多分支
来源：http://ft.521024.cn

case "$1" in
来源：http://vh.chemitech.net.cn

start) echo "启动" ;;
来源：http://jn.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://fn.hahajie.cn

*)     echo "未知命令" ;;
来源：http://ra.newstarts.cn

esac
来源：http://rz.shtwfgs.cn

[R12] for 遍历文件
来源：http://cj.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://jo.jianghongdianzi.cn

[R13] for 计数循环
来源：http://ne.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://bg.panjiajie.cn

[R14] C 风格 for
来源：http://db.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cg.lnxyls.cn

[R15] while 逐行读文件
来源：http://hn.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xg.panjiajie.cn

[R16] until 等待条件
来源：http://vf.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://km.nszjky.cn

[R17] 数组定义与取值
来源：http://bx.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jd.9csxet.cn

[R18] 遍历数组
来源：http://zy.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pl.jctech888.com.cn

[R19] 数组长度
来源：http://rt.shxzukj.cn

echo "${#arr[@]}"
来源：http://gy.shxzukj.cn

[R20] 关联数组（字典）
来源：http://sp.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vj.bookmarksfly.cn

[R21] 字符串长度
来源：http://cv.9csxet.cn

echo "${#s}"
来源：http://jk.huixinmuqiang.cn

[R22] 截取子串
来源：http://uz.huanxung.cn

echo "${s:0:5}"
来源：http://cc.yuexingan06.cn

[R23] 字符串替换
来源：http://sf.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xk.szxytkj.cn

[R24] 大小写转换
来源：http://rj.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://eq.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://gf.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hi.nicolike.cn

[R26] 命令替换
来源：http://dn.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://pl.jianghongdianzi.cn

[R27] 算术展开
来源：http://cm.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://xk.jctech888.com.cn

[R28] 浮点运算
来源：http://ai.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://mh.jctech888.com.cn

[R29] 定义函数
来源：http://ea.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jz.szxytkj.cn

[R30] 函数返回状态码
来源：http://fx.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://dl.huixiangedu.cn

[R31] 局部变量
来源：http://xp.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://jn.gzmigu.cn

[R32] 参数个数校验
来源：http://zp.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cp.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://dl.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wa.jianghongdianzi.cn

[R34] 退出时清理
来源：http://vp.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rr.shtwfgs.cn

[R35] 后台执行并等待
来源：http://yl.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://co.9csxet.cn

[R36] 并发执行多个任务
来源：http://qh.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kc.huanxung.cn

[R37] 把输出赋给变量
来源：http://ki.haigaiapp.cn

files=$(ls -1)
来源：http://vp.lnxyls.cn

[R38] 管道串联
来源：http://ys.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://ok.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://lh.hahajie.cn

cmd > out.log 2>&1
来源：http://lq.chemitech.net.cn

[R40] 追加写日志
来源：http://gm.huixinmuqiang.cn

echo "log" >> out.log
来源：http://jp.9csxet.cn

[R41] 丢弃输出
来源：http://sm.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://uj.bookmarksfly.cn

[R42] 输入重定向
来源：http://tu.jianghongdianzi.cn

wc -l < a.txt
来源：http://nm.nicolike.cn

[R43] 按名字查找文件
来源：http://gt.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://jz.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://xr.wgjwhj.cn

find . -mtime -7 -type f
来源：http://pk.shtwfgs.cn

[R45] 批量删除
来源：http://pb.9csxet.cn

find . -name "*.tmp" -delete
来源：http://vj.asd995.cn

[R46] 递归替换文件内容
来源：http://zj.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://og.hahajie.cn

[R47] sed 单行替换
来源：http://ms.yuntaijiaju.cn


<!-- 参考信息 -->