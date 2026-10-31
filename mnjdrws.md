代发 wailian999

SELECT * FROM users;
来源：http://gn.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://ku.9csxet.cn

SELECT id, name FROM users;
来源：http://ic.huanxung.cn

[Q17] 条件查询
来源：http://sf.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lb.shtwfgs.cn

[Q18] 模糊匹配
来源：http://tt.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ls.bjjhwx.cn

[Q19] 范围查询
来源：http://vo.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ud.hahajie.cn

[Q20] IN 列表
来源：http://xs.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gb.huixinmuqiang.cn

[Q21] 空值判断
来源：http://bp.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hv.jianghongdianzi.cn

[Q22] 排序
来源：http://at.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lb.bjjhwx.cn

[Q23] 分页
来源：http://ya.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tv.asd995.cn

[Q24] 去重
来源：http://zl.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://jp.lnxyls.cn

[Q25] 只取前 N 条
来源：http://qb.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ys.yuexingan06.cn

[Q26] 计数
来源：http://yi.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://wh.haigaiapp.cn

[Q27] 条件计数
来源：http://ce.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yi.panjiajie.cn

[Q28] 求和与平均
来源：http://uu.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://px.huanxung.cn

[Q29] 最大最小值
来源：http://nr.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kn.hahajie.cn

[Q30] 分组统计
来源：http://kh.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rn.yuexingan06.cn

[Q31] 分组后过滤
来源：http://jp.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://al.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://nw.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qy.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qx.nszjky.cn

[Q33] 多列分组
来源：http://vl.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fb.shxzskj.cn

[Q34] 每组取第一条
来源：http://an.asd995.cn

SELECT * FROM (
来源：http://ns.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gi.hnjuh.cn

) t WHERE rn = 1;
来源：http://dl.muxihuayi.cn

[Q35] 内连接
来源：http://dp.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xz.huixinmuqiang.cn

[Q36] 左连接
来源：http://ax.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hd.asd995.cn

[Q37] 右连接
来源：http://cc.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qm.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ff.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oj.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://jd.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qu.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bd.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oy.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://py.shtwfgs.cn

[Q41] 多表连接
来源：http://gp.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bn.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://ox.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://cm.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://pk.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://mj.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zw.nszjky.cn

[Q43] 标量子查询
来源：http://vg.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ld.szxytkj.cn

[Q44] IN 子查询
来源：http://qi.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fv.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://xt.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ki.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cs.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dn.nicolike.cn

[Q47] 与平均值比较
来源：http://dm.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jy.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://uy.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dw.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://bv.521024.cn

[Q49] 更新单行
来源：http://kd.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lb.nszjky.cn

[Q50] 批量更新
来源：http://hu.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aj.bjjhwx.cn

[Q51] 用子查询更新
来源：http://wu.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cq.haigaiapp.cn

[Q52] 删除指定行
来源：http://ps.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://ac.szxytkj.cn

[Q53] 按条件删除
来源：http://yr.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hr.jianghongdianzi.cn

[Q54] 清空表
来源：http://yd.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://yi.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://hc.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pc.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://ea.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oo.yuexingan06.cn

[Q57] 行号
来源：http://nc.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ad.szxytkj.cn

[Q58] 累计求和
来源：http://qm.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pd.gzmigu.cn

[Q59] 分组内累计
来源：http://cz.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mr.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://el.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://od.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jo.shtwfgs.cn

[Q61] 移动平均
来源：http://xe.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oc.jianghongdianzi.cn

[Q62] 分组占比
来源：http://sf.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rp.hahajie.cn

[Q63] 开启事务
来源：http://yz.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uj.521024.cn

[Q64] 提交事务
来源：http://us.panjiajie.cn

COMMIT;
来源：http://to.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://gl.panjiajie.cn

ROLLBACK;
来源：http://tu.panjiajie.cn

[Q66] 行锁查询
来源：http://rw.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ez.hahajie.cn

[Q67] 设置隔离级别
来源：http://lj.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chemitech.net.cn

