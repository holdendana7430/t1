代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lz.asd995.cn

[Q24] 去重
来源：http://il.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://rg.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://yy.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xq.lnxyls.cn

[Q26] 计数
来源：http://tp.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://oy.huixinmuqiang.cn

[Q27] 条件计数
来源：http://kc.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ji.chemitech.net.cn

[Q28] 求和与平均
来源：http://yw.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ke.haigaiapp.cn

[Q29] 最大最小值
来源：http://mw.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dr.wgjwhj.cn

[Q30] 分组统计
来源：http://us.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ri.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://uf.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qb.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://jx.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oa.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cb.bookmarksfly.cn

[Q33] 多列分组
来源：http://uh.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yw.9csxet.cn

[Q34] 每组取第一条
来源：http://vb.huixiangedu.cn

SELECT * FROM (
来源：http://uy.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://di.9csxet.cn

) t WHERE rn = 1;
来源：http://zg.jianghongdianzi.cn

[Q35] 内连接
来源：http://vq.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fw.hnjuh.cn

[Q36] 左连接
来源：http://vj.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xg.9csxet.cn

[Q37] 右连接
来源：http://zo.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aq.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://we.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zk.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://nv.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hf.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://om.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://do.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lk.jianghongdianzi.cn

[Q41] 多表连接
来源：http://tx.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ky.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://cb.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://ok.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://tl.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://wq.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uk.huanxung.cn

[Q43] 标量子查询
来源：http://kk.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ym.colortex.cn

[Q44] IN 子查询
来源：http://sh.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dd.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://jo.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qt.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zt.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sv.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://mk.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://id.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://vc.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ww.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://rx.haigaiapp.cn

[Q49] 更新单行
来源：http://mg.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vs.szxytkj.cn

[Q50] 批量更新
来源：http://ib.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jk.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://ql.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ja.bjjhwx.cn

[Q52] 删除指定行
来源：http://bv.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://nd.szsharing.cn

[Q53] 按条件删除
来源：http://vz.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ki.chemitech.net.cn

[Q54] 清空表
来源：http://iw.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://rr.szsharing.cn

[Q55] 排名（并列占位）
来源：http://uo.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://er.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://vm.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bc.9csxet.cn

[Q57] 行号
来源：http://ly.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hq.yuntaijiaju.cn

[Q58] 累计求和
来源：http://cz.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zl.hahajie.cn

[Q59] 分组内累计
来源：http://oh.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ck.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://zw.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wk.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lu.huixiangedu.cn

[Q61] 移动平均
来源：http://ho.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ab.9csxet.cn

[Q62] 分组占比
来源：http://th.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xj.chemitech.net.cn

[Q63] 开启事务
来源：http://yo.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ao.szxytkj.cn

[Q64] 提交事务
来源：http://xo.521024.cn

COMMIT;
来源：http://jr.hnjuh.cn

[Q65] 回滚事务
来源：http://bm.wgjwhj.cn

ROLLBACK;
来源：http://ma.nicolike.cn

[Q66] 行锁查询
来源：http://zh.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vu.huanxung.cn

[Q67] 设置隔离级别
来源：http://qc.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://so.panjiajie.cn

[Q68] 保存点
来源：http://yg.asd995.cn

SAVEPOINT sp1;
来源：http://dc.huanxung.cn

ROLLBACK TO sp1;
来源：http://iy.newstarts.cn

[Q69] 查看执行计划
来源：http://pi.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ez.gzmigu.cn

[Q70] 更新统计信息
来源：http://ea.huanxung.cn

ANALYZE TABLE users;
来源：http://wz.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://ke.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://in.hahajie.cn

[Q72] 查看索引
来源：http://cr.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://ju.9csxet.cn

[Q73] 查看表状态
来源：http://pl.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mk.huanxung.cn

[Q74] 强制使用索引
来源：http://ho.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xc.chemitech.net.cn

[Q75] 日期格式化
来源：http://hi.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xm.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://am.huanxung.cn

