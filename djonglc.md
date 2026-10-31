代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://fx.shtwfgs.cn

[Q07] 删除表
来源：http://ot.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://ag.shxzskj.cn

[Q08] 创建普通索引
来源：http://nr.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xw.huanxung.cn

[Q09] 创建唯一索引
来源：http://vn.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://un.wgjwhj.cn

[Q10] 插入单行
来源：http://no.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zd.panjiajie.cn

[Q11] 一次插入多行
来源：http://jk.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://va.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://iz.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gt.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ax.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://qc.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gv.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://jd.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vc.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ep.nicolike.cn

[Q15] 查询全部
来源：http://iw.nicolike.cn

SELECT * FROM users;
来源：http://yk.muxihuayi.cn

[Q16] 查询指定列
来源：http://sn.newstarts.cn

SELECT id, name FROM users;
来源：http://ph.hnjuh.cn

[Q17] 条件查询
来源：http://lj.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pn.nicolike.cn

[Q18] 模糊匹配
来源：http://km.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kb.hahajie.cn

[Q19] 范围查询
来源：http://mg.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ul.yuntaijiaju.cn

[Q20] IN 列表
来源：http://en.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://in.colortex.cn

[Q21] 空值判断
来源：http://uw.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zc.muxihuayi.cn

[Q22] 排序
来源：http://kb.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://an.chemitech.net.cn

[Q23] 分页
来源：http://hg.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zz.huanxung.cn

[Q24] 去重
来源：http://qr.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://ti.hahajie.cn

[Q25] 只取前 N 条
来源：http://wp.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ku.shxzskj.cn

[Q26] 计数
来源：http://yi.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://nj.asd995.cn

[Q27] 条件计数
来源：http://xr.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dk.colortex.cn

[Q28] 求和与平均
来源：http://vw.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lm.9csxet.cn

[Q29] 最大最小值
来源：http://df.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nz.hnjuh.cn

[Q30] 分组统计
来源：http://aj.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ag.gzmigu.cn

[Q31] 分组后过滤
来源：http://iq.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mm.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://di.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cb.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zy.hahajie.cn

[Q33] 多列分组
来源：http://hx.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aj.chemitech.net.cn

[Q34] 每组取第一条
来源：http://ur.bookmarksfly.cn

SELECT * FROM (
来源：http://dd.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xu.haigaiapp.cn

) t WHERE rn = 1;
来源：http://gv.yuexingan06.cn

[Q35] 内连接
来源：http://zz.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://os.hahajie.cn

[Q36] 左连接
来源：http://ze.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ms.521024.cn

[Q37] 右连接
来源：http://el.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zb.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ma.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ab.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://cq.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ot.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lj.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yx.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jh.newstarts.cn

[Q41] 多表连接
来源：http://ql.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xr.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://sn.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://ct.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://sg.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://ei.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://td.chemitech.net.cn

[Q43] 标量子查询
来源：http://on.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cp.szsharing.cn

[Q44] IN 子查询
来源：http://ys.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kg.asd995.cn

[Q45] EXISTS 判断存在
来源：http://ty.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kq.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ix.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ht.hahajie.cn

[Q47] 与平均值比较
来源：http://ui.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gl.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://xf.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://de.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://vf.yuntaijiaju.cn

[Q49] 更新单行
来源：http://nf.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vj.shxzukj.cn

[Q50] 批量更新
来源：http://ma.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mk.chemitech.net.cn

[Q51] 用子查询更新
来源：http://qw.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mh.521024.cn

[Q52] 删除指定行
来源：http://qm.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://xt.hahajie.cn

[Q53] 按条件删除
来源：http://va.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rk.gzmigu.cn

[Q54] 清空表
来源：http://ul.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://rd.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://kh.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qu.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://ry.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cs.asd995.cn

[Q57] 行号
来源：http://ty.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nm.muxihuayi.cn

[Q58] 累计求和
来源：http://co.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://po.jctech888.com.cn

