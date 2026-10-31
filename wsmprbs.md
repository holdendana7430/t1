代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nx.hnjuh.cn

[Q24] 去重
来源：http://zd.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://wg.nicolike.cn

[Q25] 只取前 N 条
来源：http://zl.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ih.asd995.cn

[Q26] 计数
来源：http://qq.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://ze.jianghongdianzi.cn

[Q27] 条件计数
来源：http://dr.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ws.shxzskj.cn

[Q28] 求和与平均
来源：http://qr.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fs.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://da.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ae.shxzskj.cn

[Q30] 分组统计
来源：http://vw.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://js.newstarts.cn

[Q31] 分组后过滤
来源：http://cg.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sp.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://ol.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wj.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oz.huixiangedu.cn

[Q33] 多列分组
来源：http://tt.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jy.newstarts.cn

[Q34] 每组取第一条
来源：http://iq.gzmigu.cn

SELECT * FROM (
来源：http://jk.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tl.chemitech.net.cn

) t WHERE rn = 1;
来源：http://fe.shtwfgs.cn

[Q35] 内连接
来源：http://zt.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zz.yuexingan06.cn

[Q36] 左连接
来源：http://na.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jp.yuexingan06.cn

[Q37] 右连接
来源：http://rm.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eu.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://um.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ej.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://vb.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hu.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cl.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://em.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wa.chemitech.net.cn

[Q41] 多表连接
来源：http://sm.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hx.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://hk.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://eb.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://ub.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://ns.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://is.szsharing.cn

[Q43] 标量子查询
来源：http://tc.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zr.shtwfgs.cn

[Q44] IN 子查询
来源：http://mp.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fp.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://nq.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vi.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iv.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fr.szxytkj.cn

[Q47] 与平均值比较
来源：http://qn.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ss.521024.cn

[Q48] CTE 公用表表达式
来源：http://nf.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wk.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ox.shxzskj.cn

[Q49] 更新单行
来源：http://fs.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ga.panjiajie.cn

[Q50] 批量更新
来源：http://dj.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wz.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://aa.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hg.yuexingan06.cn

[Q52] 删除指定行
来源：http://sm.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://of.yuexingan06.cn

[Q53] 按条件删除
来源：http://sk.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wb.jctech888.com.cn

[Q54] 清空表
来源：http://zv.nszjky.cn

TRUNCATE TABLE logs;
来源：http://bu.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://pi.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ge.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://cq.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ro.panjiajie.cn

[Q57] 行号
来源：http://lk.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ol.haigaiapp.cn

[Q58] 累计求和
来源：http://bt.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wi.szxytkj.cn

[Q59] 分组内累计
来源：http://go.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jt.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://bh.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ic.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zx.shxzukj.cn

[Q61] 移动平均
来源：http://nr.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tb.newstarts.cn

[Q62] 分组占比
来源：http://id.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ia.wgjwhj.cn

[Q63] 开启事务
来源：http://iy.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cz.hnjuh.cn

[Q64] 提交事务
来源：http://on.jctech888.com.cn

COMMIT;
来源：http://tz.panjiajie.cn

[Q65] 回滚事务
来源：http://fv.gzmigu.cn

ROLLBACK;
来源：http://ji.521024.cn

[Q66] 行锁查询
来源：http://hn.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zt.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://tf.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sk.muxihuayi.cn

[Q68] 保存点
来源：http://xc.jctech888.com.cn

SAVEPOINT sp1;
来源：http://dp.hnjuh.cn

ROLLBACK TO sp1;
来源：http://vb.asd995.cn

[Q69] 查看执行计划
来源：http://ht.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ua.chemitech.net.cn

[Q70] 更新统计信息
来源：http://zj.huanxung.cn

ANALYZE TABLE users;
来源：http://mo.panjiajie.cn

[Q71] 查看建表语句
来源：http://nk.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xs.colortex.cn

[Q72] 查看索引
来源：http://ye.521024.cn

SHOW INDEX FROM users;
来源：http://vt.panjiajie.cn