[Q68] 保存点
来源：http://kt.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://bv.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://nj.newstarts.cn

[Q69] 查看执行计划
来源：http://su.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xe.panjiajie.cn

[Q70] 更新统计信息
来源：http://pj.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://qk.chemitech.net.cn

[Q71] 查看建表语句
来源：http://db.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vj.shxzskj.cn

[Q72] 查看索引
来源：http://li.szsharing.cn

SHOW INDEX FROM users;
来源：http://ye.521024.cn

[Q73] 查看表状态
来源：http://bt.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ow.jctech888.com.cn

[Q74] 强制使用索引
来源：http://om.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vx.szsharing.cn

[Q75] 日期格式化
来源：http://gf.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ut.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://th.chemitech.net.cn

[Q76] 按天统计
来源：http://cw.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gv.panjiajie.cn

[Q77] 时间加减
来源：http://fd.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eo.huixinmuqiang.cn

[Q78] 当前时间
来源：http://cn.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ae.shtwfgs.cn

[Q79] 字符串拼接
来源：http://vr.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fs.521024.cn

[Q80] 字符串截取
来源：http://mm.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hk.bjjhwx.cn

[Q81] 字符串替换
来源：http://kv.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ef.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://wo.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uj.hnjuh.cn

[Q83] 大小写转换
来源：http://gp.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vc.panjiajie.cn

[Q84] 去除首尾空格
来源：http://ex.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://xw.hnjuh.cn

[Q85] 数值取整
来源：http://av.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://su.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://pk.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ed.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://kc.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ng.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://zz.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nj.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xs.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://ls.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rr.wgjwhj.cn

[Q90] 生成序号列
来源：http://jl.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sl.szsharing.cn

================================================================================
来源：http://th.lnxyls.cn

R. Bash 专题
来源：http://cc.shtwfgs.cn

================================================================================
来源：http://xv.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://hz.szsharing.cn

#!/usr/bin/env bash
来源：http://vd.newstarts.cn

set -euo pipefail
来源：http://my.lnxyls.cn

[R02] 变量赋值与使用
来源：http://gr.hahajie.cn

name="Tom"; echo "$name"
来源：http://mj.hahajie.cn

[R03] 只读变量
来源：http://vz.huixinmuqiang.cn

readonly PI=3.14
来源：http://fk.muxihuayi.cn

[R04] 位置参数
来源：http://wy.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hp.bookmarksfly.cn

[R05] 参数默认值
来源：http://ma.chemitech.net.cn

name="${1:-default}"
来源：http://jk.hahajie.cn

[R06] 判断命令是否存在
来源：http://my.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hq.huanxung.cn

[R07] if 判断文件
来源：http://ym.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lu.newstarts.cn

[R08] 数值比较
来源：http://zi.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ba.gzmigu.cn

[R09] 字符串比较
来源：http://va.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://og.chemitech.net.cn

[R10] 正则匹配
来源：http://ru.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ta.jctech888.com.cn

[R11] case 多分支
来源：http://lp.colortex.cn

case "$1" in
来源：http://zc.wgjwhj.cn

start) echo "启动" ;;
来源：http://sg.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://kc.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://qt.yuntaijiaju.cn

esac
来源：http://zv.nszjky.cn

[R12] for 遍历文件
来源：http://ph.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://hs.bookmarksfly.cn

[R13] for 计数循环
来源：http://so.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://wp.hahajie.cn

[R14] C 风格 for
来源：http://ah.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dt.szsharing.cn

[R15] while 逐行读文件
来源：http://sx.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gd.szsharing.cn

[R16] until 等待条件
来源：http://ps.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pp.colortex.cn

[R17] 数组定义与取值
来源：http://wk.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xz.hahajie.cn

[R18] 遍历数组
来源：http://gv.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qh.gzmigu.cn

[R19] 数组长度
来源：http://hi.chemitech.net.cn

echo "${#arr[@]}"
来源：http://zr.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://tb.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ei.521024.cn