[Q76] 按天统计
来源：http://ve.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://di.yuexingan06.cn

[Q77] 时间加减
来源：http://gu.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lw.yuntaijiaju.cn

[Q78] 当前时间
来源：http://si.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yo.lnxyls.cn

[Q79] 字符串拼接
来源：http://vi.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qx.bookmarksfly.cn

[Q80] 字符串截取
来源：http://oq.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zp.bjjhwx.cn

[Q81] 字符串替换
来源：http://nk.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jz.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://bl.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jf.muxihuayi.cn

[Q83] 大小写转换
来源：http://ql.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bq.nicolike.cn

[Q84] 去除首尾空格
来源：http://ta.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://gi.shtwfgs.cn

[Q85] 数值取整
来源：http://qn.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cf.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://be.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tk.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://my.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kh.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://eg.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://in.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oc.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://lb.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xf.panjiajie.cn

[Q90] 生成序号列
来源：http://yw.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jj.huixiangedu.cn

================================================================================
来源：http://ow.shtwfgs.cn

R. Bash 专题
来源：http://dt.haigaiapp.cn

================================================================================
来源：http://wl.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://mo.yuexingan06.cn

#!/usr/bin/env bash
来源：http://kj.hahajie.cn

set -euo pipefail
来源：http://he.asd995.cn

[R02] 变量赋值与使用
来源：http://ll.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://sl.lnxyls.cn

[R03] 只读变量
来源：http://ry.muxihuayi.cn

readonly PI=3.14
来源：http://xl.newstarts.cn

[R04] 位置参数
来源：http://gq.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nl.hnjuh.cn

[R05] 参数默认值
来源：http://ym.shtwfgs.cn

name="${1:-default}"
来源：http://oy.newstarts.cn

[R06] 判断命令是否存在
来源：http://zi.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uc.muxihuayi.cn

[R07] if 判断文件
来源：http://gx.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ry.colortex.cn

[R08] 数值比较
来源：http://im.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cq.newstarts.cn

[R09] 字符串比较
来源：http://ol.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aa.chemitech.net.cn

[R10] 正则匹配
来源：http://og.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oi.newstarts.cn

[R11] case 多分支
来源：http://on.newstarts.cn

case "$1" in
来源：http://ce.521024.cn

start) echo "启动" ;;
来源：http://sn.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://qs.9csxet.cn

*)     echo "未知命令" ;;
来源：http://eo.huixinmuqiang.cn

esac
来源：http://is.szxytkj.cn

[R12] for 遍历文件
来源：http://if.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://jo.yuexingan06.cn

[R13] for 计数循环
来源：http://ob.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://wz.yuntaijiaju.cn

[R14] C 风格 for
来源：http://ch.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vg.nszjky.cn

[R15] while 逐行读文件
来源：http://bp.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yy.bookmarksfly.cn

[R16] until 等待条件
来源：http://wa.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ev.gzmigu.cn

[R17] 数组定义与取值
来源：http://tu.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zh.huixiangedu.cn

[R18] 遍历数组
来源：http://jj.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fz.bjjhwx.cn

[R19] 数组长度
来源：http://ny.huixiangedu.cn

echo "${#arr[@]}"
来源：http://dl.colortex.cn

[R20] 关联数组（字典）
来源：http://rv.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hs.hnjuh.cn

[R21] 字符串长度
来源：http://tb.521024.cn

echo "${#s}"
来源：http://gi.yuexingan06.cn

[R22] 截取子串
来源：http://gr.newstarts.cn

echo "${s:0:5}"
来源：http://lo.huixinmuqiang.cn

[R23] 字符串替换
来源：http://bf.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lc.haigaiapp.cn

[R24] 大小写转换
来源：http://bw.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vn.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://gs.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bh.asd995.cn

[R26] 命令替换
来源：http://ao.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://ju.huixiangedu.cn

[R27] 算术展开
来源：http://xt.nszjky.cn

