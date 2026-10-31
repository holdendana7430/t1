代发 wailian999

SELECT * FROM users;
来源：http://rr.lnxyls.cn

[Q16] 查询指定列
来源：http://ya.szxytkj.cn

SELECT id, name FROM users;
来源：http://lf.lnxyls.cn

[Q17] 条件查询
来源：http://oq.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iy.nicolike.cn

[Q18] 模糊匹配
来源：http://mc.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tk.bookmarksfly.cn

[Q19] 范围查询
来源：http://ti.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qt.lnxyls.cn

[Q20] IN 列表
来源：http://po.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pb.panjiajie.cn

[Q21] 空值判断
来源：http://pk.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://px.nszjky.cn

[Q22] 排序
来源：http://co.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ik.9csxet.cn

[Q23] 分页
来源：http://ei.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kh.huanxung.cn

[Q24] 去重
来源：http://rk.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://gb.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://io.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ci.9csxet.cn

[Q26] 计数
来源：http://co.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://je.muxihuayi.cn

[Q27] 条件计数
来源：http://wi.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hk.huixiangedu.cn

[Q28] 求和与平均
来源：http://bd.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rv.szsharing.cn

[Q29] 最大最小值
来源：http://kb.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ml.shxzukj.cn

[Q30] 分组统计
来源：http://wy.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vb.wgjwhj.cn

[Q31] 分组后过滤
来源：http://xa.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nv.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://cs.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rw.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pb.9csxet.cn

[Q33] 多列分组
来源：http://dq.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jn.huanxung.cn

[Q34] 每组取第一条
来源：http://hl.wgjwhj.cn

SELECT * FROM (
来源：http://rt.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kw.haigaiapp.cn

) t WHERE rn = 1;
来源：http://aa.nszjky.cn

[Q35] 内连接
来源：http://ez.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qp.muxihuayi.cn

[Q36] 左连接
来源：http://nm.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fx.newstarts.cn

[Q37] 右连接
来源：http://eu.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ej.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ty.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ub.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://ue.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ku.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://co.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://am.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ob.hnjuh.cn

[Q41] 多表连接
来源：http://je.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ve.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://jh.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://nz.521024.cn

[Q42] 连接条件附加过滤
来源：http://us.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://ge.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kk.muxihuayi.cn

[Q43] 标量子查询
来源：http://bs.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yx.szxytkj.cn

[Q44] IN 子查询
来源：http://is.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fj.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://hl.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ww.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ci.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bj.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://ze.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rx.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://cr.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iu.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://aq.muxihuayi.cn

[Q49] 更新单行
来源：http://nb.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ee.yuexingan06.cn

[Q50] 批量更新
来源：http://sm.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sr.hnjuh.cn

[Q51] 用子查询更新
来源：http://zz.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://he.huixiangedu.cn

[Q52] 删除指定行
来源：http://dq.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://to.jctech888.com.cn

[Q53] 按条件删除
来源：http://wp.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cs.nszjky.cn

[Q54] 清空表
来源：http://jx.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://hp.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://nn.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ls.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://if.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ip.yuexingan06.cn

[Q57] 行号
来源：http://sm.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nh.shtwfgs.cn

[Q58] 累计求和
来源：http://rk.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kz.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://nm.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://li.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://lt.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oe.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cn.yuntaijiaju.cn

[Q61] 移动平均
来源：http://wc.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tt.huixinmuqiang.cn

[Q62] 分组占比
来源：http://sg.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bn.asd995.cn

[Q63] 开启事务
来源：http://sx.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://op.lnxyls.cn

[Q64] 提交事务
来源：http://rz.hnjuh.cn

COMMIT;
来源：http://iv.szsharing.cn

[Q65] 回滚事务
来源：http://wo.jianghongdianzi.cn

ROLLBACK;
来源：http://jn.muxihuayi.cn

[Q66] 行锁查询
来源：http://uw.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ez.newstarts.cn

[Q67] 设置隔离级别
来源：http://bq.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ch.panjiajie.cn

[Q68] 保存点
来源：http://nc.szsharing.cn

