代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ct.hahajie.cn

[Q20] IN 列表
来源：http://kw.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ds.shtwfgs.cn

[Q21] 空值判断
来源：http://bb.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wb.bjjhwx.cn

[Q22] 排序
来源：http://cb.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rk.521024.cn

[Q23] 分页
来源：http://ol.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tx.nszjky.cn

[Q24] 去重
来源：http://km.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://ey.colortex.cn

[Q25] 只取前 N 条
来源：http://pd.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ll.hnjuh.cn

[Q26] 计数
来源：http://fu.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://bv.szsharing.cn

[Q27] 条件计数
来源：http://cw.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sw.lnxyls.cn

[Q28] 求和与平均
来源：http://sb.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ga.haigaiapp.cn

[Q29] 最大最小值
来源：http://fv.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://de.huixinmuqiang.cn

[Q30] 分组统计
来源：http://yb.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cm.chemitech.net.cn

[Q31] 分组后过滤
来源：http://sp.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://el.colortex.cn

[Q32] 分组拼接字符串
来源：http://qr.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dy.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rt.hahajie.cn

[Q33] 多列分组
来源：http://nw.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jb.yuexingan06.cn

[Q34] 每组取第一条
来源：http://cj.521024.cn

SELECT * FROM (
来源：http://bs.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://he.gzmigu.cn

) t WHERE rn = 1;
来源：http://ri.521024.cn

[Q35] 内连接
来源：http://zj.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yf.haigaiapp.cn

[Q36] 左连接
来源：http://fu.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fx.hnjuh.cn

[Q37] 右连接
来源：http://hn.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jb.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zq.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pv.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://hx.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vp.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cs.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://er.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bu.szxytkj.cn

[Q41] 多表连接
来源：http://bc.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hu.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://kc.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://nj.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://fd.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://re.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bc.shxzskj.cn

[Q43] 标量子查询
来源：http://fj.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sm.asd995.cn

[Q44] IN 子查询
来源：http://dc.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pv.asd995.cn

[Q45] EXISTS 判断存在
来源：http://ls.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://co.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kk.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ro.nicolike.cn

[Q47] 与平均值比较
来源：http://zc.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mn.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://ut.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dx.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://pj.gzmigu.cn

[Q49] 更新单行
来源：http://ql.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oq.nszjky.cn

[Q50] 批量更新
来源：http://vq.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xf.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://nm.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cy.9csxet.cn

[Q52] 删除指定行
来源：http://hr.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://xf.muxihuayi.cn

[Q53] 按条件删除
来源：http://yv.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qv.huixiangedu.cn

[Q54] 清空表
来源：http://vm.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://kk.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://mz.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dz.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://mp.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xq.gzmigu.cn

[Q57] 行号
来源：http://qz.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ps.szsharing.cn

[Q58] 累计求和
来源：http://dj.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xr.nszjky.cn

[Q59] 分组内累计
来源：http://rf.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ob.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://pw.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mg.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rs.szsharing.cn

[Q61] 移动平均
来源：http://yo.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ip.nszjky.cn

[Q62] 分组占比
来源：http://gt.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hg.jianghongdianzi.cn

[Q63] 开启事务
来源：http://nu.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://su.shtwfgs.cn

[Q64] 提交事务
来源：http://rc.521024.cn

COMMIT;
来源：http://zm.haigaiapp.cn

[Q65] 回滚事务
来源：http://om.lnxyls.cn

ROLLBACK;
来源：http://zy.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://cp.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nv.szxytkj.cn

[Q67] 设置隔离级别
来源：http://vg.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bd.chemitech.net.cn

[Q68] 保存点
来源：http://rt.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://hs.asd995.cn

ROLLBACK TO sp1;
来源：http://vw.shtwfgs.cn

[Q69] 查看执行计划
来源：http://ul.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bk.9csxet.cn

[Q70] 更新统计信息
来源：http://uw.wgjwhj.cn

