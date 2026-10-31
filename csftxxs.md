代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pq.shxzukj.cn

[Q20] IN 列表
来源：http://sr.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kx.9csxet.cn

[Q21] 空值判断
来源：http://dt.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sw.jctech888.com.cn

[Q22] 排序
来源：http://gh.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ds.lnxyls.cn

[Q23] 分页
来源：http://hw.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ym.huanxung.cn

[Q24] 去重
来源：http://uj.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://pj.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://lk.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eo.panjiajie.cn

[Q26] 计数
来源：http://cm.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://gq.hnjuh.cn

[Q27] 条件计数
来源：http://pi.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ll.9csxet.cn

[Q28] 求和与平均
来源：http://ig.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sg.nicolike.cn

[Q29] 最大最小值
来源：http://da.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cs.521024.cn

[Q30] 分组统计
来源：http://nj.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qa.colortex.cn

[Q31] 分组后过滤
来源：http://ko.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iz.hahajie.cn

[Q32] 分组拼接字符串
来源：http://bv.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fl.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mi.szsharing.cn

[Q33] 多列分组
来源：http://wc.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://km.gzmigu.cn

[Q34] 每组取第一条
来源：http://jm.hahajie.cn

SELECT * FROM (
来源：http://nn.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oc.bjjhwx.cn

) t WHERE rn = 1;
来源：http://dr.huixinmuqiang.cn

[Q35] 内连接
来源：http://vd.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mf.huixinmuqiang.cn

[Q36] 左连接
来源：http://yc.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jd.huixinmuqiang.cn

[Q37] 右连接
来源：http://to.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oo.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mp.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xc.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://vf.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rb.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ln.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yx.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lm.panjiajie.cn

[Q41] 多表连接
来源：http://qo.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wj.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://lp.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://mb.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://jy.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://pl.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://os.panjiajie.cn

[Q43] 标量子查询
来源：http://dm.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dj.chemitech.net.cn

[Q44] IN 子查询
来源：http://gd.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jh.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://hl.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ki.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bk.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uy.lnxyls.cn

[Q47] 与平均值比较
来源：http://bp.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://si.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://zz.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ce.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://mo.newstarts.cn

[Q49] 更新单行
来源：http://fw.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aw.shxzukj.cn

[Q50] 批量更新
来源：http://dz.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://na.shtwfgs.cn

[Q51] 用子查询更新
来源：http://up.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://io.shxzskj.cn

[Q52] 删除指定行
来源：http://fy.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://ku.yuexingan06.cn

[Q53] 按条件删除
来源：http://zo.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rz.colortex.cn

[Q54] 清空表
来源：http://mc.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://hp.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://dr.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bp.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://ot.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uo.huixiangedu.cn

[Q57] 行号
来源：http://hq.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jm.9csxet.cn

[Q58] 累计求和
来源：http://mr.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ko.chemitech.net.cn

[Q59] 分组内累计
来源：http://lg.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sn.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://aq.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vd.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fs.asd995.cn

[Q61] 移动平均
来源：http://pi.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ua.shtwfgs.cn

[Q62] 分组占比
来源：http://ov.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://al.nicolike.cn

[Q63] 开启事务
来源：http://fc.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vq.shxzskj.cn

[Q64] 提交事务
来源：http://zv.panjiajie.cn

COMMIT;
来源：http://mg.haigaiapp.cn

[Q65] 回滚事务
来源：http://vs.chemitech.net.cn

ROLLBACK;
来源：http://bc.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://tt.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://di.lnxyls.cn

[Q67] 设置隔离级别
来源：http://ew.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ou.newstarts.cn

[Q68] 保存点
来源：http://gz.jctech888.com.cn

SAVEPOINT sp1;
来源：http://wt.gzmigu.cn

ROLLBACK TO sp1;
来源：http://je.hnjuh.cn

[Q69] 查看执行计划
来源：http://lq.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rf.panjiajie.cn

[Q70] 更新统计信息
来源：http://sz.9csxet.cn

ANALYZE TABLE users;
来源：http://qy.jctech888.com.cn

[Q71] 查看建表语句
来源：http://go.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tr.nszjky.cn

