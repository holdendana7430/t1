代发 wailian999

SELECT * FROM users;
来源：http://zj.szxytkj.cn

[Q16] 查询指定列
来源：http://zt.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://gw.colortex.cn

[Q17] 条件查询
来源：http://qz.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wh.yuexingan06.cn

[Q18] 模糊匹配
来源：http://om.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jc.shxzukj.cn

[Q19] 范围查询
来源：http://ml.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xu.wgjwhj.cn

[Q20] IN 列表
来源：http://bi.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fn.hahajie.cn

[Q21] 空值判断
来源：http://ez.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://df.szsharing.cn

[Q22] 排序
来源：http://yc.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mj.nicolike.cn

[Q23] 分页
来源：http://ko.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jh.chemitech.net.cn

[Q24] 去重
来源：http://nx.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://aa.newstarts.cn

[Q25] 只取前 N 条
来源：http://ue.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://we.szsharing.cn

[Q26] 计数
来源：http://gh.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://dm.newstarts.cn

[Q27] 条件计数
来源：http://fq.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nw.chemitech.net.cn

[Q28] 求和与平均
来源：http://tr.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ma.hnjuh.cn

[Q29] 最大最小值
来源：http://pv.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jm.wgjwhj.cn

[Q30] 分组统计
来源：http://yh.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wz.hahajie.cn

[Q31] 分组后过滤
来源：http://is.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dv.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://fe.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ip.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://da.hnjuh.cn

[Q33] 多列分组
来源：http://ml.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lm.shtwfgs.cn

[Q34] 每组取第一条
来源：http://uu.muxihuayi.cn

SELECT * FROM (
来源：http://gh.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vf.lnxyls.cn

) t WHERE rn = 1;
来源：http://ty.asd995.cn

[Q35] 内连接
来源：http://pi.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ra.yuexingan06.cn

[Q36] 左连接
来源：http://ou.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://md.shxzskj.cn

[Q37] 右连接
来源：http://jp.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jo.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gt.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pp.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://ko.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qj.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tj.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vl.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pa.huixiangedu.cn

[Q41] 多表连接
来源：http://oa.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jh.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://kv.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://gt.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://pc.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://he.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mz.chemitech.net.cn

[Q43] 标量子查询
来源：http://ro.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://do.shxzukj.cn

[Q44] IN 子查询
来源：http://fu.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ka.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://nb.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zl.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sy.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ve.9csxet.cn

[Q47] 与平均值比较
来源：http://ya.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ye.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://bp.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dl.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://fs.bookmarksfly.cn

[Q49] 更新单行
来源：http://dd.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ow.yuntaijiaju.cn

[Q50] 批量更新
来源：http://hi.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oe.szsharing.cn

[Q51] 用子查询更新
来源：http://tz.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iz.nszjky.cn

[Q52] 删除指定行
来源：http://xo.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://bw.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://wc.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mu.yuntaijiaju.cn

[Q54] 清空表
来源：http://xh.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://bx.9csxet.cn

[Q55] 排名（并列占位）
来源：http://lk.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gn.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://oy.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dy.gzmigu.cn

[Q57] 行号
来源：http://tz.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iy.haigaiapp.cn

[Q58] 累计求和
来源：http://om.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eg.chemitech.net.cn

[Q59] 分组内累计
来源：http://oo.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qx.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://nf.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qf.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zi.chemitech.net.cn

[Q61] 移动平均
来源：http://he.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ik.wgjwhj.cn

[Q62] 分组占比
来源：http://ic.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qh.muxihuayi.cn

[Q63] 开启事务
来源：http://he.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ap.hahajie.cn

[Q64] 提交事务
来源：http://gp.wgjwhj.cn

COMMIT;
来源：http://oy.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://ec.muxihuayi.cn

ROLLBACK;
来源：http://li.wgjwhj.cn

[Q66] 行锁查询
来源：http://fe.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rd.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://le.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ol.521024.cn

[Q68] 保存点
来源：http://sc.bjjhwx.cn

SAVEPOINT sp1;
来源：http://mp.panjiajie.cn

ROLLBACK TO sp1;
来源：http://nn.521024.cn

