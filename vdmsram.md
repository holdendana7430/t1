代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vq.szsharing.cn

[Q18] 模糊匹配
来源：http://qv.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xk.shxzukj.cn

[Q19] 范围查询
来源：http://sp.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rk.lnxyls.cn

[Q20] IN 列表
来源：http://wy.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qu.szsharing.cn

[Q21] 空值判断
来源：http://ri.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lw.chemitech.net.cn

[Q22] 排序
来源：http://ak.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lv.bookmarksfly.cn

[Q23] 分页
来源：http://ct.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ho.newstarts.cn

[Q24] 去重
来源：http://lv.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://jr.hahajie.cn

[Q25] 只取前 N 条
来源：http://zs.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cw.nszjky.cn

[Q26] 计数
来源：http://kw.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://sd.hnjuh.cn

[Q27] 条件计数
来源：http://nm.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jk.lnxyls.cn

[Q28] 求和与平均
来源：http://sb.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qh.shxzskj.cn

[Q29] 最大最小值
来源：http://pv.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xk.hnjuh.cn

[Q30] 分组统计
来源：http://hp.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cw.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://yz.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ux.newstarts.cn

[Q32] 分组拼接字符串
来源：http://my.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xi.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fv.lnxyls.cn

[Q33] 多列分组
来源：http://zw.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wl.yuexingan06.cn

[Q34] 每组取第一条
来源：http://oq.bookmarksfly.cn

SELECT * FROM (
来源：http://kb.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oq.jctech888.com.cn

) t WHERE rn = 1;
来源：http://gp.jianghongdianzi.cn

[Q35] 内连接
来源：http://xn.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tb.521024.cn

[Q36] 左连接
来源：http://bk.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fq.yuexingan06.cn

[Q37] 右连接
来源：http://tj.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uq.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dj.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jo.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://xz.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ie.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rk.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hp.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sr.szxytkj.cn

[Q41] 多表连接
来源：http://yj.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ed.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://dx.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://ka.colortex.cn

[Q42] 连接条件附加过滤
来源：http://mu.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://fd.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ll.szsharing.cn

[Q43] 标量子查询
来源：http://hz.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kw.panjiajie.cn

[Q44] IN 子查询
来源：http://ku.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kh.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://kl.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kz.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sp.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xl.colortex.cn

[Q47] 与平均值比较
来源：http://wn.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bw.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://an.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ye.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://mf.yuexingan06.cn

[Q49] 更新单行
来源：http://br.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ik.szsharing.cn

[Q50] 批量更新
来源：http://wh.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://by.huanxung.cn

[Q51] 用子查询更新
来源：http://zz.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hu.huanxung.cn

[Q52] 删除指定行
来源：http://iv.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://xq.shtwfgs.cn

[Q53] 按条件删除
来源：http://id.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hs.lnxyls.cn

[Q54] 清空表
来源：http://iy.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://hk.521024.cn

[Q55] 排名（并列占位）
来源：http://ev.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bk.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://fo.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rj.huixinmuqiang.cn

[Q57] 行号
来源：http://vq.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ls.yuexingan06.cn

[Q58] 累计求和
来源：http://ue.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cm.bookmarksfly.cn

[Q59] 分组内累计
来源：http://hs.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rm.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://dv.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vp.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gf.bjjhwx.cn

[Q61] 移动平均
来源：http://ek.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oq.nicolike.cn

[Q62] 分组占比
来源：http://yx.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gj.szxytkj.cn

[Q63] 开启事务
来源：http://ee.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jc.szsharing.cn

[Q64] 提交事务
来源：http://gj.yuexingan06.cn

COMMIT;
来源：http://zp.521024.cn

[Q65] 回滚事务
来源：http://sf.szxytkj.cn

ROLLBACK;
来源：http://rm.newstarts.cn

[Q66] 行锁查询
来源：http://jz.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cx.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://np.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rq.shtwfgs.cn

[Q68] 保存点
来源：http://vm.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://sp.panjiajie.cn

