代发 wailian999

SELECT * FROM users;
来源：http://bk.lnxyls.cn

[Q16] 查询指定列
来源：http://kw.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://kq.bjjhwx.cn

[Q17] 条件查询
来源：http://qh.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://di.panjiajie.cn

[Q18] 模糊匹配
来源：http://oh.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hg.yuntaijiaju.cn

[Q19] 范围查询
来源：http://gr.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zd.chemitech.net.cn

[Q20] IN 列表
来源：http://vr.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://no.shxzskj.cn

[Q21] 空值判断
来源：http://aa.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vj.szxytkj.cn

[Q22] 排序
来源：http://tt.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uc.muxihuayi.cn

[Q23] 分页
来源：http://sx.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ic.szsharing.cn

[Q24] 去重
来源：http://iq.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://go.nicolike.cn

[Q25] 只取前 N 条
来源：http://td.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://li.muxihuayi.cn

[Q26] 计数
来源：http://bn.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://er.jctech888.com.cn

[Q27] 条件计数
来源：http://pu.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uh.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://gh.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wt.chemitech.net.cn

[Q29] 最大最小值
来源：http://fp.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rq.bjjhwx.cn

[Q30] 分组统计
来源：http://xz.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ku.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://cr.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ik.huanxung.cn

[Q32] 分组拼接字符串
来源：http://ep.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rg.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://md.huixinmuqiang.cn

[Q33] 多列分组
来源：http://an.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rh.haigaiapp.cn

[Q34] 每组取第一条
来源：http://de.9csxet.cn

SELECT * FROM (
来源：http://gj.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nn.haigaiapp.cn

) t WHERE rn = 1;
来源：http://zk.huixiangedu.cn

[Q35] 内连接
来源：http://zr.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gx.huanxung.cn

[Q36] 左连接
来源：http://hb.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nv.panjiajie.cn

[Q37] 右连接
来源：http://fx.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yc.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xz.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dx.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ci.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gr.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bz.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sv.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ve.hnjuh.cn

[Q41] 多表连接
来源：http://uj.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://el.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://gl.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://fe.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://ya.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://xf.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jn.nszjky.cn

[Q43] 标量子查询
来源：http://ha.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kn.panjiajie.cn

[Q44] IN 子查询
来源：http://bj.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mj.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://oo.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dw.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wo.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ez.haigaiapp.cn

[Q47] 与平均值比较
来源：http://fm.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xm.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://ju.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wl.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://qa.colortex.cn

[Q49] 更新单行
来源：http://dc.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pq.colortex.cn

[Q50] 批量更新
来源：http://kh.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zl.szsharing.cn

[Q51] 用子查询更新
来源：http://fx.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sn.yuexingan06.cn

[Q52] 删除指定行
来源：http://uc.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://qy.haigaiapp.cn

[Q53] 按条件删除
来源：http://bf.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fd.haigaiapp.cn

[Q54] 清空表
来源：http://ta.newstarts.cn

TRUNCATE TABLE logs;
来源：http://or.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://qu.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://di.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://ls.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wm.shxzskj.cn

[Q57] 行号
来源：http://tc.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://di.huanxung.cn

[Q58] 累计求和
来源：http://xh.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cr.muxihuayi.cn

[Q59] 分组内累计
来源：http://uf.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yc.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://ow.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ad.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ra.yuexingan06.cn

[Q61] 移动平均
来源：http://cd.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qs.huixiangedu.cn

[Q62] 分组占比
来源：http://fa.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ea.shxzskj.cn

[Q63] 开启事务
来源：http://cv.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mj.chemitech.net.cn

[Q64] 提交事务
来源：http://vu.yuexingan06.cn

COMMIT;
来源：http://xo.chemitech.net.cn

[Q65] 回滚事务
来源：http://rc.haigaiapp.cn

ROLLBACK;
来源：http://wf.chemitech.net.cn

[Q66] 行锁查询
来源：http://sg.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://th.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://wg.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lu.huixiangedu.cn

[Q68] 保存点
来源：http://zb.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://jw.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://tc.gzmigu.cn

[Q69] 查看执行计划
来源：http://uc.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kq.yuexingan06.cn

