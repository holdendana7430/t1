代发 wailian999

CREATE TABLE users (
来源：http://gh.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://be.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://md.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://vu.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qj.wgjwhj.cn

);
来源：http://gf.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://vv.huixiangedu.cn

CREATE TABLE orders (
来源：http://py.shxzukj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sn.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://ys.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://lx.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cx.yuntaijiaju.cn

);
来源：http://jc.huixiangedu.cn

[Q03] 增加列
来源：http://ry.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://in.gzmigu.cn

[Q04] 修改列类型
来源：http://wj.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ti.bjjhwx.cn

[Q05] 重命名列
来源：http://hb.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rh.muxihuayi.cn

[Q06] 删除列
来源：http://hr.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vp.haigaiapp.cn

[Q07] 删除表
来源：http://qe.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://lo.lnxyls.cn

[Q08] 创建普通索引
来源：http://wk.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uv.gzmigu.cn

[Q09] 创建唯一索引
来源：http://eq.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://un.asd995.cn

[Q10] 插入单行
来源：http://sk.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ch.muxihuayi.cn

[Q11] 一次插入多行
来源：http://pt.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yv.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://cw.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vl.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://el.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://vh.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vl.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://yl.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dq.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://af.hnjuh.cn

[Q15] 查询全部
来源：http://lx.bjjhwx.cn

SELECT * FROM users;
来源：http://wi.jctech888.com.cn

[Q16] 查询指定列
来源：http://sj.newstarts.cn

SELECT id, name FROM users;
来源：http://ck.jianghongdianzi.cn

[Q17] 条件查询
来源：http://hw.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qy.jctech888.com.cn

[Q18] 模糊匹配
来源：http://ua.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lv.shtwfgs.cn

[Q19] 范围查询
来源：http://aq.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rp.bjjhwx.cn

[Q20] IN 列表
来源：http://bx.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bn.bjjhwx.cn

[Q21] 空值判断
来源：http://zw.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kr.nicolike.cn

[Q22] 排序
来源：http://nr.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jx.nicolike.cn

[Q23] 分页
来源：http://ok.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bh.nszjky.cn

[Q24] 去重
来源：http://ml.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://mj.9csxet.cn

[Q25] 只取前 N 条
来源：http://ge.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cy.shxzukj.cn

[Q26] 计数
来源：http://fi.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://mz.chemitech.net.cn

[Q27] 条件计数
来源：http://ne.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hf.lnxyls.cn

[Q28] 求和与平均
来源：http://wj.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lq.szxytkj.cn

[Q29] 最大最小值
来源：http://ff.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://be.9csxet.cn

[Q30] 分组统计
来源：http://ia.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zg.szxytkj.cn

[Q31] 分组后过滤
来源：http://ec.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kb.szsharing.cn

[Q32] 分组拼接字符串
来源：http://ef.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fl.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hk.panjiajie.cn

[Q33] 多列分组
来源：http://yq.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xd.bjjhwx.cn

[Q34] 每组取第一条
来源：http://ka.gzmigu.cn

SELECT * FROM (
来源：http://ns.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gc.hnjuh.cn

) t WHERE rn = 1;
来源：http://wy.9csxet.cn

[Q35] 内连接
来源：http://hc.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cl.szsharing.cn

[Q36] 左连接
来源：http://gb.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bp.bookmarksfly.cn

[Q37] 右连接
来源：http://mz.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ns.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://il.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ac.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://fq.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wv.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://er.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ma.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mx.lnxyls.cn

[Q41] 多表连接
来源：http://if.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tn.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://lr.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://yh.colortex.cn

[Q42] 连接条件附加过滤
来源：http://if.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://vs.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ya.huanxung.cn

[Q43] 标量子查询
来源：http://zw.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hm.shtwfgs.cn

[Q44] IN 子查询
来源：http://bf.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ko.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://qm.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rm.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://el.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cc.jctech888.com.cn

[Q47] 与平均值比较
来源：http://jt.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eb.asd995.cn