[Q69] 查看执行计划
来源：http://xs.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yg.jctech888.com.cn

[Q70] 更新统计信息
来源：http://tp.hahajie.cn

ANALYZE TABLE users;
来源：http://be.nicolike.cn

[Q71] 查看建表语句
来源：http://zh.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ng.hnjuh.cn

[Q72] 查看索引
来源：http://pw.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://df.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://ck.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jl.shxzukj.cn

[Q74] 强制使用索引
来源：http://mq.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cc.huixiangedu.cn

[Q75] 日期格式化
来源：http://dj.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wx.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zf.521024.cn

[Q76] 按天统计
来源：http://ek.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kn.huixiangedu.cn

[Q77] 时间加减
来源：http://kn.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jl.nszjky.cn

[Q78] 当前时间
来源：http://dt.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wr.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://np.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gt.wgjwhj.cn

[Q80] 字符串截取
来源：http://wt.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ir.panjiajie.cn

[Q81] 字符串替换
来源：http://jp.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kt.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://ds.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fs.muxihuayi.cn

[Q83] 大小写转换
来源：http://gb.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kp.huanxung.cn

[Q84] 去除首尾空格
来源：http://ui.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://ih.shtwfgs.cn

[Q85] 数值取整
来源：http://gt.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rq.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://kf.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qc.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://ti.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dv.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://de.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pz.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://an.shxzskj.cn

[Q89] 判断表是否存在
来源：http://lh.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ii.gzmigu.cn

[Q90] 生成序号列
来源：http://pp.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ev.hnjuh.cn

================================================================================
来源：http://tc.hnjuh.cn

R. Bash 专题
来源：http://vu.521024.cn

================================================================================
来源：http://xx.shxzukj.cn

[R01] shebang 与严格模式
来源：http://se.wgjwhj.cn

#!/usr/bin/env bash
来源：http://hr.hahajie.cn

set -euo pipefail
来源：http://ug.shxzukj.cn

[R02] 变量赋值与使用
来源：http://yt.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://yx.yuntaijiaju.cn

[R03] 只读变量
来源：http://jd.gzmigu.cn

readonly PI=3.14
来源：http://nt.colortex.cn

[R04] 位置参数
来源：http://yd.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uo.asd995.cn

[R05] 参数默认值
来源：http://md.wgjwhj.cn

name="${1:-default}"
来源：http://yf.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://bd.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xz.hahajie.cn

[R07] if 判断文件
来源：http://ma.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gg.asd995.cn

[R08] 数值比较
来源：http://ge.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hg.bjjhwx.cn

[R09] 字符串比较
来源：http://zx.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zv.szsharing.cn

[R10] 正则匹配
来源：http://sj.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vi.wgjwhj.cn

[R11] case 多分支
来源：http://hz.chemitech.net.cn

case "$1" in
来源：http://ow.panjiajie.cn

start) echo "启动" ;;
来源：http://mp.shxzukj.cn

stop)  echo "停止" ;;
来源：http://qa.nszjky.cn

*)     echo "未知命令" ;;
来源：http://bd.gzmigu.cn

esac
来源：http://oh.shxzskj.cn

[R12] for 遍历文件
来源：http://kl.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://cl.jianghongdianzi.cn

[R13] for 计数循环
来源：http://xq.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://xz.jianghongdianzi.cn

[R14] C 风格 for
来源：http://fs.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hu.chemitech.net.cn

[R15] while 逐行读文件
来源：http://ba.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tx.muxihuayi.cn

[R16] until 等待条件
来源：http://za.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sr.shtwfgs.cn

[R17] 数组定义与取值
来源：http://ux.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ne.hahajie.cn

[R18] 遍历数组
来源：http://ph.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uc.gzmigu.cn

[R19] 数组长度
来源：http://gv.shxzukj.cn

echo "${#arr[@]}"
来源：http://mp.newstarts.cn

[R20] 关联数组（字典）
来源：http://fv.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ps.bookmarksfly.cn

[R21] 字符串长度
来源：http://lk.bookmarksfly.cn

echo "${#s}"
来源：http://gm.yuntaijiaju.cn

