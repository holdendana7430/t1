代发 wailian999

SELECT * FROM users;
来源：http://mq.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://qh.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://ni.szsharing.cn

[Q17] 条件查询
来源：http://nf.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dy.newstarts.cn

[Q18] 模糊匹配
来源：http://cg.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bu.nicolike.cn

[Q19] 范围查询
来源：http://ml.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wk.jctech888.com.cn

[Q20] IN 列表
来源：http://gc.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wa.huanxung.cn

[Q21] 空值判断
来源：http://ok.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fh.muxihuayi.cn

[Q22] 排序
来源：http://ic.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ka.huanxung.cn

[Q23] 分页
来源：http://yq.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rp.asd995.cn

[Q24] 去重
来源：http://tn.521024.cn

SELECT DISTINCT city FROM users;
来源：http://wz.shxzskj.cn

[Q25] 只取前 N 条
来源：http://ug.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vb.jianghongdianzi.cn

[Q26] 计数
来源：http://nj.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://vp.huanxung.cn

[Q27] 条件计数
来源：http://xt.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zg.huixiangedu.cn

[Q28] 求和与平均
来源：http://or.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eb.hahajie.cn

[Q29] 最大最小值
来源：http://lp.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xr.muxihuayi.cn

[Q30] 分组统计
来源：http://vw.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qd.huanxung.cn

[Q31] 分组后过滤
来源：http://hv.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sc.521024.cn

[Q32] 分组拼接字符串
来源：http://aj.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qe.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dm.jianghongdianzi.cn

[Q33] 多列分组
来源：http://dw.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hf.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://qn.lnxyls.cn

