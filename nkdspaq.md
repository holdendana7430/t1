代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://re.huanxung.cn

user_id INT NOT NULL,
来源：http://cl.hahajie.cn

amount DECIMAL(10, 2),
来源：http://wg.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wx.chemitech.net.cn

);
来源：http://cx.nicolike.cn

[Q03] 增加列
来源：http://uq.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jd.panjiajie.cn

[Q04] 修改列类型
来源：http://ln.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ic.muxihuayi.cn

[Q05] 重命名列
来源：http://uj.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://va.bookmarksfly.cn

[Q06] 删除列
来源：http://ck.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cg.colortex.cn

[Q07] 删除表
来源：http://qu.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://cd.colortex.cn

[Q08] 创建普通索引
来源：http://yl.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tb.szsharing.cn

[Q09] 创建唯一索引
来源：http://gk.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yh.jianghongdianzi.cn

[Q10] 插入单行
来源：http://jb.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jf.colortex.cn

[Q11] 一次插入多行
来源：http://ps.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xq.asd995.cn

[Q12] 插入后取自增 ID
来源：http://xi.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ve.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oo.panjiajie.cn

[Q13] 忽略重复插入
来源：http://un.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yh.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://lb.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cf.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uz.shtwfgs.cn

[Q15] 查询全部
来源：http://bl.wgjwhj.cn

SELECT * FROM users;
来源：http://bh.jctech888.com.cn

[Q16] 查询指定列
来源：http://on.panjiajie.cn

SELECT id, name FROM users;
来源：http://vi.jctech888.com.cn

[Q17] 条件查询
来源：http://dt.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zg.shtwfgs.cn

[Q18] 模糊匹配
来源：http://sm.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tg.wgjwhj.cn

[Q19] 范围查询
来源：http://wl.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://th.nszjky.cn

[Q20] IN 列表
来源：http://yt.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eu.szsharing.cn

[Q21] 空值判断
来源：http://jk.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jv.yuexingan06.cn

[Q22] 排序
来源：http://xd.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yf.panjiajie.cn

[Q23] 分页
来源：http://cs.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dm.gzmigu.cn

[Q24] 去重
来源：http://xd.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://en.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://iz.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jp.asd995.cn

[Q26] 计数
来源：http://ka.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://rn.huixiangedu.cn

[Q27] 条件计数
来源：http://rv.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://on.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://fz.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zq.nszjky.cn

[Q29] 最大最小值
来源：http://if.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ve.jianghongdianzi.cn

[Q30] 分组统计
来源：http://zs.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wd.jctech888.com.cn

[Q31] 分组后过滤
来源：http://kj.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://av.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://fj.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kr.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zv.gzmigu.cn

[Q33] 多列分组
来源：http://kk.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wr.lnxyls.cn

[Q34] 每组取第一条
来源：http://tq.huanxung.cn

SELECT * FROM (
来源：http://vp.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sl.shtwfgs.cn

) t WHERE rn = 1;
来源：http://xf.jctech888.com.cn

[Q35] 内连接
来源：http://ru.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hn.shtwfgs.cn

[Q36] 左连接
来源：http://bn.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hj.bookmarksfly.cn

[Q37] 右连接
来源：http://ct.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dy.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yj.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zx.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://rm.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ul.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xg.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aa.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vo.hahajie.cn

[Q41] 多表连接
来源：http://bj.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jy.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://ho.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://aa.colortex.cn

[Q42] 连接条件附加过滤
来源：http://ox.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://su.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qp.hnjuh.cn

[Q43] 标量子查询
来源：http://dg.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ez.shxzukj.cn

[Q44] IN 子查询
来源：http://po.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cr.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://bo.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uy.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rg.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vs.newstarts.cn

[Q47] 与平均值比较
来源：http://gn.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://si.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://lt.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://js.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://vu.colortex.cn

[Q49] 更新单行
来源：http://fc.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ym.szxytkj.cn