ANALYZE TABLE users;
来源：http://bm.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://tf.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hf.hnjuh.cn

[Q72] 查看索引
来源：http://op.colortex.cn

SHOW INDEX FROM users;
来源：http://is.hnjuh.cn

[Q73] 查看表状态
来源：http://bq.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mh.hahajie.cn

[Q74] 强制使用索引
来源：http://nv.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vw.huanxung.cn

[Q75] 日期格式化
来源：http://fi.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kf.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zp.panjiajie.cn

[Q76] 按天统计
来源：http://tl.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cr.bjjhwx.cn

[Q77] 时间加减
来源：http://fu.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lp.huanxung.cn

[Q78] 当前时间
来源：http://un.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gh.muxihuayi.cn

[Q79] 字符串拼接
来源：http://pi.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vt.yuexingan06.cn

[Q80] 字符串截取
来源：http://hz.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bk.huanxung.cn

[Q81] 字符串替换
来源：http://ou.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jg.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://bz.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jl.jctech888.com.cn

[Q83] 大小写转换
来源：http://nb.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://az.nicolike.cn

[Q84] 去除首尾空格
来源：http://uc.521024.cn

SELECT TRIM(name) FROM users;
来源：http://dp.szxytkj.cn

[Q85] 数值取整
来源：http://sq.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tp.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://ts.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://no.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://bo.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qa.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://co.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ta.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vm.huanxung.cn

[Q89] 判断表是否存在
来源：http://do.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bu.hahajie.cn

[Q90] 生成序号列
来源：http://yl.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://by.wgjwhj.cn

================================================================================
来源：http://ms.chemitech.net.cn

R. Bash 专题
来源：http://aj.bjjhwx.cn

================================================================================
来源：http://my.hahajie.cn

[R01] shebang 与严格模式
来源：http://md.hnjuh.cn

#!/usr/bin/env bash
来源：http://cl.yuntaijiaju.cn

set -euo pipefail
来源：http://vh.nszjky.cn

[R02] 变量赋值与使用
来源：http://fw.lnxyls.cn

name="Tom"; echo "$name"
来源：http://ft.shxzukj.cn

[R03] 只读变量
来源：http://ld.lnxyls.cn

readonly PI=3.14
来源：http://qx.colortex.cn

[R04] 位置参数
来源：http://ja.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ou.jianghongdianzi.cn

[R05] 参数默认值
来源：http://xa.huixiangedu.cn

name="${1:-default}"
来源：http://nk.nszjky.cn

[R06] 判断命令是否存在
来源：http://qe.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ax.lnxyls.cn

[R07] if 判断文件
来源：http://hu.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vs.chemitech.net.cn

[R08] 数值比较
来源：http://ww.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zz.asd995.cn

[R09] 字符串比较
来源：http://lo.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yn.nszjky.cn

[R10] 正则匹配
来源：http://lq.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ie.shxzskj.cn

[R11] case 多分支
来源：http://bh.colortex.cn

case "$1" in
来源：http://ii.haigaiapp.cn

start) echo "启动" ;;
来源：http://gn.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://jb.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://dn.hnjuh.cn

esac
来源：http://vj.shxzukj.cn

[R12] for 遍历文件
来源：http://gv.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://lo.chemitech.net.cn

[R13] for 计数循环
来源：http://vo.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://nd.hahajie.cn

[R14] C 风格 for
来源：http://cw.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dx.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://gf.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ai.shtwfgs.cn

[R16] until 等待条件
来源：http://dt.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pn.hnjuh.cn

[R17] 数组定义与取值
来源：http://rt.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uy.huanxung.cn

[R18] 遍历数组
来源：http://ga.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wt.hnjuh.cn

[R19] 数组长度
来源：http://vc.9csxet.cn

echo "${#arr[@]}"
来源：http://wn.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://vf.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ow.huanxung.cn

[R21] 字符串长度
来源：http://tu.wgjwhj.cn

echo "${#s}"
来源：http://kh.huixiangedu.cn

