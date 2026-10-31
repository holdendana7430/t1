代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://zc.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qe.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fx.shtwfgs.cn

[Q15] 查询全部
来源：http://cc.hnjuh.cn

SELECT * FROM users;
来源：http://ox.nszjky.cn

[Q16] 查询指定列
来源：http://jo.colortex.cn

SELECT id, name FROM users;
来源：http://an.huixinmuqiang.cn

[Q17] 条件查询
来源：http://tw.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ym.shxzskj.cn

[Q18] 模糊匹配
来源：http://uf.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xj.shxzskj.cn

[Q19] 范围查询
来源：http://ie.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ei.bjjhwx.cn

[Q20] IN 列表
来源：http://qv.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yi.lnxyls.cn

[Q21] 空值判断
来源：http://we.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ro.szsharing.cn

[Q22] 排序
来源：http://yl.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cc.bookmarksfly.cn

[Q23] 分页
来源：http://as.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bq.huanxung.cn

[Q24] 去重
来源：http://sv.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://jy.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://bl.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wz.9csxet.cn

[Q26] 计数
来源：http://fl.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://zv.huanxung.cn

[Q27] 条件计数
来源：http://eq.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bu.chemitech.net.cn

[Q28] 求和与平均
来源：http://mo.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ti.shxzskj.cn

[Q29] 最大最小值
来源：http://rn.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xm.colortex.cn

[Q30] 分组统计
来源：http://au.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://op.haigaiapp.cn

[Q31] 分组后过滤
来源：http://kb.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iz.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://mm.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://on.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wt.panjiajie.cn

[Q33] 多列分组
来源：http://hr.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hs.newstarts.cn

[Q34] 每组取第一条
来源：http://qy.jctech888.com.cn

SELECT * FROM (
来源：http://gu.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sm.szsharing.cn

) t WHERE rn = 1;
来源：http://xr.colortex.cn

[Q35] 内连接
来源：http://ky.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hq.yuntaijiaju.cn

[Q36] 左连接
来源：http://nu.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dn.lnxyls.cn

[Q37] 右连接
来源：http://se.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pz.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ap.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nh.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://eo.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://am.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bj.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uc.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vu.521024.cn

[Q41] 多表连接
来源：http://lg.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://as.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://qc.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://gz.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://in.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://vg.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vx.9csxet.cn

[Q43] 标量子查询
来源：http://ev.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ng.shtwfgs.cn

[Q44] IN 子查询
来源：http://ei.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mv.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://nv.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ar.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qk.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xk.bjjhwx.cn

[Q47] 与平均值比较
来源：http://kk.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iw.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://md.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ij.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://no.bookmarksfly.cn

[Q49] 更新单行
来源：http://ti.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://an.szxytkj.cn

[Q50] 批量更新
来源：http://cl.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fr.yuexingan06.cn

[Q51] 用子查询更新
来源：http://xo.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lp.9csxet.cn

[Q52] 删除指定行
来源：http://bm.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://yx.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://dq.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ps.muxihuayi.cn

[Q54] 清空表
来源：http://im.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://mp.huanxung.cn

[Q55] 排名（并列占位）
来源：http://ly.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vj.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://hy.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wy.huixiangedu.cn

[Q57] 行号
来源：http://uq.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rq.gzmigu.cn

[Q58] 累计求和
来源：http://ax.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gf.chemitech.net.cn

[Q59] 分组内累计
来源：http://ry.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://it.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://mt.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mu.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wk.huixinmuqiang.cn

[Q61] 移动平均
来源：http://hy.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sn.haigaiapp.cn

[Q62] 分组占比
来源：http://mw.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zo.nszjky.cn

[Q63] 开启事务
来源：http://xx.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tq.asd995.cn

[Q64] 提交事务
来源：http://zi.muxihuayi.cn

COMMIT;
来源：http://id.nszjky.cn

[Q65] 回滚事务
来源：http://ev.gzmigu.cn

ROLLBACK;
来源：http://ql.newstarts.cn