[Q48] CTE 公用表表达式
来源：http://wv.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zh.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://oa.nszjky.cn

[Q49] 更新单行
来源：http://xm.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zp.huixiangedu.cn

[Q50] 批量更新
来源：http://ur.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yn.521024.cn

[Q51] 用子查询更新
来源：http://ej.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uu.gzmigu.cn

[Q52] 删除指定行
来源：http://ad.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://ep.muxihuayi.cn

[Q53] 按条件删除
来源：http://uu.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://is.gzmigu.cn

[Q54] 清空表
来源：http://rt.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://wd.hahajie.cn

[Q55] 排名（并列占位）
来源：http://ku.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ll.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://yf.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ih.521024.cn

[Q57] 行号
来源：http://uh.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jq.shtwfgs.cn

[Q58] 累计求和
来源：http://dl.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rn.nszjky.cn

[Q59] 分组内累计
来源：http://sn.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wj.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://oq.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ga.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ts.yuexingan06.cn

[Q61] 移动平均
来源：http://ov.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ht.lnxyls.cn

[Q62] 分组占比
来源：http://hd.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://br.521024.cn

[Q63] 开启事务
来源：http://pd.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rc.asd995.cn

[Q64] 提交事务
来源：http://uc.jctech888.com.cn

COMMIT;
来源：http://rg.yuexingan06.cn

[Q65] 回滚事务
来源：http://xu.bjjhwx.cn

ROLLBACK;
来源：http://xf.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://ck.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://as.nszjky.cn

[Q67] 设置隔离级别
来源：http://aw.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bg.yuexingan06.cn

[Q68] 保存点
来源：http://cj.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://yk.nicolike.cn

ROLLBACK TO sp1;
来源：http://ya.nicolike.cn

[Q69] 查看执行计划
来源：http://od.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vn.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://eu.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://hn.haigaiapp.cn

[Q71] 查看建表语句
来源：http://qq.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pt.shxzskj.cn

[Q72] 查看索引
来源：http://cw.panjiajie.cn

SHOW INDEX FROM users;
来源：http://pn.newstarts.cn

[Q73] 查看表状态
来源：http://up.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yy.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://ld.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cr.9csxet.cn

[Q75] 日期格式化
来源：http://et.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xa.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://im.asd995.cn

[Q76] 按天统计
来源：http://tg.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qz.wgjwhj.cn

[Q77] 时间加减
来源：http://il.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ld.shtwfgs.cn

[Q78] 当前时间
来源：http://qk.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bg.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://tv.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ne.shxzukj.cn

[Q80] 字符串截取
来源：http://dl.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gu.wgjwhj.cn

[Q81] 字符串替换
来源：http://ma.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kp.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://vo.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bu.bookmarksfly.cn

[Q83] 大小写转换
来源：http://yf.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ee.nszjky.cn

[Q84] 去除首尾空格
来源：http://sl.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://fg.shtwfgs.cn

[Q85] 数值取整
来源：http://yf.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kp.colortex.cn

[Q86] 读取 JSON 字段
来源：http://dq.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uh.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://dv.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xd.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://bx.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yx.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bh.newstarts.cn

[Q89] 判断表是否存在
来源：http://xk.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rt.shxzukj.cn

[Q90] 生成序号列
来源：http://ls.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wj.bookmarksfly.cn

================================================================================
来源：http://is.szsharing.cn

R. Bash 专题
来源：http://ib.nszjky.cn

================================================================================
来源：http://ld.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://nr.colortex.cn

#!/usr/bin/env bash
来源：http://iv.hnjuh.cn

set -euo pipefail
来源：http://vp.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://xa.9csxet.cn

name="Tom"; echo "$name"
来源：http://ml.gzmigu.cn

[R03] 只读变量
来源：http://pi.huixinmuqiang.cn

readonly PI=3.14
来源：http://tw.asd995.cn

[R04] 位置参数
来源：http://st.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hg.colortex.cn

[R05] 参数默认值
来源：http://to.shxzukj.cn