[Q70] 更新统计信息
来源：http://ui.bjjhwx.cn

ANALYZE TABLE users;
来源：http://li.chemitech.net.cn

[Q71] 查看建表语句
来源：http://hj.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://of.szxytkj.cn

[Q72] 查看索引
来源：http://js.huanxung.cn

SHOW INDEX FROM users;
来源：http://fl.chemitech.net.cn

[Q73] 查看表状态
来源：http://oq.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nw.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://mz.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ql.asd995.cn

[Q75] 日期格式化
来源：http://io.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ki.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bb.jctech888.com.cn

[Q76] 按天统计
来源：http://ka.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pu.haigaiapp.cn

[Q77] 时间加减
来源：http://gx.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bv.jctech888.com.cn

[Q78] 当前时间
来源：http://iw.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rb.shtwfgs.cn

[Q79] 字符串拼接
来源：http://jw.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://br.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://kc.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vb.haigaiapp.cn

[Q81] 字符串替换
来源：http://tj.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qq.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://xb.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://te.gzmigu.cn

[Q83] 大小写转换
来源：http://xl.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lk.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://zt.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://qd.haigaiapp.cn

[Q85] 数值取整
来源：http://aq.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ux.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://iq.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ds.521024.cn

[Q87] JSON 字段做条件
来源：http://zx.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ao.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://re.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eb.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tb.panjiajie.cn

[Q89] 判断表是否存在
来源：http://iq.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gx.huixiangedu.cn

[Q90] 生成序号列
来源：http://cf.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ck.nszjky.cn

================================================================================
来源：http://yb.wgjwhj.cn

R. Bash 专题
来源：http://xs.szsharing.cn

================================================================================
来源：http://wh.asd995.cn

[R01] shebang 与严格模式
来源：http://mw.muxihuayi.cn

#!/usr/bin/env bash
来源：http://oh.yuexingan06.cn

set -euo pipefail
来源：http://dg.shxzukj.cn

[R02] 变量赋值与使用
来源：http://os.gzmigu.cn

name="Tom"; echo "$name"
来源：http://so.huixiangedu.cn

[R03] 只读变量
来源：http://nr.bookmarksfly.cn

readonly PI=3.14
来源：http://bu.yuexingan06.cn

[R04] 位置参数
来源：http://tx.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://os.shxzukj.cn

[R05] 参数默认值
来源：http://wt.shxzukj.cn

name="${1:-default}"
来源：http://yt.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://hg.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ku.huixiangedu.cn

[R07] if 判断文件
来源：http://we.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ct.jianghongdianzi.cn

[R08] 数值比较
来源：http://cm.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ap.gzmigu.cn

[R09] 字符串比较
来源：http://xv.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vu.muxihuayi.cn

[R10] 正则匹配
来源：http://ve.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lu.bookmarksfly.cn

[R11] case 多分支
来源：http://hx.jctech888.com.cn

case "$1" in
来源：http://ka.haigaiapp.cn

start) echo "启动" ;;
来源：http://sx.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://jf.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://vs.nszjky.cn

esac
来源：http://mu.hahajie.cn

[R12] for 遍历文件
来源：http://cb.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://qn.yuntaijiaju.cn

[R13] for 计数循环
来源：http://ru.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://jp.szsharing.cn

[R14] C 风格 for
来源：http://rr.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rm.haigaiapp.cn

[R15] while 逐行读文件
来源：http://mw.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://na.yuntaijiaju.cn

[R16] until 等待条件
来源：http://qa.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yg.newstarts.cn

[R17] 数组定义与取值
来源：http://kh.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yg.shxzskj.cn

[R18] 遍历数组
来源：http://fw.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dn.colortex.cn

[R19] 数组长度
来源：http://jj.muxihuayi.cn

echo "${#arr[@]}"
来源：http://sf.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://fv.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gn.nicolike.cn

[R21] 字符串长度
来源：http://ux.yuntaijiaju.cn

echo "${#s}"
来源：http://rc.hnjuh.cn

[R22] 截取子串
来源：http://vf.asd995.cn

echo "${s:0:5}"
来源：http://cr.521024.cn