[Q66] 行锁查询
来源：http://of.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qj.gzmigu.cn

[Q67] 设置隔离级别
来源：http://rv.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sf.hahajie.cn

[Q68] 保存点
来源：http://is.huixiangedu.cn

SAVEPOINT sp1;
来源：http://aq.szxytkj.cn

ROLLBACK TO sp1;
来源：http://ab.gzmigu.cn

[Q69] 查看执行计划
来源：http://cu.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fg.shxzukj.cn

[Q70] 更新统计信息
来源：http://or.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://qz.bjjhwx.cn

[Q71] 查看建表语句
来源：http://co.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://il.szsharing.cn

[Q72] 查看索引
来源：http://ha.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://ew.shtwfgs.cn

[Q73] 查看表状态
来源：http://to.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://is.panjiajie.cn

[Q74] 强制使用索引
来源：http://ew.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vi.nicolike.cn

[Q75] 日期格式化
来源：http://sz.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yq.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gu.shxzskj.cn

[Q76] 按天统计
来源：http://cf.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pi.bookmarksfly.cn

[Q77] 时间加减
来源：http://ih.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tl.haigaiapp.cn

[Q78] 当前时间
来源：http://ok.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://my.shxzukj.cn

[Q79] 字符串拼接
来源：http://bo.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gw.nicolike.cn

[Q80] 字符串截取
来源：http://bt.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qc.panjiajie.cn

[Q81] 字符串替换
来源：http://hx.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://np.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://pa.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ss.asd995.cn

[Q83] 大小写转换
来源：http://rl.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ws.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://fr.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://si.lnxyls.cn

[Q85] 数值取整
来源：http://xf.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mg.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://bf.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rp.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://os.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ki.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://kx.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://no.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qs.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://ki.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://td.haigaiapp.cn

[Q90] 生成序号列
来源：http://ek.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zi.szsharing.cn

================================================================================
来源：http://gc.521024.cn

R. Bash 专题
来源：http://ld.shxzukj.cn

================================================================================
来源：http://uu.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://oq.asd995.cn

#!/usr/bin/env bash
来源：http://oe.wgjwhj.cn

set -euo pipefail
来源：http://tj.gzmigu.cn

[R02] 变量赋值与使用
来源：http://ry.hahajie.cn

name="Tom"; echo "$name"
来源：http://ee.huixiangedu.cn

[R03] 只读变量
来源：http://hx.jctech888.com.cn

readonly PI=3.14
来源：http://bx.yuntaijiaju.cn

[R04] 位置参数
来源：http://hq.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gm.chemitech.net.cn

[R05] 参数默认值
来源：http://im.newstarts.cn

name="${1:-default}"
来源：http://hd.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://ut.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wa.9csxet.cn

[R07] if 判断文件
来源：http://ml.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yr.panjiajie.cn

[R08] 数值比较
来源：http://bs.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zp.nszjky.cn

[R09] 字符串比较
来源：http://oi.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zp.yuexingan06.cn

[R10] 正则匹配
来源：http://uy.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ye.nicolike.cn

[R11] case 多分支
来源：http://jk.nicolike.cn

case "$1" in
来源：http://mq.521024.cn

start) echo "启动" ;;
来源：http://hk.panjiajie.cn

stop)  echo "停止" ;;
来源：http://pu.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://dj.shxzskj.cn

esac
来源：http://bc.haigaiapp.cn

[R12] for 遍历文件
来源：http://hu.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://op.jianghongdianzi.cn

[R13] for 计数循环
来源：http://pm.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://wa.asd995.cn

[R14] C 风格 for
来源：http://kg.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://or.wgjwhj.cn

[R15] while 逐行读文件
来源：http://ni.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ht.shxzukj.cn

[R16] until 等待条件
来源：http://bl.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dv.nszjky.cn

[R17] 数组定义与取值
来源：http://wm.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sw.asd995.cn

[R18] 遍历数组
来源：http://xu.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mi.shxzukj.cn

[R19] 数组长度
来源：http://lt.panjiajie.cn