[Q72] 查看索引
来源：http://xb.shxzukj.cn

SHOW INDEX FROM users;
来源：http://iu.hnjuh.cn

[Q73] 查看表状态
来源：http://xm.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fg.huixiangedu.cn

[Q74] 强制使用索引
来源：http://it.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://al.wgjwhj.cn

[Q75] 日期格式化
来源：http://ge.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://js.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gj.szsharing.cn

[Q76] 按天统计
来源：http://wh.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hg.asd995.cn

[Q77] 时间加减
来源：http://ns.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jy.shxzskj.cn

[Q78] 当前时间
来源：http://tu.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ol.yuexingan06.cn

[Q79] 字符串拼接
来源：http://pz.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jo.shxzukj.cn

[Q80] 字符串截取
来源：http://dt.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://um.wgjwhj.cn

[Q81] 字符串替换
来源：http://zs.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tg.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://bn.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uw.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://kt.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://go.hahajie.cn

[Q84] 去除首尾空格
来源：http://gk.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://my.521024.cn

[Q85] 数值取整
来源：http://eb.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cg.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://wi.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eq.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://xf.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sv.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://zk.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jl.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lp.nicolike.cn

[Q89] 判断表是否存在
来源：http://ys.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zy.jctech888.com.cn

[Q90] 生成序号列
来源：http://vf.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ke.jctech888.com.cn

================================================================================
来源：http://vc.yuexingan06.cn

R. Bash 专题
来源：http://sh.nicolike.cn

================================================================================
来源：http://xa.newstarts.cn

[R01] shebang 与严格模式
来源：http://zo.hnjuh.cn

#!/usr/bin/env bash
来源：http://wg.colortex.cn

set -euo pipefail
来源：http://wu.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://ik.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://lm.9csxet.cn

[R03] 只读变量
来源：http://qu.shxzskj.cn

readonly PI=3.14
来源：http://yg.panjiajie.cn

[R04] 位置参数
来源：http://ab.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yr.lnxyls.cn

[R05] 参数默认值
来源：http://ye.shtwfgs.cn

name="${1:-default}"
来源：http://vt.nicolike.cn

[R06] 判断命令是否存在
来源：http://ix.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gh.newstarts.cn

[R07] if 判断文件
来源：http://me.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pr.nszjky.cn

[R08] 数值比较
来源：http://nc.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qg.shxzskj.cn

[R09] 字符串比较
来源：http://yy.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cr.bookmarksfly.cn

[R10] 正则匹配
来源：http://op.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yz.shtwfgs.cn

[R11] case 多分支
来源：http://kn.newstarts.cn

case "$1" in
来源：http://dg.jctech888.com.cn

start) echo "启动" ;;
来源：http://mt.nicolike.cn

stop)  echo "停止" ;;
来源：http://vr.9csxet.cn

*)     echo "未知命令" ;;
来源：http://yr.shtwfgs.cn

esac
来源：http://aw.shtwfgs.cn

[R12] for 遍历文件
来源：http://po.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://hz.521024.cn

[R13] for 计数循环
来源：http://pc.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://tc.haigaiapp.cn

[R14] C 风格 for
来源：http://zx.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kz.shtwfgs.cn

[R15] while 逐行读文件
来源：http://yd.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xq.gzmigu.cn

[R16] until 等待条件
来源：http://la.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mm.jctech888.com.cn

[R17] 数组定义与取值
来源：http://ou.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fq.szxytkj.cn

[R18] 遍历数组
来源：http://eq.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vq.hahajie.cn

[R19] 数组长度
来源：http://au.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://zw.asd995.cn

[R20] 关联数组（字典）
来源：http://mq.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iw.haigaiapp.cn

[R21] 字符串长度
来源：http://qi.hahajie.cn

echo "${#s}"
来源：http://fp.gzmigu.cn

[R22] 截取子串
来源：http://es.huixiangedu.cn

echo "${s:0:5}"
来源：http://zz.huixinmuqiang.cn

[R23] 字符串替换
来源：http://wv.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vf.huixinmuqiang.cn

[R24] 大小写转换
来源：http://vt.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ru.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://zv.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rg.nszjky.cn