[Q73] 查看表状态
来源：http://fq.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vp.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://nz.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oy.yuexingan06.cn

[Q75] 日期格式化
来源：http://ev.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kh.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://na.shxzskj.cn

[Q76] 按天统计
来源：http://tw.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://op.huanxung.cn

[Q77] 时间加减
来源：http://dx.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://we.jianghongdianzi.cn

[Q78] 当前时间
来源：http://xl.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xi.lnxyls.cn

[Q79] 字符串拼接
来源：http://ux.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ri.haigaiapp.cn

[Q80] 字符串截取
来源：http://kb.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dx.521024.cn

[Q81] 字符串替换
来源：http://db.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qq.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://ll.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bg.asd995.cn

[Q83] 大小写转换
来源：http://kt.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rv.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://hq.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://ex.szsharing.cn

[Q85] 数值取整
来源：http://rn.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fu.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://rm.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wz.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://po.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yg.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://lf.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yq.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gc.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://se.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dz.bookmarksfly.cn

[Q90] 生成序号列
来源：http://jf.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ae.szxytkj.cn

================================================================================
来源：http://to.muxihuayi.cn

R. Bash 专题
来源：http://il.shxzukj.cn

================================================================================
来源：http://pp.nszjky.cn

[R01] shebang 与严格模式
来源：http://br.hnjuh.cn

#!/usr/bin/env bash
来源：http://wl.chemitech.net.cn

set -euo pipefail
来源：http://qg.521024.cn

[R02] 变量赋值与使用
来源：http://he.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://sw.huixinmuqiang.cn

[R03] 只读变量
来源：http://ka.wgjwhj.cn

readonly PI=3.14
来源：http://oo.gzmigu.cn

[R04] 位置参数
来源：http://xd.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rl.wgjwhj.cn

[R05] 参数默认值
来源：http://yh.huanxung.cn

name="${1:-default}"
来源：http://og.colortex.cn

[R06] 判断命令是否存在
来源：http://nz.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yk.huanxung.cn

[R07] if 判断文件
来源：http://or.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ln.shxzukj.cn

[R08] 数值比较
来源：http://xe.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://np.521024.cn

[R09] 字符串比较
来源：http://qz.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ww.szsharing.cn

[R10] 正则匹配
来源：http://di.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://st.jianghongdianzi.cn

[R11] case 多分支
来源：http://qz.panjiajie.cn

case "$1" in
来源：http://zc.jctech888.com.cn

start) echo "启动" ;;
来源：http://sh.lnxyls.cn

stop)  echo "停止" ;;
来源：http://ow.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://jc.szxytkj.cn

esac
来源：http://ff.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://me.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://ze.huixiangedu.cn

[R13] for 计数循环
来源：http://ba.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://pq.nszjky.cn

[R14] C 风格 for
来源：http://xn.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eo.nicolike.cn

[R15] while 逐行读文件
来源：http://vl.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rd.jctech888.com.cn

[R16] until 等待条件
来源：http://vy.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iu.nicolike.cn

[R17] 数组定义与取值
来源：http://il.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bv.huixiangedu.cn

[R18] 遍历数组
来源：http://hh.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jh.yuntaijiaju.cn

[R19] 数组长度
来源：http://rx.nszjky.cn

echo "${#arr[@]}"
来源：http://ml.asd995.cn

[R20] 关联数组（字典）
来源：http://vn.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yt.szsharing.cn

[R21] 字符串长度
来源：http://go.asd995.cn

echo "${#s}"
来源：http://ij.hnjuh.cn

[R22] 截取子串
来源：http://va.lnxyls.cn

echo "${s:0:5}"
来源：http://hv.shxzskj.cn

[R23] 字符串替换
来源：http://gs.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xj.yuntaijiaju.cn

[R24] 大小写转换
来源：http://au.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gc.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://tl.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fv.9csxet.cn

[R26] 命令替换
来源：http://pt.asd995.cn

now=$(date +%F); echo "$now"
来源：http://gp.panjiajie.cn