[R22] 截取子串
来源：http://se.521024.cn

echo "${s:0:5}"
来源：http://qc.jianghongdianzi.cn

[R23] 字符串替换
来源：http://kp.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://de.yuexingan06.cn

[R24] 大小写转换
来源：http://pc.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://av.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://do.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://za.huixinmuqiang.cn

[R26] 命令替换
来源：http://dm.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://la.521024.cn

[R27] 算术展开
来源：http://dj.9csxet.cn

echo $((1 + 2 * 3))
来源：http://yc.shxzukj.cn

[R28] 浮点运算
来源：http://iz.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://xo.panjiajie.cn

[R29] 定义函数
来源：http://gl.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ot.muxihuayi.cn

[R30] 函数返回状态码
来源：http://vb.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://rn.szsharing.cn

[R31] 局部变量
来源：http://vf.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://ru.hahajie.cn

[R32] 参数个数校验
来源：http://ou.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gb.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://bp.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://db.hnjuh.cn

[R34] 退出时清理
来源：http://ff.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fl.gzmigu.cn

[R35] 后台执行并等待
来源：http://gb.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ui.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://ft.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lk.hnjuh.cn

[R37] 把输出赋给变量
来源：http://tn.521024.cn

files=$(ls -1)
来源：http://ai.yuntaijiaju.cn

[R38] 管道串联
来源：http://mu.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://dn.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://zp.hahajie.cn

cmd > out.log 2>&1
来源：http://vi.wgjwhj.cn

[R40] 追加写日志
来源：http://lc.panjiajie.cn

echo "log" >> out.log
来源：http://hr.9csxet.cn

[R41] 丢弃输出
来源：http://hu.nszjky.cn

cmd >/dev/null 2>&1
来源：http://kv.bjjhwx.cn

[R42] 输入重定向
来源：http://ac.521024.cn

wc -l < a.txt
来源：http://qi.shtwfgs.cn

[R43] 按名字查找文件
来源：http://ka.colortex.cn

find . -name "*.log" -type f
来源：http://sf.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://ak.huanxung.cn

find . -mtime -7 -type f
来源：http://lc.shtwfgs.cn

[R45] 批量删除
来源：http://bo.huanxung.cn

find . -name "*.tmp" -delete
来源：http://iz.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://dy.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://og.asd995.cn

[R47] sed 单行替换
来源：http://bv.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gv.nicolike.cn

[R48] awk 取指定列
来源：http://ra.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://rt.hahajie.cn

[R49] awk 带条件
来源：http://ug.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sr.9csxet.cn

[R50] awk 求和
来源：http://wd.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vc.jctech888.com.cn

[R51] 排序去重取前几
来源：http://xa.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xy.yuntaijiaju.cn

[R52] 统计行数
来源：http://yc.jctech888.com.cn

wc -l a.txt
来源：http://kz.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://vd.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wz.huixiangedu.cn

[R54] 比较两个文件
来源：http://uz.chemitech.net.cn

diff a.txt b.txt
来源：http://jl.lnxyls.cn

[R55] 压缩与解压
来源：http://cq.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gt.chemitech.net.cn

[R56] 远程拷贝
来源：http://gn.hahajie.cn

scp file user@host:/path/
来源：http://wz.wgjwhj.cn

[R57] 远程执行命令
来源：http://ju.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://jo.chemitech.net.cn

[R58] 下载文件
来源：http://bl.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ge.chemitech.net.cn

[R59] 发 POST JSON
来源：http://tf.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fh.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://az.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rd.521024.cn

[R61] 磁盘占用
来源：http://ya.bookmarksfly.cn

df -h;  du -sh *
来源：http://po.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://qj.521024.cn

du -ah . | sort -rh | head -10
来源：http://wt.bookmarksfly.cn

[R63] 内存与进程
来源：http://wk.colortex.cn

free -h;  ps aux | grep nginx
来源：http://sj.szxytkj.cn

[R64] 结束进程
来源：http://el.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://dc.521024.cn

[R65] 查看端口占用
来源：http://xu.szxytkj.cn


<!-- 参考信息 -->