echo $((1 + 2 * 3))
来源：http://sg.nszjky.cn

[R28] 浮点运算
来源：http://lu.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://ww.haigaiapp.cn

[R29] 定义函数
来源：http://hq.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ss.wgjwhj.cn

[R30] 函数返回状态码
来源：http://jz.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://el.shxzukj.cn

[R31] 局部变量
来源：http://ol.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://sj.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://oj.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zw.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://pv.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ex.yuntaijiaju.cn

[R34] 退出时清理
来源：http://vu.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ad.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://nd.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pf.521024.cn

[R36] 并发执行多个任务
来源：http://we.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ah.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://xs.lnxyls.cn

files=$(ls -1)
来源：http://if.bjjhwx.cn

[R38] 管道串联
来源：http://nf.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://zr.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://pb.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://ei.yuexingan06.cn

[R40] 追加写日志
来源：http://pz.huixinmuqiang.cn

echo "log" >> out.log
来源：http://yq.bjjhwx.cn

[R41] 丢弃输出
来源：http://td.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://is.szxytkj.cn

[R42] 输入重定向
来源：http://cs.muxihuayi.cn

wc -l < a.txt
来源：http://fb.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://rj.nszjky.cn

find . -name "*.log" -type f
来源：http://wl.huixiangedu.cn

[R44] 按修改时间查找
来源：http://cc.nicolike.cn

find . -mtime -7 -type f
来源：http://dz.shxzskj.cn

[R45] 批量删除
来源：http://my.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://pu.521024.cn

[R46] 递归替换文件内容
来源：http://lh.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tu.asd995.cn

[R47] sed 单行替换
来源：http://va.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xl.9csxet.cn

[R48] awk 取指定列
来源：http://ts.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://jy.szsharing.cn

[R49] awk 带条件
来源：http://kk.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://es.wgjwhj.cn

[R50] awk 求和
来源：http://wf.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kn.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://uz.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ll.panjiajie.cn

[R52] 统计行数
来源：http://wn.521024.cn

wc -l a.txt
来源：http://ks.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://mb.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pb.jctech888.com.cn

[R54] 比较两个文件
来源：http://dw.huixinmuqiang.cn

diff a.txt b.txt
来源：http://pn.lnxyls.cn

[R55] 压缩与解压
来源：http://ky.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://af.hnjuh.cn

[R56] 远程拷贝
来源：http://wm.nicolike.cn

scp file user@host:/path/
来源：http://bt.gzmigu.cn

[R57] 远程执行命令
来源：http://sf.yuexingan06.cn

ssh user@host 'uptime'
来源：http://jl.hahajie.cn

[R58] 下载文件
来源：http://ds.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qm.shtwfgs.cn

[R59] 发 POST JSON
来源：http://ag.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wm.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://ly.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://py.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://kg.bookmarksfly.cn

df -h;  du -sh *
来源：http://dy.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://fb.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://de.huixiangedu.cn

[R63] 内存与进程
来源：http://th.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://cu.9csxet.cn

[R64] 结束进程
来源：http://tv.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://lj.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://zm.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ss.nszjky.cn

[R66] 定时任务
来源：http://mp.nszjky.cn

crontab -e;  crontab -l
来源：http://kh.asd995.cn

[R67] 生成随机十六进制串
来源：http://ci.shxzskj.cn

openssl rand -hex 16
来源：http://eh.colortex.cn

[R68] 计算文件校验值
来源：http://fr.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ch.hnjuh.cn

[R69] 生成随机密码
来源：http://rg.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://pe.szxytkj.cn

[R70] 时间戳与互转
来源：http://ud.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://le.huixiangedu.cn

[R71] 日期格式化
来源：http://qv.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ee.hahajie.cn

[R72] 等待端口就绪
来源：http://nc.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qy.shtwfgs.cn

[R73] 分割大日志
来源：http://jy.huixinmuqiang.cn


<!-- 参考信息 -->