name="${1:-default}"
来源：http://de.521024.cn

[R06] 判断命令是否存在
来源：http://oc.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jl.shxzukj.cn

[R07] if 判断文件
来源：http://eb.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rr.newstarts.cn

[R08] 数值比较
来源：http://om.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://re.yuexingan06.cn

[R09] 字符串比较
来源：http://wx.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lu.newstarts.cn

[R10] 正则匹配
来源：http://vu.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://on.newstarts.cn

[R11] case 多分支
来源：http://qe.shxzukj.cn

case "$1" in
来源：http://zz.shxzukj.cn

start) echo "启动" ;;
来源：http://se.nicolike.cn

stop)  echo "停止" ;;
来源：http://ln.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://gb.shtwfgs.cn

esac
来源：http://so.bookmarksfly.cn

[R12] for 遍历文件
来源：http://hm.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://ay.chemitech.net.cn

[R13] for 计数循环
来源：http://cu.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://vh.szsharing.cn

[R14] C 风格 for
来源：http://di.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dk.jctech888.com.cn

[R15] while 逐行读文件
来源：http://ur.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iy.yuntaijiaju.cn

[R16] until 等待条件
来源：http://vy.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nj.nicolike.cn

[R17] 数组定义与取值
来源：http://hw.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pu.muxihuayi.cn

[R18] 遍历数组
来源：http://ca.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rh.shtwfgs.cn

[R19] 数组长度
来源：http://fn.shxzukj.cn

echo "${#arr[@]}"
来源：http://ef.panjiajie.cn

[R20] 关联数组（字典）
来源：http://jn.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tq.shxzukj.cn

[R21] 字符串长度
来源：http://fl.shtwfgs.cn

echo "${#s}"
来源：http://iu.colortex.cn

[R22] 截取子串
来源：http://ti.szxytkj.cn

echo "${s:0:5}"
来源：http://cj.lnxyls.cn

[R23] 字符串替换
来源：http://bh.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qv.nszjky.cn

[R24] 大小写转换
来源：http://eq.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pj.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://ez.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iu.szsharing.cn

[R26] 命令替换
来源：http://tz.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://ea.newstarts.cn

[R27] 算术展开
来源：http://jc.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://os.huixinmuqiang.cn

[R28] 浮点运算
来源：http://vz.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://ew.panjiajie.cn

[R29] 定义函数
来源：http://uy.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iq.9csxet.cn

[R30] 函数返回状态码
来源：http://oq.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://cf.9csxet.cn

[R31] 局部变量
来源：http://qs.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://dl.wgjwhj.cn

[R32] 参数个数校验
来源：http://xd.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nm.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://jc.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dw.muxihuayi.cn

[R34] 退出时清理
来源：http://hm.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fg.colortex.cn

[R35] 后台执行并等待
来源：http://tm.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kb.szsharing.cn

[R36] 并发执行多个任务
来源：http://ce.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rc.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://dv.shxzukj.cn

files=$(ls -1)
来源：http://we.huixinmuqiang.cn

[R38] 管道串联
来源：http://bc.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://jy.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://xc.nicolike.cn

cmd > out.log 2>&1
来源：http://wu.muxihuayi.cn

[R40] 追加写日志
来源：http://fa.yuexingan06.cn

echo "log" >> out.log
来源：http://qs.shxzskj.cn

[R41] 丢弃输出
来源：http://yc.nszjky.cn

cmd >/dev/null 2>&1
来源：http://hq.wgjwhj.cn

[R42] 输入重定向
来源：http://oc.lnxyls.cn

wc -l < a.txt
来源：http://rt.haigaiapp.cn

[R43] 按名字查找文件
来源：http://pc.shxzukj.cn

find . -name "*.log" -type f
来源：http://xi.nicolike.cn

[R44] 按修改时间查找
来源：http://wk.newstarts.cn

find . -mtime -7 -type f
来源：http://tn.nszjky.cn

[R45] 批量删除
来源：http://cy.huixinmuqiang.cn


<!-- 参考信息 -->