SAVEPOINT sp1;
来源：http://km.colortex.cn

ROLLBACK TO sp1;
来源：http://ad.521024.cn

[Q69] 查看执行计划
来源：http://wd.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vs.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://iy.nicolike.cn

ANALYZE TABLE users;
来源：http://cz.chemitech.net.cn

[Q71] 查看建表语句
来源：http://fs.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://af.asd995.cn

[Q72] 查看索引
来源：http://as.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://ug.chemitech.net.cn

[Q73] 查看表状态
来源：http://km.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kh.huanxung.cn

[Q74] 强制使用索引
来源：http://go.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tv.colortex.cn

[Q75] 日期格式化
来源：http://yi.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fq.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://in.yuntaijiaju.cn

[Q76] 按天统计
来源：http://oe.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zs.9csxet.cn

[Q77] 时间加减
来源：http://xi.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qr.yuexingan06.cn

[Q78] 当前时间
来源：http://up.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mu.szsharing.cn

[Q79] 字符串拼接
来源：http://ml.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ep.panjiajie.cn

[Q80] 字符串截取
来源：http://ae.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ye.newstarts.cn

[Q81] 字符串替换
来源：http://fx.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yc.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://tz.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iv.panjiajie.cn

[Q83] 大小写转换
来源：http://we.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qy.shxzskj.cn

[Q84] 去除首尾空格
来源：http://hi.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://rw.bookmarksfly.cn

[Q85] 数值取整
来源：http://rb.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pu.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://tq.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hp.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://dv.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kt.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://nk.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ox.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xx.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://lp.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ku.newstarts.cn

[Q90] 生成序号列
来源：http://gz.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ew.yuntaijiaju.cn

================================================================================
来源：http://aq.hnjuh.cn

R. Bash 专题
来源：http://lu.shtwfgs.cn

================================================================================
来源：http://hb.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://zx.shtwfgs.cn

#!/usr/bin/env bash
来源：http://ie.521024.cn

set -euo pipefail
来源：http://jk.huanxung.cn

[R02] 变量赋值与使用
来源：http://db.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://sp.chemitech.net.cn

[R03] 只读变量
来源：http://ur.9csxet.cn

readonly PI=3.14
来源：http://rf.lnxyls.cn

[R04] 位置参数
来源：http://qu.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yw.shxzskj.cn

[R05] 参数默认值
来源：http://jv.jctech888.com.cn

name="${1:-default}"
来源：http://hr.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://ph.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pv.bookmarksfly.cn

[R07] if 判断文件
来源：http://fo.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ve.hnjuh.cn

[R08] 数值比较
来源：http://sb.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ce.nszjky.cn

[R09] 字符串比较
来源：http://hj.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dg.hahajie.cn

[R10] 正则匹配
来源：http://wn.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pz.shxzskj.cn

[R11] case 多分支
来源：http://vo.yuntaijiaju.cn

case "$1" in
来源：http://iu.huixiangedu.cn

start) echo "启动" ;;
来源：http://ab.hahajie.cn

stop)  echo "停止" ;;
来源：http://hl.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://bi.shxzskj.cn

esac
来源：http://hs.nicolike.cn

[R12] for 遍历文件
来源：http://ao.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://jc.chemitech.net.cn

[R13] for 计数循环
来源：http://vp.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://pw.nszjky.cn

[R14] C 风格 for
来源：http://vi.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ie.yuexingan06.cn

[R15] while 逐行读文件
来源：http://gj.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hi.chemitech.net.cn

[R16] until 等待条件
来源：http://st.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hf.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://rx.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ds.hahajie.cn

[R18] 遍历数组
来源：http://ua.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://np.hahajie.cn

[R19] 数组长度
来源：http://if.yuexingan06.cn

echo "${#arr[@]}"
来源：http://mm.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://ke.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gw.hnjuh.cn

[R21] 字符串长度
来源：http://hk.bookmarksfly.cn

echo "${#s}"
来源：http://dr.yuntaijiaju.cn

[R22] 截取子串
来源：http://lf.nszjky.cn

