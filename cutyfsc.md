代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://lh.muxihuayi.cn

[Q22] 排序
来源：http://cg.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fa.chemitech.net.cn

[Q23] 分页
来源：http://wr.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://an.muxihuayi.cn

[Q24] 去重
来源：http://bt.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://nb.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://ot.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oa.shtwfgs.cn

[Q26] 计数
来源：http://cu.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://hm.huixiangedu.cn

[Q27] 条件计数
来源：http://fn.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fp.gzmigu.cn

[Q28] 求和与平均
来源：http://gr.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qj.asd995.cn

[Q29] 最大最小值
来源：http://po.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ca.huixiangedu.cn

[Q30] 分组统计
来源：http://kb.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vr.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://vz.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wu.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://ca.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mj.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://il.huanxung.cn

[Q33] 多列分组
来源：http://wk.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oy.chemitech.net.cn

[Q34] 每组取第一条
来源：http://xa.nicolike.cn

SELECT * FROM (
来源：http://kn.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://py.huanxung.cn

) t WHERE rn = 1;
来源：http://gr.shxzukj.cn

[Q35] 内连接
来源：http://zg.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gi.wgjwhj.cn

[Q36] 左连接
来源：http://uq.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ui.bjjhwx.cn

[Q37] 右连接
来源：http://cu.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cr.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qh.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://us.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://lb.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bj.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pr.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bp.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yf.lnxyls.cn

[Q41] 多表连接
来源：http://xv.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ep.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://ec.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://gz.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://ti.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://io.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yy.colortex.cn

[Q43] 标量子查询
来源：http://up.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://be.wgjwhj.cn

[Q44] IN 子查询
来源：http://fp.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ah.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://pl.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nz.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ht.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eo.gzmigu.cn

[Q47] 与平均值比较
来源：http://do.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ts.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://uj.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hv.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://yx.chemitech.net.cn

[Q49] 更新单行
来源：http://bx.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jb.hahajie.cn

[Q50] 批量更新
来源：http://bt.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ml.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://jt.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vv.bookmarksfly.cn

[Q52] 删除指定行
来源：http://hd.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://gq.jctech888.com.cn

[Q53] 按条件删除
来源：http://ry.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uu.nicolike.cn

[Q54] 清空表
来源：http://fy.nszjky.cn

TRUNCATE TABLE logs;
来源：http://qu.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://yg.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jg.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://ly.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://se.szxytkj.cn

[Q57] 行号
来源：http://ni.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xj.chemitech.net.cn

[Q58] 累计求和
来源：http://sb.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ay.nicolike.cn

[Q59] 分组内累计
来源：http://qm.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rz.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://mt.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bh.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xq.lnxyls.cn

[Q61] 移动平均
来源：http://tt.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://to.nszjky.cn

[Q62] 分组占比
来源：http://dk.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hp.szxytkj.cn

[Q63] 开启事务
来源：http://qk.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vl.shxzskj.cn

[Q64] 提交事务
来源：http://dt.9csxet.cn

COMMIT;
来源：http://ud.lnxyls.cn

[Q65] 回滚事务
来源：http://xz.gzmigu.cn

ROLLBACK;
来源：http://ke.lnxyls.cn

[Q66] 行锁查询
来源：http://hf.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://dq.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bx.nicolike.cn

[Q68] 保存点
来源：http://ab.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://hs.lnxyls.cn

ROLLBACK TO sp1;
来源：http://mu.shxzskj.cn

[Q69] 查看执行计划
来源：http://dm.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ee.szsharing.cn

[Q70] 更新统计信息
来源：http://br.huixiangedu.cn

ANALYZE TABLE users;
来源：http://hy.newstarts.cn

[Q71] 查看建表语句
来源：http://mc.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ku.gzmigu.cn

[Q72] 查看索引
来源：http://mc.colortex.cn

SHOW INDEX FROM users;
来源：http://uq.hahajie.cn

[Q73] 查看表状态
来源：http://yp.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hv.wgjwhj.cn

[Q74] 强制使用索引
来源：http://rn.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cf.shxzskj.cn

