代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mx.chemitech.net.cn

[Q20] IN 列表
来源：http://gn.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xu.panjiajie.cn

[Q21] 空值判断
来源：http://mm.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oj.yuexingan06.cn

[Q22] 排序
来源：http://en.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yh.szxytkj.cn

[Q23] 分页
来源：http://pc.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ej.lnxyls.cn

[Q24] 去重
来源：http://yz.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://tf.9csxet.cn

[Q25] 只取前 N 条
来源：http://dg.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bd.bookmarksfly.cn

[Q26] 计数
来源：http://hw.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://qt.hahajie.cn

[Q27] 条件计数
来源：http://nz.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fr.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://vh.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ku.huanxung.cn

[Q29] 最大最小值
来源：http://qe.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ew.nszjky.cn

[Q30] 分组统计
来源：http://nz.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eg.chemitech.net.cn

[Q31] 分组后过滤
来源：http://db.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zp.nicolike.cn

[Q32] 分组拼接字符串
来源：http://pj.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kb.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yq.lnxyls.cn

[Q33] 多列分组
来源：http://qc.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jh.szsharing.cn

[Q34] 每组取第一条
来源：http://zh.haigaiapp.cn

SELECT * FROM (
来源：http://qd.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ks.colortex.cn

) t WHERE rn = 1;
来源：http://ak.hahajie.cn

[Q35] 内连接
来源：http://hp.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sv.panjiajie.cn

[Q36] 左连接
来源：http://wy.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kr.panjiajie.cn

[Q37] 右连接
来源：http://im.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ni.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ds.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yh.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://mw.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lq.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gs.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nn.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fi.521024.cn

[Q41] 多表连接
来源：http://pg.huanxung.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fk.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://jp.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://ag.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://ea.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://ty.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zy.shxzskj.cn

[Q43] 标量子查询
来源：http://vw.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wp.bjjhwx.cn

[Q44] IN 子查询
来源：http://sl.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aq.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://va.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vv.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sy.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jb.shxzukj.cn

[Q47] 与平均值比较
来源：http://va.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fc.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://dr.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xy.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://xc.shxzskj.cn

[Q49] 更新单行
来源：http://md.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fn.szxytkj.cn

[Q50] 批量更新
来源：http://uy.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gm.hnjuh.cn

[Q51] 用子查询更新
来源：http://on.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bn.shxzukj.cn

[Q52] 删除指定行
来源：http://ef.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://di.shxzskj.cn

[Q53] 按条件删除
来源：http://al.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sv.lnxyls.cn

[Q54] 清空表
来源：http://qg.asd995.cn

TRUNCATE TABLE logs;
来源：http://zt.521024.cn

[Q55] 排名（并列占位）
来源：http://bc.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ol.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://gf.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zd.yuntaijiaju.cn

[Q57] 行号
来源：http://ds.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oi.shxzskj.cn

[Q58] 累计求和
来源：http://zm.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vp.asd995.cn

[Q59] 分组内累计
来源：http://xm.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dh.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://xj.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rh.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ry.jianghongdianzi.cn

[Q61] 移动平均
来源：http://lq.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jf.asd995.cn

[Q62] 分组占比
来源：http://dj.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tc.jianghongdianzi.cn

[Q63] 开启事务
来源：http://bg.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gp.huanxung.cn

[Q64] 提交事务
来源：http://oh.huixiangedu.cn

COMMIT;
来源：http://er.wgjwhj.cn

[Q65] 回滚事务
来源：http://qh.muxihuayi.cn

ROLLBACK;
来源：http://tp.panjiajie.cn

[Q66] 行锁查询
来源：http://tt.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yu.panjiajie.cn

[Q67] 设置隔离级别
来源：http://vw.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mx.521024.cn

[Q68] 保存点
来源：http://gv.newstarts.cn

SAVEPOINT sp1;
来源：http://ja.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://ap.521024.cn

[Q69] 查看执行计划
来源：http://mk.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jc.shxzukj.cn

[Q70] 更新统计信息
来源：http://ta.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://yg.nszjky.cn