SELECT * FROM (
来源：http://mw.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qj.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://rp.huanxung.cn

[Q35] 内连接
来源：http://mz.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fi.huanxung.cn

[Q36] 左连接
来源：http://xm.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gj.huanxung.cn

[Q37] 右连接
来源：http://pb.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wk.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qp.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ua.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://su.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hf.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sa.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fw.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wz.huanxung.cn

[Q41] 多表连接
来源：http://zm.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://aa.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://bs.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://an.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://rr.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://kk.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iw.wgjwhj.cn

[Q43] 标量子查询
来源：http://vj.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yr.newstarts.cn

[Q44] IN 子查询
来源：http://sf.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tz.asd995.cn

[Q45] EXISTS 判断存在
来源：http://yt.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jt.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bw.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mf.chemitech.net.cn

[Q47] 与平均值比较
来源：http://ej.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dg.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://ab.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://um.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://kn.bookmarksfly.cn

[Q49] 更新单行
来源：http://yu.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://au.9csxet.cn

[Q50] 批量更新
来源：http://ul.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vw.521024.cn

[Q51] 用子查询更新
来源：http://hr.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nb.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://os.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://kd.colortex.cn

[Q53] 按条件删除
来源：http://kr.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ga.yuntaijiaju.cn

[Q54] 清空表
来源：http://pm.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://vj.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://jp.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://en.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://bb.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fo.huixinmuqiang.cn

[Q57] 行号
来源：http://ki.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cw.shtwfgs.cn

[Q58] 累计求和
来源：http://sy.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ow.szxytkj.cn

[Q59] 分组内累计
来源：http://nc.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://um.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://iu.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ec.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ei.gzmigu.cn

[Q61] 移动平均
来源：http://lw.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ko.huixinmuqiang.cn

[Q62] 分组占比
来源：http://zl.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://um.yuntaijiaju.cn

[Q63] 开启事务
来源：http://jf.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oz.shtwfgs.cn

[Q64] 提交事务
来源：http://ht.hahajie.cn

COMMIT;
来源：http://rt.gzmigu.cn

[Q65] 回滚事务
来源：http://zj.hahajie.cn

ROLLBACK;
来源：http://qz.huixiangedu.cn

[Q66] 行锁查询
来源：http://gr.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ky.newstarts.cn

[Q67] 设置隔离级别
来源：http://ce.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hm.huixiangedu.cn

[Q68] 保存点
来源：http://hd.hahajie.cn

SAVEPOINT sp1;
来源：http://hr.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://hn.newstarts.cn

[Q69] 查看执行计划
来源：http://rz.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ns.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://cq.wgjwhj.cn

ANALYZE TABLE users;
来源：http://wu.huanxung.cn

[Q71] 查看建表语句
来源：http://rr.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hq.gzmigu.cn

[Q72] 查看索引
来源：http://lu.shxzukj.cn

SHOW INDEX FROM users;
来源：http://js.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://sw.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://df.haigaiapp.cn

[Q74] 强制使用索引
来源：http://bx.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ew.asd995.cn

[Q75] 日期格式化
来源：http://kr.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lx.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fd.colortex.cn

[Q76] 按天统计
来源：http://dh.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dj.szsharing.cn

[Q77] 时间加减
来源：http://rg.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qc.chemitech.net.cn

[Q78] 当前时间
来源：http://mm.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://az.nicolike.cn

[Q79] 字符串拼接
来源：http://cd.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://np.szsharing.cn

[Q80] 字符串截取
来源：http://id.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hb.panjiajie.cn

[Q81] 字符串替换
来源：http://cx.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rv.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://tv.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ub.asd995.cn

[Q83] 大小写转换
来源：http://co.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://my.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://qd.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://si.yuexingan06.cn

[Q85] 数值取整
来源：http://zu.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lx.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://hk.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lq.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://sp.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ov.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://vq.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ly.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lc.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://cl.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qh.szxytkj.cn

[Q90] 生成序号列
来源：http://tm.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mj.huixiangedu.cn

================================================================================
来源：http://em.9csxet.cn

R. Bash 专题
来源：http://vj.haigaiapp.cn

================================================================================
来源：http://qh.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://uv.asd995.cn

#!/usr/bin/env bash
来源：http://sw.9csxet.cn

set -euo pipefail
来源：http://rb.szxytkj.cn

[R02] 变量赋值与使用
来源：http://sg.asd995.cn

name="Tom"; echo "$name"
来源：http://ct.bjjhwx.cn

[R03] 只读变量
来源：http://it.panjiajie.cn

readonly PI=3.14
来源：http://qz.yuexingan06.cn

[R04] 位置参数
来源：http://xs.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bz.szxytkj.cn

[R05] 参数默认值
来源：http://ac.huixinmuqiang.cn

name="${1:-default}"
来源：http://dw.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://yq.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qq.shxzukj.cn

[R07] if 判断文件
来源：http://fy.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hs.huanxung.cn

[R08] 数值比较
来源：http://oe.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ld.bjjhwx.cn

[R09] 字符串比较
来源：http://uq.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rk.huixiangedu.cn

[R10] 正则匹配
来源：http://ho.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pv.asd995.cn

[R11] case 多分支
来源：http://br.panjiajie.cn

case "$1" in
来源：http://dg.wgjwhj.cn

start) echo "启动" ;;
来源：http://kd.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://af.9csxet.cn

*)     echo "未知命令" ;;
来源：http://st.bookmarksfly.cn

esac
来源：http://ew.chemitech.net.cn

[R12] for 遍历文件
来源：http://nc.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://cq.hahajie.cn

[R13] for 计数循环
来源：http://jg.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://lz.szxytkj.cn

[R14] C 风格 for
来源：http://sx.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ya.panjiajie.cn

[R15] while 逐行读文件
来源：http://la.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ip.9csxet.cn

[R16] until 等待条件
来源：http://dq.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ve.lnxyls.cn

[R17] 数组定义与取值
来源：http://vs.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qs.nicolike.cn

[R18] 遍历数组
来源：http://pi.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://go.shtwfgs.cn

[R19] 数组长度
来源：http://yk.wgjwhj.cn

echo "${#arr[@]}"
来源：http://ga.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://ed.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kn.521024.cn

[R21] 字符串长度
来源：http://vd.jctech888.com.cn

