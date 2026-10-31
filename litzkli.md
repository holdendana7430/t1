代发 wailian999

CREATE TABLE users (
来源：http://nx.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eo.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://hv.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://az.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wd.bjjhwx.cn

);
来源：http://ds.521024.cn

[Q02] 创建带外键的表
来源：http://pb.9csxet.cn

CREATE TABLE orders (
来源：http://oj.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ok.huixiangedu.cn

user_id INT NOT NULL,
来源：http://zx.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://np.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fl.hahajie.cn

);
来源：http://fc.bookmarksfly.cn

[Q03] 增加列
来源：http://jz.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ku.szsharing.cn

[Q04] 修改列类型
来源：http://qk.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lp.wgjwhj.cn

[Q05] 重命名列
来源：http://tp.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ip.szxytkj.cn

[Q06] 删除列
来源：http://aa.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dx.shxzukj.cn

[Q07] 删除表
来源：http://un.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://fj.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://wf.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pz.newstarts.cn

[Q09] 创建唯一索引
来源：http://lf.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ll.chemitech.net.cn

[Q10] 插入单行
来源：http://mi.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nf.huixiangedu.cn

[Q11] 一次插入多行
来源：http://ox.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yl.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://tl.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eg.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vk.huanxung.cn

[Q13] 忽略重复插入
来源：http://bd.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mg.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://nh.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xh.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://id.nszjky.cn

[Q15] 查询全部
来源：http://mq.szsharing.cn

SELECT * FROM users;
来源：http://id.chemitech.net.cn

[Q16] 查询指定列
来源：http://aa.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://zv.colortex.cn

[Q17] 条件查询
来源：http://dq.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ho.521024.cn

[Q18] 模糊匹配
来源：http://rv.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ub.shtwfgs.cn

[Q19] 范围查询
来源：http://rp.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ti.colortex.cn

[Q20] IN 列表
来源：http://et.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bx.wgjwhj.cn

[Q21] 空值判断
来源：http://po.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xb.nicolike.cn

[Q22] 排序
来源：http://hi.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://in.huanxung.cn

[Q23] 分页
来源：http://ap.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oq.521024.cn

[Q24] 去重
来源：http://jt.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://iu.huanxung.cn

[Q25] 只取前 N 条
来源：http://ur.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kt.szxytkj.cn

[Q26] 计数
来源：http://cj.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://fv.shxzukj.cn

[Q27] 条件计数
来源：http://mu.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vq.yuexingan06.cn

[Q28] 求和与平均
来源：http://jf.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aq.hnjuh.cn

[Q29] 最大最小值
来源：http://xx.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kb.colortex.cn

[Q30] 分组统计
来源：http://ra.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jy.nicolike.cn

[Q31] 分组后过滤
来源：http://re.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xi.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://bl.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bb.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bd.yuntaijiaju.cn

[Q33] 多列分组
来源：http://pa.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gi.shxzskj.cn

[Q34] 每组取第一条
来源：http://ix.shxzskj.cn

SELECT * FROM (
来源：http://cp.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://up.nszjky.cn

) t WHERE rn = 1;
来源：http://mi.colortex.cn

[Q35] 内连接
来源：http://ja.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pj.lnxyls.cn

[Q36] 左连接
来源：http://xw.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wv.muxihuayi.cn

[Q37] 右连接
来源：http://fy.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nq.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dd.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mr.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://za.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qa.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gk.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ev.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bq.szxytkj.cn

[Q41] 多表连接
来源：http://yy.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fm.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://xh.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://jq.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://dw.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://uq.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pm.wgjwhj.cn

[Q43] 标量子查询
来源：http://dq.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ct.huanxung.cn

[Q44] IN 子查询
来源：http://ye.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oi.szxytkj.cn

[Q45] EXISTS 判断存在
来源：http://el.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ur.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wm.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nv.bjjhwx.cn

[Q47] 与平均值比较
来源：http://ig.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rf.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://mi.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xn.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://qo.haigaiapp.cn

[Q49] 更新单行
来源：http://ad.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://af.jianghongdianzi.cn