[Q75] 日期格式化
来源：http://mn.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cw.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://op.chemitech.net.cn

[Q76] 按天统计
来源：http://dr.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wm.shtwfgs.cn

[Q77] 时间加减
来源：http://rk.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dj.szsharing.cn

[Q78] 当前时间
来源：http://aw.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://da.shxzskj.cn

[Q79] 字符串拼接
来源：http://rn.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yg.nszjky.cn

[Q80] 字符串截取
来源：http://wm.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ye.colortex.cn

[Q81] 字符串替换
来源：http://td.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mu.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://aa.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ha.gzmigu.cn

[Q83] 大小写转换
来源：http://wn.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ih.colortex.cn

[Q84] 去除首尾空格
来源：http://mn.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://vp.wgjwhj.cn

[Q85] 数值取整
来源：http://xw.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gg.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://ik.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ki.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://zb.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iw.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://fy.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fe.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ql.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://jw.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uo.521024.cn

[Q90] 生成序号列
来源：http://pr.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ni.yuntaijiaju.cn

================================================================================
来源：http://rx.gzmigu.cn

R. Bash 专题
来源：http://bk.gzmigu.cn

================================================================================
来源：http://xt.521024.cn

[R01] shebang 与严格模式
来源：http://vp.panjiajie.cn

#!/usr/bin/env bash
来源：http://po.bookmarksfly.cn

set -euo pipefail
来源：http://xm.hnjuh.cn

[R02] 变量赋值与使用
来源：http://fr.newstarts.cn

name="Tom"; echo "$name"
来源：http://iy.shtwfgs.cn

[R03] 只读变量
来源：http://wc.shxzskj.cn

readonly PI=3.14
来源：http://nt.nszjky.cn

[R04] 位置参数
来源：http://ax.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lm.huixiangedu.cn

[R05] 参数默认值
来源：http://fb.lnxyls.cn

name="${1:-default}"
来源：http://to.hahajie.cn

[R06] 判断命令是否存在
来源：http://of.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jn.szsharing.cn

[R07] if 判断文件
来源：http://ra.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xz.huanxung.cn

[R08] 数值比较
来源：http://ya.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ct.shtwfgs.cn

[R09] 字符串比较
来源：http://au.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ih.szxytkj.cn

[R10] 正则匹配
来源：http://xj.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://es.hnjuh.cn

[R11] case 多分支
来源：http://oe.yuexingan06.cn

case "$1" in
来源：http://bz.hnjuh.cn

start) echo "启动" ;;
来源：http://xs.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://ax.newstarts.cn

*)     echo "未知命令" ;;
来源：http://sy.huanxung.cn

esac
来源：http://ed.shxzukj.cn

[R12] for 遍历文件
来源：http://pu.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://de.bookmarksfly.cn

[R13] for 计数循环
来源：http://cq.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://kk.chemitech.net.cn

[R14] C 风格 for
来源：http://ss.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ul.hahajie.cn

[R15] while 逐行读文件
来源：http://gp.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hq.asd995.cn

[R16] until 等待条件
来源：http://ri.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iz.haigaiapp.cn

[R17] 数组定义与取值
来源：http://hk.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://er.bookmarksfly.cn

[R18] 遍历数组
来源：http://jj.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lt.newstarts.cn

[R19] 数组长度
来源：http://es.huixiangedu.cn

echo "${#arr[@]}"
来源：http://zs.colortex.cn

[R20] 关联数组（字典）
来源：http://du.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gc.nicolike.cn

[R21] 字符串长度
来源：http://qn.yuexingan06.cn

echo "${#s}"
来源：http://je.chemitech.net.cn

[R22] 截取子串
来源：http://gg.bjjhwx.cn

echo "${s:0:5}"
来源：http://sn.shxzukj.cn

[R23] 字符串替换
来源：http://jw.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yb.shxzskj.cn

[R24] 大小写转换
来源：http://dv.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ep.521024.cn

[R25] 去后缀 / 去前缀
来源：http://bk.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tv.szsharing.cn

[R26] 命令替换
来源：http://zu.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://rk.huixiangedu.cn

[R27] 算术展开
来源：http://wj.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://lx.colortex.cn