[R21] 字符串长度
来源：http://zr.newstarts.cn

echo "${#s}"
来源：http://of.huixinmuqiang.cn

[R22] 截取子串
来源：http://gu.gzmigu.cn

echo "${s:0:5}"
来源：http://xr.bookmarksfly.cn

[R23] 字符串替换
来源：http://oc.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ml.huixiangedu.cn

[R24] 大小写转换
来源：http://ak.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wd.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://mx.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qv.hahajie.cn

[R26] 命令替换
来源：http://ux.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://qc.szxytkj.cn

[R27] 算术展开
来源：http://ef.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://du.panjiajie.cn

[R28] 浮点运算
来源：http://jt.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://to.bjjhwx.cn

[R29] 定义函数
来源：http://rg.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://th.bjjhwx.cn

[R30] 函数返回状态码
来源：http://su.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://zs.colortex.cn

[R31] 局部变量
来源：http://xh.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://fc.shxzskj.cn

[R32] 参数个数校验
来源：http://dk.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dm.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://et.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ue.521024.cn

[R34] 退出时清理
来源：http://wl.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jw.newstarts.cn

[R35] 后台执行并等待
来源：http://vm.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uu.panjiajie.cn

[R36] 并发执行多个任务
来源：http://gu.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yj.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://rb.nicolike.cn

files=$(ls -1)
来源：http://kt.shxzukj.cn

[R38] 管道串联
来源：http://sr.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://vv.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://qc.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://hf.szsharing.cn

[R40] 追加写日志
来源：http://jl.asd995.cn

echo "log" >> out.log
来源：http://dj.shxzskj.cn

[R41] 丢弃输出
来源：http://me.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://mx.lnxyls.cn

[R42] 输入重定向
来源：http://ed.shtwfgs.cn

wc -l < a.txt
来源：http://sq.newstarts.cn

[R43] 按名字查找文件
来源：http://qw.nszjky.cn

find . -name "*.log" -type f
来源：http://hb.panjiajie.cn

[R44] 按修改时间查找
来源：http://yu.szsharing.cn

find . -mtime -7 -type f
来源：http://hh.jianghongdianzi.cn

[R45] 批量删除
来源：http://tp.szsharing.cn

find . -name "*.tmp" -delete
来源：http://hs.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://zq.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ex.szxytkj.cn

[R47] sed 单行替换
来源：http://ji.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lf.szxytkj.cn

[R48] awk 取指定列
来源：http://in.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://xj.colortex.cn

[R49] awk 带条件
来源：http://jb.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.szsharing.cn

[R50] awk 求和
来源：http://hb.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dh.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://ep.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zn.nicolike.cn

[R52] 统计行数
来源：http://pi.bjjhwx.cn

wc -l a.txt
来源：http://sf.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://gp.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qh.newstarts.cn

[R54] 比较两个文件
来源：http://gw.bjjhwx.cn

diff a.txt b.txt
来源：http://zd.haigaiapp.cn

[R55] 压缩与解压
来源：http://xa.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bt.colortex.cn

[R56] 远程拷贝
来源：http://vi.jctech888.com.cn

scp file user@host:/path/
来源：http://gd.gzmigu.cn

[R57] 远程执行命令
来源：http://eu.asd995.cn

ssh user@host 'uptime'
来源：http://qp.bookmarksfly.cn

[R58] 下载文件
来源：http://tr.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gc.wgjwhj.cn

[R59] 发 POST JSON
来源：http://jz.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://my.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://gf.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qs.panjiajie.cn

[R61] 磁盘占用
来源：http://ka.lnxyls.cn

df -h;  du -sh *
来源：http://qj.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://vn.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://ni.panjiajie.cn

[R63] 内存与进程
来源：http://te.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://rs.9csxet.cn

[R64] 结束进程
来源：http://tp.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://gz.9csxet.cn

[R65] 查看端口占用
来源：http://xn.nszjky.cn


<!-- 参考信息 -->