[Q50] 批量更新
来源：http://dy.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ne.asd995.cn

[Q51] 用子查询更新
来源：http://xo.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ie.szsharing.cn

[Q52] 删除指定行
来源：http://kh.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://rq.huixiangedu.cn

[Q53] 按条件删除
来源：http://of.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jp.szsharing.cn

[Q54] 清空表
来源：http://ux.newstarts.cn

TRUNCATE TABLE logs;
来源：http://tg.colortex.cn

[Q55] 排名（并列占位）
来源：http://tb.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xp.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://vt.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hi.9csxet.cn

[Q57] 行号
来源：http://mj.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xw.muxihuayi.cn

[Q58] 累计求和
来源：http://un.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://or.bjjhwx.cn

[Q59] 分组内累计
来源：http://em.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fy.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://kg.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ol.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bm.hahajie.cn

[Q61] 移动平均
来源：http://pk.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ip.haigaiapp.cn

[Q62] 分组占比
来源：http://yg.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hx.huixinmuqiang.cn

[Q63] 开启事务
来源：http://mm.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zr.chemitech.net.cn

[Q64] 提交事务
来源：http://mu.hnjuh.cn

COMMIT;
来源：http://ou.bookmarksfly.cn

[Q65] 回滚事务
来源：http://xq.haigaiapp.cn

ROLLBACK;
来源：http://hb.bookmarksfly.cn

[Q66] 行锁查询
来源：http://df.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hb.asd995.cn

[Q67] 设置隔离级别
来源：http://lr.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ty.haigaiapp.cn

[Q68] 保存点
来源：http://fd.521024.cn

SAVEPOINT sp1;
来源：http://le.szxytkj.cn

ROLLBACK TO sp1;
来源：http://fn.nszjky.cn

[Q69] 查看执行计划
来源：http://in.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vz.shxzukj.cn

[Q70] 更新统计信息
来源：http://hk.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://wm.haigaiapp.cn

[Q71] 查看建表语句
来源：http://cn.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ov.newstarts.cn

[Q72] 查看索引
来源：http://sf.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://bj.asd995.cn

[Q73] 查看表状态
来源：http://kj.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ek.nicolike.cn

[Q74] 强制使用索引
来源：http://og.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vh.gzmigu.cn

[Q75] 日期格式化
来源：http://sj.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gq.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tp.huanxung.cn

[Q76] 按天统计
来源：http://mo.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lo.bookmarksfly.cn

[Q77] 时间加减
来源：http://zf.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rj.bjjhwx.cn

[Q78] 当前时间
来源：http://qm.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jz.gzmigu.cn

[Q79] 字符串拼接
来源：http://fp.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uz.bjjhwx.cn

[Q80] 字符串截取
来源：http://dk.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lv.shtwfgs.cn

[Q81] 字符串替换
来源：http://hx.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bz.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://yd.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://op.shxzukj.cn

[Q83] 大小写转换
来源：http://lv.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sn.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://gv.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://vr.wgjwhj.cn

[Q85] 数值取整
来源：http://wh.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ef.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://mf.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sy.huanxung.cn

[Q87] JSON 字段做条件
来源：http://ap.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sw.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://na.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://on.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ee.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://aa.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lp.szsharing.cn

[Q90] 生成序号列
来源：http://uz.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dy.haigaiapp.cn

================================================================================
来源：http://iq.huixiangedu.cn

R. Bash 专题
来源：http://te.panjiajie.cn

================================================================================
来源：http://sr.colortex.cn

[R01] shebang 与严格模式
来源：http://lt.haigaiapp.cn

#!/usr/bin/env bash
来源：http://ao.shtwfgs.cn

set -euo pipefail
来源：http://ip.nszjky.cn

[R02] 变量赋值与使用
来源：http://bs.shxzukj.cn

name="Tom"; echo "$name"
来源：http://ch.muxihuayi.cn

[R03] 只读变量
来源：http://bi.shxzukj.cn

readonly PI=3.14
来源：http://li.bookmarksfly.cn