echo "${s:0:5}"
来源：http://xh.panjiajie.cn

[R23] 字符串替换
来源：http://wi.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dv.jctech888.com.cn

[R24] 大小写转换
来源：http://zv.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://im.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://jo.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bv.jctech888.com.cn

[R26] 命令替换
来源：http://ke.colortex.cn

now=$(date +%F); echo "$now"
来源：http://hq.yuexingan06.cn

[R27] 算术展开
来源：http://bc.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://nm.wgjwhj.cn

[R28] 浮点运算
来源：http://oi.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://xw.szxytkj.cn

[R29] 定义函数
来源：http://qu.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://la.shtwfgs.cn

[R30] 函数返回状态码
来源：http://in.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://sp.szxytkj.cn

[R31] 局部变量
来源：http://jw.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://tq.lnxyls.cn

[R32] 参数个数校验
来源：http://us.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bz.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://ov.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jn.panjiajie.cn

[R34] 退出时清理
来源：http://bu.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ad.asd995.cn

[R35] 后台执行并等待
来源：http://fj.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ph.shxzukj.cn

[R36] 并发执行多个任务
来源：http://bm.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hl.hnjuh.cn

[R37] 把输出赋给变量
来源：http://nn.nicolike.cn

files=$(ls -1)
来源：http://kx.huanxung.cn

[R38] 管道串联
来源：http://uz.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://gb.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://vp.jctech888.com.cn

cmd > out.log 2>&1
来源：http://oq.lnxyls.cn

[R40] 追加写日志
来源：http://xy.yuexingan06.cn

echo "log" >> out.log
来源：http://ev.muxihuayi.cn

[R41] 丢弃输出
来源：http://iw.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://eq.haigaiapp.cn

[R42] 输入重定向
来源：http://hp.hnjuh.cn

wc -l < a.txt
来源：http://ki.yuexingan06.cn

[R43] 按名字查找文件
来源：http://gl.jctech888.com.cn

find . -name "*.log" -type f
来源：http://uu.szsharing.cn

[R44] 按修改时间查找
来源：http://ed.haigaiapp.cn

find . -mtime -7 -type f
来源：http://bv.muxihuayi.cn

[R45] 批量删除
来源：http://ci.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://an.huanxung.cn

[R46] 递归替换文件内容
来源：http://jl.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://al.gzmigu.cn

[R47] sed 单行替换
来源：http://nz.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://px.yuexingan06.cn

[R48] awk 取指定列
来源：http://tk.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://zj.521024.cn

[R49] awk 带条件
来源：http://wu.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://im.shxzskj.cn

[R50] awk 求和
来源：http://lc.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lf.nicolike.cn

[R51] 排序去重取前几
来源：http://cp.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ym.521024.cn

[R52] 统计行数
来源：http://eb.521024.cn

wc -l a.txt
来源：http://po.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://qt.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ns.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://hs.huixiangedu.cn

diff a.txt b.txt
来源：http://qe.shtwfgs.cn

[R55] 压缩与解压
来源：http://gh.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qi.gzmigu.cn

[R56] 远程拷贝
来源：http://xz.chemitech.net.cn

scp file user@host:/path/
来源：http://jv.hahajie.cn

[R57] 远程执行命令
来源：http://tv.yuexingan06.cn

ssh user@host 'uptime'
来源：http://ns.huixiangedu.cn

[R58] 下载文件
来源：http://ry.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ft.shxzukj.cn

[R59] 发 POST JSON
来源：http://xc.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vv.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://bb.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gj.szxytkj.cn

[R61] 磁盘占用
来源：http://cn.colortex.cn

df -h;  du -sh *
来源：http://uh.lnxyls.cn

[R62] 找最占空间的文件
来源：http://cz.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://zn.9csxet.cn

[R63] 内存与进程
来源：http://xb.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://el.huixinmuqiang.cn

[R64] 结束进程
来源：http://ty.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://ga.huanxung.cn

[R65] 查看端口占用
来源：http://ml.bookmarksfly.cn


<!-- 参考信息 -->