[R23] 字符串替换
来源：http://vy.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ik.shtwfgs.cn

[R24] 大小写转换
来源：http://tk.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://my.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://qm.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fi.shxzukj.cn

[R26] 命令替换
来源：http://wm.colortex.cn

now=$(date +%F); echo "$now"
来源：http://fe.gzmigu.cn

[R27] 算术展开
来源：http://ci.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://om.yuexingan06.cn

[R28] 浮点运算
来源：http://cr.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://hx.huixinmuqiang.cn

[R29] 定义函数
来源：http://fh.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wv.panjiajie.cn

[R30] 函数返回状态码
来源：http://oh.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://gm.haigaiapp.cn

[R31] 局部变量
来源：http://yp.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://rm.huixiangedu.cn

[R32] 参数个数校验
来源：http://po.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ew.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://dg.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://se.yuntaijiaju.cn

[R34] 退出时清理
来源：http://qc.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vk.gzmigu.cn

[R35] 后台执行并等待
来源：http://gf.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mg.shxzskj.cn

[R36] 并发执行多个任务
来源：http://ua.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://le.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://jj.bjjhwx.cn

files=$(ls -1)
来源：http://bx.haigaiapp.cn

[R38] 管道串联
来源：http://ur.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://ug.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://hv.bjjhwx.cn

cmd > out.log 2>&1
来源：http://uo.nicolike.cn

[R40] 追加写日志
来源：http://wu.shxzukj.cn

echo "log" >> out.log
来源：http://kt.nicolike.cn

[R41] 丢弃输出
来源：http://ts.nszjky.cn

cmd >/dev/null 2>&1
来源：http://up.wgjwhj.cn

[R42] 输入重定向
来源：http://mk.huixinmuqiang.cn

wc -l < a.txt
来源：http://tm.asd995.cn

[R43] 按名字查找文件
来源：http://di.shxzskj.cn

find . -name "*.log" -type f
来源：http://bd.jctech888.com.cn

[R44] 按修改时间查找
来源：http://kb.wgjwhj.cn

find . -mtime -7 -type f
来源：http://rn.szxytkj.cn

[R45] 批量删除
来源：http://vy.asd995.cn

find . -name "*.tmp" -delete
来源：http://av.hahajie.cn

[R46] 递归替换文件内容
来源：http://ke.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jm.asd995.cn

[R47] sed 单行替换
来源：http://lf.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yb.asd995.cn

[R48] awk 取指定列
来源：http://xr.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://qz.chemitech.net.cn

[R49] awk 带条件
来源：http://tx.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oj.521024.cn

[R50] awk 求和
来源：http://ni.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pu.nicolike.cn

[R51] 排序去重取前几
来源：http://ug.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jd.shxzukj.cn

[R52] 统计行数
来源：http://kv.yuexingan06.cn

wc -l a.txt
来源：http://ir.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://sz.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tn.chemitech.net.cn

[R54] 比较两个文件
来源：http://ob.yuexingan06.cn

diff a.txt b.txt
来源：http://oy.nszjky.cn

[R55] 压缩与解压
来源：http://iw.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ys.9csxet.cn

[R56] 远程拷贝
来源：http://vj.yuntaijiaju.cn

scp file user@host:/path/
来源：http://pv.hahajie.cn

[R57] 远程执行命令
来源：http://uu.shxzukj.cn

ssh user@host 'uptime'
来源：http://hz.nszjky.cn

[R58] 下载文件
来源：http://fd.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://er.bjjhwx.cn

[R59] 发 POST JSON
来源：http://vh.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://af.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://ye.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lb.szxytkj.cn

[R61] 磁盘占用
来源：http://ft.huixiangedu.cn

df -h;  du -sh *
来源：http://aa.hnjuh.cn

[R62] 找最占空间的文件
来源：http://ry.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://dz.newstarts.cn

[R63] 内存与进程
来源：http://dw.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://uy.wgjwhj.cn

[R64] 结束进程
来源：http://tg.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://bd.wgjwhj.cn

[R65] 查看端口占用
来源：http://jj.colortex.cn


<!-- 参考信息 -->