[Q71] 查看建表语句
来源：http://mm.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yf.huixinmuqiang.cn

[Q72] 查看索引
来源：http://su.shxzskj.cn

SHOW INDEX FROM users;
来源：http://mw.chemitech.net.cn

[Q73] 查看表状态
来源：http://pn.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ga.shtwfgs.cn

[Q74] 强制使用索引
来源：http://nq.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vb.hnjuh.cn

[Q75] 日期格式化
来源：http://qc.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cs.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wu.jianghongdianzi.cn

[Q76] 按天统计
来源：http://yt.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nw.panjiajie.cn

[Q77] 时间加减
来源：http://tr.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://id.bookmarksfly.cn

[Q78] 当前时间
来源：http://eu.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qj.hnjuh.cn

[Q79] 字符串拼接
来源：http://zh.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lq.panjiajie.cn

[Q80] 字符串截取
来源：http://pg.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pe.9csxet.cn

[Q81] 字符串替换
来源：http://tc.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jy.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://rc.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ne.huanxung.cn

[Q83] 大小写转换
来源：http://ja.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ro.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://er.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://uz.szxytkj.cn

[Q85] 数值取整
来源：http://dp.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kx.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://jn.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jg.nicolike.cn

[Q87] JSON 字段做条件
来源：http://si.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uv.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://pc.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jx.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kf.panjiajie.cn

[Q89] 判断表是否存在
来源：http://ki.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ms.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://gz.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eo.jianghongdianzi.cn

================================================================================
来源：http://wd.wgjwhj.cn

R. Bash 专题
来源：http://hd.asd995.cn

================================================================================
来源：http://qd.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://ir.hnjuh.cn

#!/usr/bin/env bash
来源：http://zj.huixiangedu.cn

set -euo pipefail
来源：http://mj.521024.cn

[R02] 变量赋值与使用
来源：http://ub.9csxet.cn

name="Tom"; echo "$name"
来源：http://ho.colortex.cn

[R03] 只读变量
来源：http://ed.huanxung.cn

readonly PI=3.14
来源：http://ye.yuexingan06.cn

[R04] 位置参数
来源：http://ww.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qo.haigaiapp.cn

[R05] 参数默认值
来源：http://nz.shxzskj.cn

name="${1:-default}"
来源：http://la.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://rz.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pl.9csxet.cn

[R07] if 判断文件
来源：http://vi.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ey.muxihuayi.cn

[R08] 数值比较
来源：http://dx.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zq.yuexingan06.cn

[R09] 字符串比较
来源：http://ge.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ij.newstarts.cn

[R10] 正则匹配
来源：http://co.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hy.muxihuayi.cn

[R11] case 多分支
来源：http://uh.colortex.cn

case "$1" in
来源：http://cb.huixiangedu.cn

start) echo "启动" ;;
来源：http://cm.colortex.cn

stop)  echo "停止" ;;
来源：http://ei.huanxung.cn

*)     echo "未知命令" ;;
来源：http://fu.jctech888.com.cn

esac
来源：http://xd.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://fu.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://ec.szxytkj.cn

[R13] for 计数循环
来源：http://it.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://nk.shxzskj.cn

[R14] C 风格 for
来源：http://ia.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://br.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://sc.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kz.wgjwhj.cn

[R16] until 等待条件
来源：http://rw.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xp.bjjhwx.cn

[R17] 数组定义与取值
来源：http://pu.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iq.shtwfgs.cn

[R18] 遍历数组
来源：http://ff.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tg.hahajie.cn

[R19] 数组长度
来源：http://bm.shtwfgs.cn

echo "${#arr[@]}"
来源：http://es.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://nb.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vr.yuntaijiaju.cn

[R21] 字符串长度
来源：http://hd.hnjuh.cn

echo "${#s}"
来源：http://ic.panjiajie.cn

[R22] 截取子串
来源：http://nr.szsharing.cn

echo "${s:0:5}"
来源：http://yk.newstarts.cn

[R23] 字符串替换
来源：http://tc.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mz.haigaiapp.cn