[R04] 位置参数
来源：http://fc.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cx.shxzukj.cn

[R05] 参数默认值
来源：http://qt.huanxung.cn

name="${1:-default}"
来源：http://mq.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://dl.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gw.jianghongdianzi.cn

[R07] if 判断文件
来源：http://rz.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ou.bookmarksfly.cn

[R08] 数值比较
来源：http://wl.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bs.newstarts.cn

[R09] 字符串比较
来源：http://ae.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cf.chemitech.net.cn

[R10] 正则匹配
来源：http://sm.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zv.shxzskj.cn

[R11] case 多分支
来源：http://vm.shxzukj.cn

case "$1" in
来源：http://qs.bookmarksfly.cn

start) echo "启动" ;;
来源：http://ip.gzmigu.cn

stop)  echo "停止" ;;
来源：http://bi.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://ri.yuexingan06.cn

esac
来源：http://oq.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://hs.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://xs.nicolike.cn

[R13] for 计数循环
来源：http://eu.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://lo.jianghongdianzi.cn

[R14] C 风格 for
来源：http://ir.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ep.bjjhwx.cn

[R15] while 逐行读文件
来源：http://rh.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ip.huanxung.cn

[R16] until 等待条件
来源：http://ht.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ds.huanxung.cn

[R17] 数组定义与取值
来源：http://az.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yz.nicolike.cn

[R18] 遍历数组
来源：http://xq.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://se.wgjwhj.cn

[R19] 数组长度
来源：http://dy.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://ds.newstarts.cn

[R20] 关联数组（字典）
来源：http://gg.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vn.haigaiapp.cn

[R21] 字符串长度
来源：http://ig.bjjhwx.cn

echo "${#s}"
来源：http://ei.bjjhwx.cn

[R22] 截取子串
来源：http://in.hahajie.cn

echo "${s:0:5}"
来源：http://qu.szxytkj.cn

[R23] 字符串替换
来源：http://oe.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fr.yuntaijiaju.cn

[R24] 大小写转换
来源：http://we.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gu.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://ju.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://al.haigaiapp.cn

[R26] 命令替换
来源：http://wc.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://zq.huixinmuqiang.cn

[R27] 算术展开
来源：http://bs.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://af.shxzskj.cn

[R28] 浮点运算
来源：http://ao.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://cu.gzmigu.cn

[R29] 定义函数
来源：http://aw.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dz.shtwfgs.cn

[R30] 函数返回状态码
来源：http://jy.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://kw.panjiajie.cn

[R31] 局部变量
来源：http://sh.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://ki.jctech888.com.cn

[R32] 参数个数校验
来源：http://nx.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kz.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://os.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://em.huixiangedu.cn

[R34] 退出时清理
来源：http://zx.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wa.shxzskj.cn

[R35] 后台执行并等待
来源：http://yg.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jz.521024.cn

[R36] 并发执行多个任务
来源：http://gi.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://he.asd995.cn

[R37] 把输出赋给变量
来源：http://tl.huanxung.cn

files=$(ls -1)
来源：http://gb.wgjwhj.cn

[R38] 管道串联
来源：http://hh.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://ym.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://jr.hnjuh.cn

cmd > out.log 2>&1
来源：http://lm.shxzukj.cn

[R40] 追加写日志
来源：http://oh.panjiajie.cn

echo "log" >> out.log
来源：http://kr.bookmarksfly.cn

[R41] 丢弃输出
来源：http://am.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://jt.huixinmuqiang.cn

[R42] 输入重定向
来源：http://bq.szsharing.cn

wc -l < a.txt
来源：http://qw.panjiajie.cn

[R43] 按名字查找文件
来源：http://jc.lnxyls.cn

find . -name "*.log" -type f
来源：http://oj.jctech888.com.cn

[R44] 按修改时间查找
来源：http://ff.colortex.cn

find . -mtime -7 -type f
来源：http://xv.wgjwhj.cn

[R45] 批量删除
来源：http://ij.haigaiapp.cn


<!-- 参考信息 -->