[R22] 截取子串
来源：http://wg.lnxyls.cn

echo "${s:0:5}"
来源：http://ks.panjiajie.cn

[R23] 字符串替换
来源：http://lj.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bw.yuexingan06.cn

[R24] 大小写转换
来源：http://du.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vd.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://vu.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hw.huixinmuqiang.cn

[R26] 命令替换
来源：http://dh.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://al.colortex.cn

[R27] 算术展开
来源：http://ej.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://se.chemitech.net.cn

[R28] 浮点运算
来源：http://nu.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://ym.wgjwhj.cn

[R29] 定义函数
来源：http://nm.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://av.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://hc.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://pg.bookmarksfly.cn

[R31] 局部变量
来源：http://en.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://wz.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://wo.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hr.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://rf.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ts.yuntaijiaju.cn

[R34] 退出时清理
来源：http://of.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rq.szsharing.cn

[R35] 后台执行并等待
来源：http://zl.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oy.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://zk.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://st.hnjuh.cn

[R37] 把输出赋给变量
来源：http://rw.jctech888.com.cn

files=$(ls -1)
来源：http://th.haigaiapp.cn

[R38] 管道串联
来源：http://cw.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://rr.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://nz.panjiajie.cn

cmd > out.log 2>&1
来源：http://wv.bookmarksfly.cn

[R40] 追加写日志
来源：http://fj.huixinmuqiang.cn

echo "log" >> out.log
来源：http://dj.jctech888.com.cn

[R41] 丢弃输出
来源：http://fi.newstarts.cn

cmd >/dev/null 2>&1
来源：http://cg.haigaiapp.cn

[R42] 输入重定向
来源：http://ep.9csxet.cn

wc -l < a.txt
来源：http://wz.asd995.cn

[R43] 按名字查找文件
来源：http://do.shxzukj.cn

find . -name "*.log" -type f
来源：http://pr.szsharing.cn

[R44] 按修改时间查找
来源：http://pb.szsharing.cn

find . -mtime -7 -type f
来源：http://ct.hnjuh.cn

[R45] 批量删除
来源：http://gx.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://mx.panjiajie.cn

[R46] 递归替换文件内容
来源：http://dh.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pb.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://wv.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ko.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://iq.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://pd.newstarts.cn

[R49] awk 带条件
来源：http://xh.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://od.yuexingan06.cn

[R50] awk 求和
来源：http://xt.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xj.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://zr.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://er.chemitech.net.cn

[R52] 统计行数
来源：http://yc.szxytkj.cn

wc -l a.txt
来源：http://bp.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://ta.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ax.szxytkj.cn

[R54] 比较两个文件
来源：http://sx.bjjhwx.cn

diff a.txt b.txt
来源：http://pt.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://ss.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xz.colortex.cn

[R56] 远程拷贝
来源：http://rm.yuexingan06.cn

scp file user@host:/path/
来源：http://hf.asd995.cn

[R57] 远程执行命令
来源：http://lt.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://bh.shxzukj.cn

[R58] 下载文件
来源：http://xv.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bl.haigaiapp.cn

[R59] 发 POST JSON
来源：http://sr.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fz.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://fn.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ep.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://op.szsharing.cn

df -h;  du -sh *
来源：http://gx.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://ub.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ma.bookmarksfly.cn

[R63] 内存与进程
来源：http://pc.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://xv.asd995.cn

[R64] 结束进程
来源：http://jr.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://be.panjiajie.cn

[R65] 查看端口占用
来源：http://hr.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ri.jctech888.com.cn

[R66] 定时任务
来源：http://ls.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://vh.hahajie.cn

[R67] 生成随机十六进制串
来源：http://xz.gzmigu.cn

openssl rand -hex 16
来源：http://ht.nicolike.cn

[R68] 计算文件校验值
来源：http://dy.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ba.huanxung.cn

[R69] 生成随机密码
来源：http://jo.huixiangedu.cn


<!-- 参考信息 -->