echo "${#s}"
来源：http://vg.bjjhwx.cn

[R22] 截取子串
来源：http://tf.hnjuh.cn

echo "${s:0:5}"
来源：http://ob.hnjuh.cn

[R23] 字符串替换
来源：http://bh.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kf.huixinmuqiang.cn

[R24] 大小写转换
来源：http://zt.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jn.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://ij.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ci.jctech888.com.cn

[R26] 命令替换
来源：http://zn.colortex.cn

now=$(date +%F); echo "$now"
来源：http://vk.haigaiapp.cn

[R27] 算术展开
来源：http://au.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://rd.newstarts.cn

[R28] 浮点运算
来源：http://jb.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://rw.huixiangedu.cn

[R29] 定义函数
来源：http://ds.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://de.shxzukj.cn

[R30] 函数返回状态码
来源：http://td.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://ec.bjjhwx.cn

[R31] 局部变量
来源：http://ap.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://su.colortex.cn

[R32] 参数个数校验
来源：http://re.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oe.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://ve.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dz.lnxyls.cn

[R34] 退出时清理
来源：http://jo.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://do.huanxung.cn

[R35] 后台执行并等待
来源：http://rw.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ke.hahajie.cn

[R36] 并发执行多个任务
来源：http://rs.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nv.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://lq.huanxung.cn

files=$(ls -1)
来源：http://os.chemitech.net.cn

[R38] 管道串联
来源：http://fd.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://pi.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://pe.nszjky.cn

cmd > out.log 2>&1
来源：http://ia.yuexingan06.cn

[R40] 追加写日志
来源：http://fm.lnxyls.cn

echo "log" >> out.log
来源：http://hu.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://vz.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://et.9csxet.cn

[R42] 输入重定向
来源：http://ht.newstarts.cn

wc -l < a.txt
来源：http://sj.lnxyls.cn

[R43] 按名字查找文件
来源：http://hi.muxihuayi.cn

find . -name "*.log" -type f
来源：http://od.gzmigu.cn

[R44] 按修改时间查找
来源：http://ji.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://lw.newstarts.cn

[R45] 批量删除
来源：http://vz.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://bp.521024.cn

[R46] 递归替换文件内容
来源：http://xl.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zu.asd995.cn

[R47] sed 单行替换
来源：http://jp.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cq.shxzskj.cn

[R48] awk 取指定列
来源：http://wf.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://nu.9csxet.cn

[R49] awk 带条件
来源：http://rk.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aw.yuntaijiaju.cn

[R50] awk 求和
来源：http://cs.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hi.gzmigu.cn

[R51] 排序去重取前几
来源：http://mj.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oi.yuexingan06.cn

[R52] 统计行数
来源：http://el.hnjuh.cn

wc -l a.txt
来源：http://xn.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://kk.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zg.lnxyls.cn

[R54] 比较两个文件
来源：http://uy.asd995.cn

diff a.txt b.txt
来源：http://li.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://kd.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nk.gzmigu.cn

[R56] 远程拷贝
来源：http://qi.shxzskj.cn

scp file user@host:/path/
来源：http://kp.521024.cn

[R57] 远程执行命令
来源：http://ip.chemitech.net.cn

ssh user@host 'uptime'
来源：http://xk.huanxung.cn

[R58] 下载文件
来源：http://cq.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sb.huanxung.cn

[R59] 发 POST JSON
来源：http://yw.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://md.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://la.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fn.colortex.cn

[R61] 磁盘占用
来源：http://ca.haigaiapp.cn

df -h;  du -sh *
来源：http://xh.nszjky.cn

[R62] 找最占空间的文件
来源：http://fz.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://pa.chemitech.net.cn

[R63] 内存与进程
来源：http://yp.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://xi.szsharing.cn

[R64] 结束进程
来源：http://sm.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://bz.hahajie.cn

[R65] 查看端口占用
来源：http://us.bookmarksfly.cn


<!-- 参考信息 -->