ROLLBACK TO sp1;
来源：http://bj.shtwfgs.cn

[Q69] 查看执行计划
来源：http://ef.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iw.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://sl.hnjuh.cn

ANALYZE TABLE users;
来源：http://rv.yuexingan06.cn

[Q71] 查看建表语句
来源：http://fk.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tx.hnjuh.cn

[Q72] 查看索引
来源：http://av.521024.cn

SHOW INDEX FROM users;
来源：http://rn.panjiajie.cn

[Q73] 查看表状态
来源：http://ux.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bd.colortex.cn

[Q74] 强制使用索引
来源：http://qh.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://js.haigaiapp.cn

[Q75] 日期格式化
来源：http://sa.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sz.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qq.panjiajie.cn

[Q76] 按天统计
来源：http://fp.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://am.panjiajie.cn

[Q77] 时间加减
来源：http://fd.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vz.asd995.cn

[Q78] 当前时间
来源：http://fi.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nb.szsharing.cn

[Q79] 字符串拼接
来源：http://lk.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bh.nszjky.cn

[Q80] 字符串截取
来源：http://dx.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kd.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://ev.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yt.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://pb.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fy.szxytkj.cn

[Q83] 大小写转换
来源：http://bg.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xt.9csxet.cn

[Q84] 去除首尾空格
来源：http://qb.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://bn.szsharing.cn

[Q85] 数值取整
来源：http://ih.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rg.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://bl.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eq.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://ax.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sy.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://qd.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hw.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xo.newstarts.cn

[Q89] 判断表是否存在
来源：http://lz.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ec.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://vn.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vf.shtwfgs.cn

================================================================================
来源：http://dh.szxytkj.cn

R. Bash 专题
来源：http://nm.szxytkj.cn

================================================================================
来源：http://ww.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://ll.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://uo.shxzukj.cn

set -euo pipefail
来源：http://lu.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://xu.gzmigu.cn

name="Tom"; echo "$name"
来源：http://dp.shxzskj.cn

[R03] 只读变量
来源：http://hq.jianghongdianzi.cn

readonly PI=3.14
来源：http://ii.huanxung.cn

[R04] 位置参数
来源：http://oz.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hb.szxytkj.cn

[R05] 参数默认值
来源：http://fs.huanxung.cn

name="${1:-default}"
来源：http://pd.gzmigu.cn

[R06] 判断命令是否存在
来源：http://ai.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kw.shtwfgs.cn

[R07] if 判断文件
来源：http://is.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vh.asd995.cn

[R08] 数值比较
来源：http://hs.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ym.yuexingan06.cn

[R09] 字符串比较
来源：http://kn.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://se.hahajie.cn

[R10] 正则匹配
来源：http://my.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ad.panjiajie.cn

[R11] case 多分支
来源：http://es.bjjhwx.cn

case "$1" in
来源：http://iu.szxytkj.cn

start) echo "启动" ;;
来源：http://xj.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://fj.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://eo.lnxyls.cn

esac
来源：http://sh.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://of.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://ty.shxzukj.cn

[R13] for 计数循环
来源：http://mv.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://ah.asd995.cn

[R14] C 风格 for
来源：http://ve.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wf.9csxet.cn

[R15] while 逐行读文件
来源：http://vj.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cc.jctech888.com.cn

[R16] until 等待条件
来源：http://nz.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ro.shtwfgs.cn

[R17] 数组定义与取值
来源：http://da.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zs.nszjky.cn

[R18] 遍历数组
来源：http://dk.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ha.haigaiapp.cn

[R19] 数组长度
来源：http://on.jctech888.com.cn

echo "${#arr[@]}"
来源：http://ht.hahajie.cn

[R20] 关联数组（字典）
来源：http://ts.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://db.panjiajie.cn

[R21] 字符串长度
来源：http://tb.lnxyls.cn

echo "${#s}"
来源：http://ri.hahajie.cn

[R22] 截取子串
来源：http://ip.hahajie.cn