[Q59] 分组内累计
来源：http://fa.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pg.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://vc.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aj.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ny.chemitech.net.cn

[Q61] 移动平均
来源：http://pp.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fs.huixiangedu.cn

[Q62] 分组占比
来源：http://qa.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wx.asd995.cn

[Q63] 开启事务
来源：http://qq.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pi.haigaiapp.cn

[Q64] 提交事务
来源：http://kn.hahajie.cn

COMMIT;
来源：http://in.521024.cn

[Q65] 回滚事务
来源：http://pg.newstarts.cn

ROLLBACK;
来源：http://fr.bjjhwx.cn

[Q66] 行锁查询
来源：http://qc.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fl.newstarts.cn

[Q67] 设置隔离级别
来源：http://fy.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qd.521024.cn

[Q68] 保存点
来源：http://br.bjjhwx.cn

SAVEPOINT sp1;
来源：http://uo.hahajie.cn

ROLLBACK TO sp1;
来源：http://mb.shxzukj.cn

[Q69] 查看执行计划
来源：http://ih.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nw.wgjwhj.cn

[Q70] 更新统计信息
来源：http://sh.gzmigu.cn

ANALYZE TABLE users;
来源：http://pa.521024.cn

[Q71] 查看建表语句
来源：http://pf.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cj.jianghongdianzi.cn

[Q72] 查看索引
来源：http://hb.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://ro.huixiangedu.cn

[Q73] 查看表状态
来源：http://qo.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://or.wgjwhj.cn

[Q74] 强制使用索引
来源：http://ak.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dz.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://xk.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://at.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qa.shxzskj.cn

[Q76] 按天统计
来源：http://ol.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://le.shxzukj.cn

[Q77] 时间加减
来源：http://la.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mp.huanxung.cn

[Q78] 当前时间
来源：http://ld.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lr.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://sx.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cw.colortex.cn

[Q80] 字符串截取
来源：http://mu.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iy.bjjhwx.cn

[Q81] 字符串替换
来源：http://gf.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kf.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://pv.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://en.szxytkj.cn

[Q83] 大小写转换
来源：http://dc.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pu.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://wr.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://ad.yuexingan06.cn

[Q85] 数值取整
来源：http://oq.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yl.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://tx.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dd.asd995.cn

[Q87] JSON 字段做条件
来源：http://uu.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rw.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://kz.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bg.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wa.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://jc.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ho.wgjwhj.cn

[Q90] 生成序号列
来源：http://ja.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xj.shxzskj.cn

================================================================================
来源：http://dx.asd995.cn

R. Bash 专题
来源：http://ni.shxzukj.cn

================================================================================
来源：http://ek.hahajie.cn

[R01] shebang 与严格模式
来源：http://rd.szsharing.cn

#!/usr/bin/env bash
来源：http://ue.huanxung.cn

set -euo pipefail
来源：http://os.shxzukj.cn

[R02] 变量赋值与使用
来源：http://lk.szsharing.cn

name="Tom"; echo "$name"
来源：http://ox.asd995.cn

[R03] 只读变量
来源：http://zc.huanxung.cn

readonly PI=3.14
来源：http://no.shxzskj.cn

[R04] 位置参数
来源：http://zu.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ja.nszjky.cn

[R05] 参数默认值
来源：http://di.huixiangedu.cn

name="${1:-default}"
来源：http://ah.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://rq.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yq.nszjky.cn

[R07] if 判断文件
来源：http://nw.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fy.szxytkj.cn

[R08] 数值比较
来源：http://pc.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wi.yuntaijiaju.cn

[R09] 字符串比较
来源：http://el.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://of.nszjky.cn

[R10] 正则匹配
来源：http://vn.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nk.huanxung.cn

[R11] case 多分支
来源：http://es.asd995.cn

case "$1" in
来源：http://oj.szsharing.cn

start) echo "启动" ;;
来源：http://rs.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://td.asd995.cn