echo "${#arr[@]}"
来源：http://my.asd995.cn

[R20] 关联数组（字典）
来源：http://jj.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vp.bookmarksfly.cn

[R21] 字符串长度
来源：http://em.shxzukj.cn

echo "${#s}"
来源：http://dc.bookmarksfly.cn

[R22] 截取子串
来源：http://rp.nicolike.cn

echo "${s:0:5}"
来源：http://ng.jianghongdianzi.cn

[R23] 字符串替换
来源：http://ty.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://av.muxihuayi.cn

[R24] 大小写转换
来源：http://pi.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hw.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://pa.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ed.huixinmuqiang.cn

[R26] 命令替换
来源：http://mg.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://ew.huixinmuqiang.cn

[R27] 算术展开
来源：http://dp.newstarts.cn

echo $((1 + 2 * 3))
来源：http://ho.newstarts.cn

[R28] 浮点运算
来源：http://iz.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ya.huixiangedu.cn

[R29] 定义函数
来源：http://jv.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://os.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://kb.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://ra.muxihuayi.cn

[R31] 局部变量
来源：http://tj.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://yg.hahajie.cn

[R32] 参数个数校验
来源：http://iz.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zg.521024.cn

[R33] 捕获错误并提示行号
来源：http://hu.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kg.wgjwhj.cn

[R34] 退出时清理
来源：http://er.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cn.colortex.cn

[R35] 后台执行并等待
来源：http://ci.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cl.shxzskj.cn

[R36] 并发执行多个任务
来源：http://yr.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ab.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://hn.9csxet.cn

files=$(ls -1)
来源：http://pr.nicolike.cn

[R38] 管道串联
来源：http://rb.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://ou.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://rs.huanxung.cn

cmd > out.log 2>&1
来源：http://my.lnxyls.cn

[R40] 追加写日志
来源：http://jz.asd995.cn

echo "log" >> out.log
来源：http://lk.haigaiapp.cn

[R41] 丢弃输出
来源：http://bu.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://cb.huixiangedu.cn

[R42] 输入重定向
来源：http://tp.nicolike.cn

wc -l < a.txt
来源：http://ab.gzmigu.cn

[R43] 按名字查找文件
来源：http://ee.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://or.521024.cn

[R44] 按修改时间查找
来源：http://wr.9csxet.cn

find . -mtime -7 -type f
来源：http://qn.shtwfgs.cn

[R45] 批量删除
来源：http://qv.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://uy.huanxung.cn

[R46] 递归替换文件内容
来源：http://mk.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gj.szsharing.cn

[R47] sed 单行替换
来源：http://ve.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ul.wgjwhj.cn

[R48] awk 取指定列
来源：http://vm.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://xf.hnjuh.cn

[R49] awk 带条件
来源：http://rb.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jc.hnjuh.cn

[R50] awk 求和
来源：http://yv.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zo.szsharing.cn

[R51] 排序去重取前几
来源：http://xb.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gz.lnxyls.cn

[R52] 统计行数
来源：http://zy.bjjhwx.cn

wc -l a.txt
来源：http://jq.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://tz.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ld.lnxyls.cn

[R54] 比较两个文件
来源：http://sd.jctech888.com.cn

diff a.txt b.txt
来源：http://es.huanxung.cn

[R55] 压缩与解压
来源：http://rk.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://io.panjiajie.cn

[R56] 远程拷贝
来源：http://as.nicolike.cn

scp file user@host:/path/
来源：http://nr.9csxet.cn

[R57] 远程执行命令
来源：http://dl.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://uy.yuexingan06.cn

[R58] 下载文件
来源：http://xx.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dk.yuexingan06.cn

[R59] 发 POST JSON
来源：http://yg.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aj.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://pj.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iy.huanxung.cn

[R61] 磁盘占用
来源：http://bi.wgjwhj.cn

df -h;  du -sh *
来源：http://bd.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://ym.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://fc.bjjhwx.cn

[R63] 内存与进程
来源：http://lz.gzmigu.cn


<!-- 参考信息 -->