[Q50] 批量更新
来源：http://kt.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pi.huixiangedu.cn

[Q51] 用子查询更新
来源：http://vv.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ca.chemitech.net.cn

[Q52] 删除指定行
来源：http://mh.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://ya.haigaiapp.cn

[Q53] 按条件删除
来源：http://nk.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gs.szsharing.cn

[Q54] 清空表
来源：http://lu.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://gk.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://ap.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wn.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://gt.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xo.haigaiapp.cn

[Q57] 行号
来源：http://kg.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kk.521024.cn

[Q58] 累计求和
来源：http://ej.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xt.nszjky.cn

[Q59] 分组内累计
来源：http://ho.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sv.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://kj.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gm.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wj.yuexingan06.cn

[Q61] 移动平均
来源：http://on.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ds.panjiajie.cn

[Q62] 分组占比
来源：http://zd.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ed.shtwfgs.cn

[Q63] 开启事务
来源：http://fp.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dw.lnxyls.cn

[Q64] 提交事务
来源：http://mc.521024.cn

COMMIT;
来源：http://hi.szsharing.cn

[Q65] 回滚事务
来源：http://dd.szxytkj.cn

ROLLBACK;
来源：http://ig.szsharing.cn

[Q66] 行锁查询
来源：http://pg.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ip.gzmigu.cn

[Q67] 设置隔离级别
来源：http://kq.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gf.jctech888.com.cn

[Q68] 保存点
来源：http://py.nicolike.cn

SAVEPOINT sp1;
来源：http://dw.nicolike.cn

ROLLBACK TO sp1;
来源：http://hj.huanxung.cn

[Q69] 查看执行计划
来源：http://vi.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wu.nicolike.cn

[Q70] 更新统计信息
来源：http://jm.shtwfgs.cn

ANALYZE TABLE users;
来源：http://ay.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://do.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yh.bookmarksfly.cn

[Q72] 查看索引
来源：http://dw.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://gp.wgjwhj.cn

[Q73] 查看表状态
来源：http://zb.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gx.huanxung.cn

[Q74] 强制使用索引
来源：http://li.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ej.nszjky.cn

[Q75] 日期格式化
来源：http://tx.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tv.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gk.bjjhwx.cn

[Q76] 按天统计
来源：http://jw.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sx.shxzskj.cn

[Q77] 时间加减
来源：http://qo.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ai.panjiajie.cn

[Q78] 当前时间
来源：http://iq.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yg.9csxet.cn

[Q79] 字符串拼接
来源：http://ka.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qn.hahajie.cn

[Q80] 字符串截取
来源：http://rv.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dv.bjjhwx.cn

[Q81] 字符串替换
来源：http://iy.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ko.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://ux.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fb.jctech888.com.cn

[Q83] 大小写转换
来源：http://xe.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jr.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://sr.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://tq.szsharing.cn

[Q85] 数值取整
来源：http://mh.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fm.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://qe.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://by.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://wv.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ey.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://hs.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nx.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pw.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://id.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ea.huixiangedu.cn

[Q90] 生成序号列
来源：http://si.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yv.gzmigu.cn

================================================================================
来源：http://oc.shxzukj.cn

R. Bash 专题
来源：http://vt.asd995.cn

================================================================================
来源：http://oc.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://my.panjiajie.cn

#!/usr/bin/env bash
来源：http://fk.szsharing.cn

set -euo pipefail
来源：http://vt.szsharing.cn

[R02] 变量赋值与使用
来源：http://ti.521024.cn

name="Tom"; echo "$name"
来源：http://yv.521024.cn

[R03] 只读变量
来源：http://fk.jctech888.com.cn

readonly PI=3.14
来源：http://lq.jctech888.com.cn

[R04] 位置参数
来源：http://ln.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ga.lnxyls.cn

[R05] 参数默认值
来源：http://my.haigaiapp.cn