echo "${s:0:5}"
来源：http://yj.bookmarksfly.cn

[R23] 字符串替换
来源：http://jy.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kt.haigaiapp.cn

[R24] 大小写转换
来源：http://kj.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ct.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://tl.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rl.gzmigu.cn

[R26] 命令替换
来源：http://ih.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://fl.haigaiapp.cn

[R27] 算术展开
来源：http://yv.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://qr.jctech888.com.cn

[R28] 浮点运算
来源：http://jh.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://vr.newstarts.cn

[R29] 定义函数
来源：http://qi.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gz.shtwfgs.cn

[R30] 函数返回状态码
来源：http://ov.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://eo.haigaiapp.cn

[R31] 局部变量
来源：http://uo.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://qy.nszjky.cn

[R32] 参数个数校验
来源：http://qh.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ug.asd995.cn

[R33] 捕获错误并提示行号
来源：http://xf.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yw.asd995.cn

[R34] 退出时清理
来源：http://nw.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uv.yuexingan06.cn

[R35] 后台执行并等待
来源：http://ax.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tg.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://to.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://af.szxytkj.cn

[R37] 把输出赋给变量
来源：http://ha.haigaiapp.cn

files=$(ls -1)
来源：http://zu.9csxet.cn

[R38] 管道串联
来源：http://kz.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://ra.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://go.9csxet.cn

cmd > out.log 2>&1
来源：http://mx.nszjky.cn

[R40] 追加写日志
来源：http://is.bookmarksfly.cn

echo "log" >> out.log
来源：http://ne.521024.cn

[R41] 丢弃输出
来源：http://wn.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://ap.wgjwhj.cn

[R42] 输入重定向
来源：http://je.521024.cn

wc -l < a.txt
来源：http://dx.huanxung.cn

[R43] 按名字查找文件
来源：http://cd.panjiajie.cn

find . -name "*.log" -type f
来源：http://ay.panjiajie.cn

[R44] 按修改时间查找
来源：http://mx.colortex.cn

find . -mtime -7 -type f
来源：http://yu.huixinmuqiang.cn

[R45] 批量删除
来源：http://kj.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://vd.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://rq.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mi.chemitech.net.cn

[R47] sed 单行替换
来源：http://so.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vd.gzmigu.cn

[R48] awk 取指定列
来源：http://pd.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://ck.colortex.cn

[R49] awk 带条件
来源：http://zj.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://te.nszjky.cn

[R50] awk 求和
来源：http://sb.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vb.hnjuh.cn

[R51] 排序去重取前几
来源：http://hs.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zk.jianghongdianzi.cn

[R52] 统计行数
来源：http://en.bookmarksfly.cn

wc -l a.txt
来源：http://mn.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://nj.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iv.chemitech.net.cn

[R54] 比较两个文件
来源：http://fw.chemitech.net.cn

diff a.txt b.txt
来源：http://tv.shxzukj.cn

[R55] 压缩与解压
来源：http://ss.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mv.panjiajie.cn

[R56] 远程拷贝
来源：http://lr.wgjwhj.cn

scp file user@host:/path/
来源：http://eo.hnjuh.cn

[R57] 远程执行命令
来源：http://la.shxzskj.cn

ssh user@host 'uptime'
来源：http://hj.muxihuayi.cn

[R58] 下载文件
来源：http://km.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vg.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://he.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://it.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://ai.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kg.yuexingan06.cn

[R61] 磁盘占用
来源：http://ew.haigaiapp.cn

df -h;  du -sh *
来源：http://tz.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://px.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://ir.lnxyls.cn

[R63] 内存与进程
来源：http://wm.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://lu.9csxet.cn

[R64] 结束进程
来源：http://df.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://ce.asd995.cn

[R65] 查看端口占用
来源：http://lx.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lx.nszjky.cn

[R66] 定时任务
来源：http://cx.hnjuh.cn

crontab -e;  crontab -l
来源：http://uf.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://nt.hnjuh.cn


<!-- 参考信息 -->