[R28] 浮点运算
来源：http://id.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://io.newstarts.cn

[R29] 定义函数
来源：http://ma.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dl.colortex.cn

[R30] 函数返回状态码
来源：http://dj.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://ma.jctech888.com.cn

[R31] 局部变量
来源：http://dp.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://gg.9csxet.cn

[R32] 参数个数校验
来源：http://sj.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qq.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://no.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rp.newstarts.cn

[R34] 退出时清理
来源：http://dw.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rs.9csxet.cn

[R35] 后台执行并等待
来源：http://ww.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kv.shxzskj.cn

[R36] 并发执行多个任务
来源：http://be.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yr.521024.cn

[R37] 把输出赋给变量
来源：http://fd.szxytkj.cn

files=$(ls -1)
来源：http://fx.yuntaijiaju.cn

[R38] 管道串联
来源：http://ho.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://uj.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://si.colortex.cn

cmd > out.log 2>&1
来源：http://xm.huanxung.cn

[R40] 追加写日志
来源：http://ng.jctech888.com.cn

echo "log" >> out.log
来源：http://at.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://pj.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://nv.hahajie.cn

[R42] 输入重定向
来源：http://jp.colortex.cn

wc -l < a.txt
来源：http://ro.nszjky.cn

[R43] 按名字查找文件
来源：http://mo.huanxung.cn

find . -name "*.log" -type f
来源：http://cu.newstarts.cn

[R44] 按修改时间查找
来源：http://bm.wgjwhj.cn

find . -mtime -7 -type f
来源：http://mb.lnxyls.cn

[R45] 批量删除
来源：http://hg.asd995.cn

find . -name "*.tmp" -delete
来源：http://it.nicolike.cn

[R46] 递归替换文件内容
来源：http://gi.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://po.bjjhwx.cn

[R47] sed 单行替换
来源：http://we.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hz.asd995.cn

[R48] awk 取指定列
来源：http://jx.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://tj.lnxyls.cn

[R49] awk 带条件
来源：http://qa.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oq.9csxet.cn

[R50] awk 求和
来源：http://os.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zi.bjjhwx.cn

[R51] 排序去重取前几
来源：http://hd.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://an.gzmigu.cn

[R52] 统计行数
来源：http://ld.hahajie.cn

wc -l a.txt
来源：http://um.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://rm.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://om.nicolike.cn

[R54] 比较两个文件
来源：http://hy.huanxung.cn

diff a.txt b.txt
来源：http://gz.bjjhwx.cn

[R55] 压缩与解压
来源：http://gk.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://my.panjiajie.cn

[R56] 远程拷贝
来源：http://mk.asd995.cn

scp file user@host:/path/
来源：http://ca.521024.cn

[R57] 远程执行命令
来源：http://en.huanxung.cn

ssh user@host 'uptime'
来源：http://ks.huixinmuqiang.cn

[R58] 下载文件
来源：http://eq.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kb.521024.cn

[R59] 发 POST JSON
来源：http://tv.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pc.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://rx.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vx.hahajie.cn

[R61] 磁盘占用
来源：http://aq.shxzukj.cn

df -h;  du -sh *
来源：http://eh.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://wh.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://zx.nicolike.cn

[R63] 内存与进程
来源：http://gj.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://kf.wgjwhj.cn

[R64] 结束进程
来源：http://fv.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://vt.szsharing.cn

[R65] 查看端口占用
来源：http://yo.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yv.jctech888.com.cn

[R66] 定时任务
来源：http://bw.hnjuh.cn

crontab -e;  crontab -l
来源：http://td.huanxung.cn

[R67] 生成随机十六进制串
来源：http://ru.hnjuh.cn

openssl rand -hex 16
来源：http://vp.521024.cn

[R68] 计算文件校验值
来源：http://lr.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eu.chemitech.net.cn

[R69] 生成随机密码
来源：http://aj.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://qq.szsharing.cn

[R70] 时间戳与互转
来源：http://wf.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://fe.lnxyls.cn

[R71] 日期格式化
来源：http://vn.9csxet.cn


<!-- 参考信息 -->