[R24] 大小写转换
来源：http://ss.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ic.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://kv.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bw.chemitech.net.cn

[R26] 命令替换
来源：http://ba.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://qi.colortex.cn

[R27] 算术展开
来源：http://zw.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://pv.shxzukj.cn

[R28] 浮点运算
来源：http://vm.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://cm.muxihuayi.cn

[R29] 定义函数
来源：http://mm.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cp.haigaiapp.cn

[R30] 函数返回状态码
来源：http://pf.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://nw.panjiajie.cn

[R31] 局部变量
来源：http://sd.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://df.shtwfgs.cn

[R32] 参数个数校验
来源：http://lr.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zo.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://yq.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ei.wgjwhj.cn

[R34] 退出时清理
来源：http://jj.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yj.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://jc.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://aa.nicolike.cn

[R36] 并发执行多个任务
来源：http://do.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ld.szsharing.cn

[R37] 把输出赋给变量
来源：http://kl.shxzskj.cn

files=$(ls -1)
来源：http://lr.bookmarksfly.cn

[R38] 管道串联
来源：http://cu.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://rm.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://dv.huanxung.cn

cmd > out.log 2>&1
来源：http://on.shxzukj.cn

[R40] 追加写日志
来源：http://ln.haigaiapp.cn

echo "log" >> out.log
来源：http://pp.nicolike.cn

[R41] 丢弃输出
来源：http://pf.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://cu.szsharing.cn

[R42] 输入重定向
来源：http://ag.lnxyls.cn

wc -l < a.txt
来源：http://ar.shtwfgs.cn

[R43] 按名字查找文件
来源：http://lt.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://tj.shtwfgs.cn

[R44] 按修改时间查找
来源：http://do.wgjwhj.cn

find . -mtime -7 -type f
来源：http://tm.huanxung.cn

[R45] 批量删除
来源：http://ua.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://ap.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://zw.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dh.hahajie.cn

[R47] sed 单行替换
来源：http://ng.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vk.jctech888.com.cn

[R48] awk 取指定列
来源：http://ol.521024.cn

awk '{print $1, $3}' a.txt
来源：http://do.shxzukj.cn

[R49] awk 带条件
来源：http://la.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qj.nicolike.cn

[R50] awk 求和
来源：http://ji.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ci.lnxyls.cn

[R51] 排序去重取前几
来源：http://ow.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bn.szsharing.cn

[R52] 统计行数
来源：http://ak.lnxyls.cn

wc -l a.txt
来源：http://rz.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://yj.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cf.yuexingan06.cn

[R54] 比较两个文件
来源：http://ur.huixiangedu.cn

diff a.txt b.txt
来源：http://sq.wgjwhj.cn

[R55] 压缩与解压
来源：http://tr.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ps.szsharing.cn

[R56] 远程拷贝
来源：http://tg.shxzskj.cn

scp file user@host:/path/
来源：http://rd.huanxung.cn

[R57] 远程执行命令
来源：http://oj.chemitech.net.cn

ssh user@host 'uptime'
来源：http://ht.wgjwhj.cn

[R58] 下载文件
来源：http://ni.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qj.hahajie.cn

[R59] 发 POST JSON
来源：http://ku.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vw.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://lr.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zh.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://pu.shxzskj.cn

df -h;  du -sh *
来源：http://hg.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://jj.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://ko.wgjwhj.cn

[R63] 内存与进程
来源：http://zq.colortex.cn

free -h;  ps aux | grep nginx
来源：http://qu.asd995.cn

[R64] 结束进程
来源：http://tv.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://uf.colortex.cn

[R65] 查看端口占用
来源：http://av.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ge.wgjwhj.cn

[R66] 定时任务
来源：http://xd.asd995.cn

crontab -e;  crontab -l
来源：http://vx.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://ne.yuexingan06.cn

openssl rand -hex 16
来源：http://zi.gzmigu.cn

[R68] 计算文件校验值
来源：http://yf.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jr.shtwfgs.cn

[R69] 生成随机密码
来源：http://xm.521024.cn


<!-- 参考信息 -->