[R26] 命令替换
来源：http://wm.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://gx.shxzukj.cn

[R27] 算术展开
来源：http://ku.nszjky.cn

echo $((1 + 2 * 3))
来源：http://ui.asd995.cn

[R28] 浮点运算
来源：http://pj.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://vi.chemitech.net.cn

[R29] 定义函数
来源：http://qm.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wr.9csxet.cn

[R30] 函数返回状态码
来源：http://po.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://hy.yuexingan06.cn

[R31] 局部变量
来源：http://ad.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://xf.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://ok.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kf.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://rm.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lf.asd995.cn

[R34] 退出时清理
来源：http://ae.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gc.lnxyls.cn

[R35] 后台执行并等待
来源：http://zn.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sq.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://zd.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ni.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://gj.chemitech.net.cn

files=$(ls -1)
来源：http://ot.szsharing.cn

[R38] 管道串联
来源：http://gi.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://nr.colortex.cn

[R39] 重定向标准输出与错误
来源：http://qi.shxzskj.cn

cmd > out.log 2>&1
来源：http://qg.panjiajie.cn

[R40] 追加写日志
来源：http://dm.hnjuh.cn

echo "log" >> out.log
来源：http://zw.bjjhwx.cn

[R41] 丢弃输出
来源：http://go.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://ee.bjjhwx.cn

[R42] 输入重定向
来源：http://eg.shxzukj.cn

wc -l < a.txt
来源：http://rm.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://ij.hnjuh.cn

find . -name "*.log" -type f
来源：http://wo.bjjhwx.cn

[R44] 按修改时间查找
来源：http://ke.huixiangedu.cn

find . -mtime -7 -type f
来源：http://tw.wgjwhj.cn

[R45] 批量删除
来源：http://vp.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://bq.nicolike.cn

[R46] 递归替换文件内容
来源：http://mo.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cl.wgjwhj.cn

[R47] sed 单行替换
来源：http://lc.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ly.bookmarksfly.cn

[R48] awk 取指定列
来源：http://vq.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://zf.9csxet.cn

[R49] awk 带条件
来源：http://vm.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zc.panjiajie.cn

[R50] awk 求和
来源：http://lv.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cp.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://fc.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mz.shtwfgs.cn

[R52] 统计行数
来源：http://nk.gzmigu.cn

wc -l a.txt
来源：http://pb.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://an.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wx.asd995.cn

[R54] 比较两个文件
来源：http://yn.colortex.cn

diff a.txt b.txt
来源：http://wo.hahajie.cn

[R55] 压缩与解压
来源：http://ma.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lp.bookmarksfly.cn

[R56] 远程拷贝
来源：http://kp.bookmarksfly.cn

scp file user@host:/path/
来源：http://re.9csxet.cn

[R57] 远程执行命令
来源：http://iz.hahajie.cn

ssh user@host 'uptime'
来源：http://ki.bjjhwx.cn

[R58] 下载文件
来源：http://vm.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rx.jctech888.com.cn

[R59] 发 POST JSON
来源：http://zx.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xv.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://hh.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bo.chemitech.net.cn

[R61] 磁盘占用
来源：http://lb.huixinmuqiang.cn

df -h;  du -sh *
来源：http://ph.lnxyls.cn

[R62] 找最占空间的文件
来源：http://vi.colortex.cn

du -ah . | sort -rh | head -10
来源：http://ya.wgjwhj.cn

[R63] 内存与进程
来源：http://lr.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://jo.yuntaijiaju.cn

[R64] 结束进程
来源：http://mb.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://xx.chemitech.net.cn

[R65] 查看端口占用
来源：http://vp.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mv.huixiangedu.cn

[R66] 定时任务
来源：http://lz.asd995.cn

crontab -e;  crontab -l
来源：http://it.nszjky.cn

[R67] 生成随机十六进制串
来源：http://bp.nszjky.cn

openssl rand -hex 16
来源：http://ns.yuexingan06.cn

[R68] 计算文件校验值
来源：http://pm.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tk.nicolike.cn

[R69] 生成随机密码
来源：http://nl.jctech888.com.cn


<!-- 参考信息 -->