*)     echo "未知命令" ;;
来源：http://ez.gzmigu.cn

esac
来源：http://pn.haigaiapp.cn

[R12] for 遍历文件
来源：http://hp.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://tx.521024.cn

[R13] for 计数循环
来源：http://am.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://cy.shxzskj.cn

[R14] C 风格 for
来源：http://un.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dv.szxytkj.cn

[R15] while 逐行读文件
来源：http://kj.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ia.bookmarksfly.cn

[R16] until 等待条件
来源：http://yz.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tq.shxzskj.cn

[R17] 数组定义与取值
来源：http://ev.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mx.huanxung.cn

[R18] 遍历数组
来源：http://pl.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kt.panjiajie.cn

[R19] 数组长度
来源：http://av.muxihuayi.cn

echo "${#arr[@]}"
来源：http://qa.colortex.cn

[R20] 关联数组（字典）
来源：http://ff.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ra.asd995.cn

[R21] 字符串长度
来源：http://dy.hahajie.cn

echo "${#s}"
来源：http://dh.521024.cn

[R22] 截取子串
来源：http://ck.newstarts.cn

echo "${s:0:5}"
来源：http://ol.nszjky.cn

[R23] 字符串替换
来源：http://yu.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lf.yuexingan06.cn

[R24] 大小写转换
来源：http://pd.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zt.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://jk.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://us.nszjky.cn

[R26] 命令替换
来源：http://bh.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://dk.newstarts.cn

[R27] 算术展开
来源：http://jq.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://au.gzmigu.cn

[R28] 浮点运算
来源：http://ie.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://tj.hahajie.cn

[R29] 定义函数
来源：http://le.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yn.9csxet.cn

[R30] 函数返回状态码
来源：http://cu.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://qt.szsharing.cn

[R31] 局部变量
来源：http://jr.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://ay.asd995.cn

[R32] 参数个数校验
来源：http://pd.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sd.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://th.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ak.shxzukj.cn

[R34] 退出时清理
来源：http://wp.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zs.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://xo.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bz.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://jm.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bl.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://ff.lnxyls.cn

files=$(ls -1)
来源：http://hk.shtwfgs.cn

[R38] 管道串联
来源：http://ct.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://vm.521024.cn

[R39] 重定向标准输出与错误
来源：http://ox.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://pf.wgjwhj.cn

[R40] 追加写日志
来源：http://cw.wgjwhj.cn

echo "log" >> out.log
来源：http://uu.shxzskj.cn

[R41] 丢弃输出
来源：http://tq.9csxet.cn

cmd >/dev/null 2>&1
来源：http://vs.huanxung.cn

[R42] 输入重定向
来源：http://iy.bookmarksfly.cn

wc -l < a.txt
来源：http://pd.nicolike.cn

[R43] 按名字查找文件
来源：http://qk.szxytkj.cn

find . -name "*.log" -type f
来源：http://rz.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://pz.newstarts.cn

find . -mtime -7 -type f
来源：http://su.yuexingan06.cn

[R45] 批量删除
来源：http://kt.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://bk.9csxet.cn

[R46] 递归替换文件内容
来源：http://if.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jn.newstarts.cn

[R47] sed 单行替换
来源：http://fb.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jd.shxzukj.cn

[R48] awk 取指定列
来源：http://lg.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://kc.yuntaijiaju.cn

[R49] awk 带条件
来源：http://cf.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ry.yuntaijiaju.cn

[R50] awk 求和
来源：http://ys.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dn.bjjhwx.cn

[R51] 排序去重取前几
来源：http://hc.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bf.wgjwhj.cn

[R52] 统计行数
来源：http://ey.asd995.cn

wc -l a.txt
来源：http://tz.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://ka.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://od.newstarts.cn

[R54] 比较两个文件
来源：http://fv.huixiangedu.cn

diff a.txt b.txt
来源：http://ig.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://fv.haigaiapp.cn


<!-- 参考信息 -->