name="${1:-default}"
来源：http://hr.hnjuh.cn

[R06] 判断命令是否存在
来源：http://fz.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pd.521024.cn

[R07] if 判断文件
来源：http://ii.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lv.huanxung.cn

[R08] 数值比较
来源：http://mn.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wp.panjiajie.cn

[R09] 字符串比较
来源：http://xn.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sy.szsharing.cn

[R10] 正则匹配
来源：http://we.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gt.shtwfgs.cn

[R11] case 多分支
来源：http://em.shxzskj.cn

case "$1" in
来源：http://qa.haigaiapp.cn

start) echo "启动" ;;
来源：http://fv.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://nx.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://nh.asd995.cn

esac
来源：http://vx.colortex.cn

[R12] for 遍历文件
来源：http://pz.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://hl.jianghongdianzi.cn

[R13] for 计数循环
来源：http://zz.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://qg.hahajie.cn

[R14] C 风格 for
来源：http://fu.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hq.shxzukj.cn

[R15] while 逐行读文件
来源：http://fm.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tv.521024.cn

[R16] until 等待条件
来源：http://gf.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eb.colortex.cn

[R17] 数组定义与取值
来源：http://vo.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qu.wgjwhj.cn

[R18] 遍历数组
来源：http://nk.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oo.shxzskj.cn

[R19] 数组长度
来源：http://gq.wgjwhj.cn

echo "${#arr[@]}"
来源：http://ds.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://re.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zq.yuexingan06.cn

[R21] 字符串长度
来源：http://tl.muxihuayi.cn

echo "${#s}"
来源：http://kx.muxihuayi.cn

[R22] 截取子串
来源：http://vj.bookmarksfly.cn

echo "${s:0:5}"
来源：http://de.lnxyls.cn

[R23] 字符串替换
来源：http://tj.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ze.521024.cn

[R24] 大小写转换
来源：http://gu.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mb.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://lw.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ko.9csxet.cn

[R26] 命令替换
来源：http://cr.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://ja.huixiangedu.cn

[R27] 算术展开
来源：http://ui.hahajie.cn

echo $((1 + 2 * 3))
来源：http://al.9csxet.cn

[R28] 浮点运算
来源：http://gt.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://ey.jianghongdianzi.cn

[R29] 定义函数
来源：http://md.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cz.chemitech.net.cn

[R30] 函数返回状态码
来源：http://td.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://pn.lnxyls.cn

[R31] 局部变量
来源：http://ue.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://jc.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://cn.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jb.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://ok.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xs.hahajie.cn

[R34] 退出时清理
来源：http://sj.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bg.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://hm.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xh.lnxyls.cn

[R36] 并发执行多个任务
来源：http://nw.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cg.huanxung.cn

[R37] 把输出赋给变量
来源：http://vz.jianghongdianzi.cn

files=$(ls -1)
来源：http://dg.bookmarksfly.cn

[R38] 管道串联
来源：http://rx.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://yq.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://vh.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://kw.newstarts.cn

[R40] 追加写日志
来源：http://jw.colortex.cn

echo "log" >> out.log
来源：http://ez.huixiangedu.cn

[R41] 丢弃输出
来源：http://zp.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://fr.szsharing.cn

[R42] 输入重定向
来源：http://lo.szsharing.cn

wc -l < a.txt
来源：http://uq.gzmigu.cn

[R43] 按名字查找文件
来源：http://bo.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://ut.hahajie.cn

[R44] 按修改时间查找
来源：http://qs.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://mi.nszjky.cn

[R45] 批量删除
来源：http://zh.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://mz.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://ty.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://od.9csxet.cn

[R47] sed 单行替换
来源：http://cb.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://su.newstarts.cn

[R48] awk 取指定列
来源：http://sl.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://ad.huixinmuqiang.cn

[R49] awk 带条件
来源：http://sj.shtwfgs.cn


<!-- 参考信息 -->