[R27] 算术展开
来源：http://xj.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://wq.szsharing.cn

[R28] 浮点运算
来源：http://of.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://bb.nszjky.cn

[R29] 定义函数
来源：http://pd.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rr.wgjwhj.cn

[R30] 函数返回状态码
来源：http://nt.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://bu.nszjky.cn

[R31] 局部变量
来源：http://ut.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://vi.gzmigu.cn

[R32] 参数个数校验
来源：http://ny.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uy.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://dz.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lx.hahajie.cn

[R34] 退出时清理
来源：http://uj.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ds.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://xb.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bt.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://kh.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fp.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://iy.huixiangedu.cn

files=$(ls -1)
来源：http://kv.panjiajie.cn

[R38] 管道串联
来源：http://ck.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://pd.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://xz.shxzskj.cn

cmd > out.log 2>&1
来源：http://ir.szsharing.cn

[R40] 追加写日志
来源：http://wa.newstarts.cn

echo "log" >> out.log
来源：http://hi.huanxung.cn

[R41] 丢弃输出
来源：http://hp.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://gw.jctech888.com.cn

[R42] 输入重定向
来源：http://yf.shxzukj.cn

wc -l < a.txt
来源：http://fn.szxytkj.cn

[R43] 按名字查找文件
来源：http://zz.huanxung.cn

find . -name "*.log" -type f
来源：http://ik.szxytkj.cn

[R44] 按修改时间查找
来源：http://hw.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://pd.wgjwhj.cn

[R45] 批量删除
来源：http://hc.colortex.cn

find . -name "*.tmp" -delete
来源：http://sw.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://li.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wu.szsharing.cn

[R47] sed 单行替换
来源：http://qx.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yk.shxzukj.cn

[R48] awk 取指定列
来源：http://by.521024.cn

awk '{print $1, $3}' a.txt
来源：http://da.huixinmuqiang.cn

[R49] awk 带条件
来源：http://fi.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ew.asd995.cn

[R50] awk 求和
来源：http://ju.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zc.nszjky.cn

[R51] 排序去重取前几
来源：http://tc.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://et.shtwfgs.cn

[R52] 统计行数
来源：http://cp.szsharing.cn

wc -l a.txt
来源：http://sq.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://jv.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ms.bookmarksfly.cn

[R54] 比较两个文件
来源：http://sn.huixiangedu.cn

diff a.txt b.txt
来源：http://ow.szsharing.cn

[R55] 压缩与解压
来源：http://od.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ij.shxzskj.cn

[R56] 远程拷贝
来源：http://fn.shxzskj.cn

scp file user@host:/path/
来源：http://vx.haigaiapp.cn

[R57] 远程执行命令
来源：http://ug.nszjky.cn

ssh user@host 'uptime'
来源：http://cc.shxzukj.cn

[R58] 下载文件
来源：http://xc.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ur.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qz.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://wd.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://di.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://wf.bookmarksfly.cn

df -h;  du -sh *
来源：http://lh.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://yn.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://cu.nszjky.cn

[R63] 内存与进程
来源：http://ao.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://mf.yuntaijiaju.cn

[R64] 结束进程
来源：http://sg.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://cl.colortex.cn

[R65] 查看端口占用
来源：http://kn.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pv.szxytkj.cn

[R66] 定时任务
来源：http://gu.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://az.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://rk.szsharing.cn

openssl rand -hex 16
来源：http://qn.asd995.cn

[R68] 计算文件校验值
来源：http://km.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xb.chemitech.net.cn

[R69] 生成随机密码
来源：http://bw.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://hg.jctech888.com.cn

[R70] 时间戳与互转
来源：http://nv.hahajie.cn

date +%s;  date -d @1700000000
来源：http://px.521024.cn

[R71] 日期格式化
来源：http://hj.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oe.huanxung.cn

[R72] 等待端口就绪
来源：http://ci.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ho.newstarts.cn

[R73] 分割大日志
来源：http://ql.huanxung.cn


<!-- 参考信息 -->