代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://ui.nicolike.cn

[Q22] 排序
来源：http://ok.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tn.newstarts.cn

[Q23] 分页
来源：http://mi.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ay.nicolike.cn

[Q24] 去重
来源：http://uj.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://hs.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://eg.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bj.huixiangedu.cn

[Q26] 计数
来源：http://va.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://lm.szsharing.cn

[Q27] 条件计数
来源：http://gr.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vu.chemitech.net.cn

[Q28] 求和与平均
来源：http://yj.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jf.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://sx.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cp.hnjuh.cn

[Q30] 分组统计
来源：http://yb.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nm.asd995.cn

[Q31] 分组后过滤
来源：http://de.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bh.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://qs.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aw.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xe.chemitech.net.cn

[Q33] 多列分组
来源：http://hu.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ta.nszjky.cn

[Q34] 每组取第一条
来源：http://bz.shtwfgs.cn

SELECT * FROM (
来源：http://to.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ol.szxytkj.cn

) t WHERE rn = 1;
来源：http://sq.asd995.cn

[Q35] 内连接
来源：http://vx.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pn.huanxung.cn

[Q36] 左连接
来源：http://tx.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bh.hahajie.cn

[Q37] 右连接
来源：http://st.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kw.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yk.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pe.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://go.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ri.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tt.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qw.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xa.shxzukj.cn

[Q41] 多表连接
来源：http://vw.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://id.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://ko.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://me.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://dj.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://jl.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gc.shtwfgs.cn

[Q43] 标量子查询
来源：http://ml.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sb.lnxyls.cn

[Q44] IN 子查询
来源：http://yy.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ee.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://ms.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hm.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tn.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fc.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://sf.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://es.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://ii.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sw.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://bn.muxihuayi.cn

[Q49] 更新单行
来源：http://qd.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ok.lnxyls.cn

[Q50] 批量更新
来源：http://fw.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ix.shxzskj.cn

[Q51] 用子查询更新
来源：http://oe.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lh.panjiajie.cn

[Q52] 删除指定行
来源：http://li.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://fu.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://bw.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fl.chemitech.net.cn

[Q54] 清空表
来源：http://ge.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://up.hahajie.cn

[Q55] 排名（并列占位）
来源：http://rb.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wl.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://sx.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vw.gzmigu.cn

[Q57] 行号
来源：http://tg.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kz.huixiangedu.cn

[Q58] 累计求和
来源：http://ph.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yy.521024.cn

[Q59] 分组内累计
来源：http://dw.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://in.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://xh.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ng.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qg.huanxung.cn

[Q61] 移动平均
来源：http://sd.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nx.wgjwhj.cn

[Q62] 分组占比
来源：http://ob.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zk.shxzukj.cn

[Q63] 开启事务
来源：http://yr.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mr.shxzukj.cn

[Q64] 提交事务
来源：http://ej.wgjwhj.cn

COMMIT;
来源：http://uw.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://zd.shxzukj.cn

ROLLBACK;
来源：http://mk.yuexingan06.cn

[Q66] 行锁查询
来源：http://pl.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yj.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://rx.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fd.shxzskj.cn

[Q68] 保存点
来源：http://ax.nicolike.cn

SAVEPOINT sp1;
来源：http://pp.szxytkj.cn

ROLLBACK TO sp1;
来源：http://rz.newstarts.cn

[Q69] 查看执行计划
来源：http://pc.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ny.hnjuh.cn

[Q70] 更新统计信息
来源：http://pt.wgjwhj.cn

ANALYZE TABLE users;
来源：http://rm.hahajie.cn

[Q71] 查看建表语句
来源：http://kl.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ph.yuexingan06.cn

[Q72] 查看索引
来源：http://ht.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://qw.chemitech.net.cn

[Q73] 查看表状态
来源：http://cx.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ob.hahajie.cn

[Q74] 强制使用索引
来源：http://xz.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xg.jctech888.com.cn

[Q75] 日期格式化
来源：http://vj.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pu.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zf.newstarts.cn

[Q76] 按天统计
来源：http://bo.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ud.9csxet.cn

[Q77] 时间加减
来源：http://fi.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qs.wgjwhj.cn

[Q78] 当前时间
来源：http://lv.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ca.wgjwhj.cn

[Q79] 字符串拼接
来源：http://en.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dq.nicolike.cn

[Q80] 字符串截取
来源：http://eg.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hu.yuexingan06.cn

[Q81] 字符串替换
来源：http://qg.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ff.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://nd.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aq.shxzukj.cn

[Q83] 大小写转换
来源：http://ch.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lv.9csxet.cn

[Q84] 去除首尾空格
来源：http://bv.521024.cn

SELECT TRIM(name) FROM users;
来源：http://fq.521024.cn

[Q85] 数值取整
来源：http://kq.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nm.colortex.cn

[Q86] 读取 JSON 字段
来源：http://ty.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://si.asd995.cn

[Q87] JSON 字段做条件
来源：http://ye.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kc.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://tz.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bb.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vo.hahajie.cn

[Q89] 判断表是否存在
来源：http://vn.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zl.wgjwhj.cn

[Q90] 生成序号列
来源：http://mr.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nb.yuntaijiaju.cn

================================================================================
来源：http://zo.hnjuh.cn

R. Bash 专题
来源：http://nj.jctech888.com.cn

================================================================================
来源：http://ie.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://vp.jctech888.com.cn

#!/usr/bin/env bash
来源：http://zh.huanxung.cn

set -euo pipefail
来源：http://hk.521024.cn

[R02] 变量赋值与使用
来源：http://ov.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://mm.lnxyls.cn

[R03] 只读变量
来源：http://gs.newstarts.cn

readonly PI=3.14
来源：http://hi.huixiangedu.cn

[R04] 位置参数
来源：http://fu.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fr.lnxyls.cn

[R05] 参数默认值
来源：http://pr.nszjky.cn

name="${1:-default}"
来源：http://ew.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://du.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nf.huixiangedu.cn

[R07] if 判断文件
来源：http://jj.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wh.shtwfgs.cn

[R08] 数值比较
来源：http://uo.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oj.szxytkj.cn

[R09] 字符串比较
来源：http://yx.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yh.nszjky.cn

[R10] 正则匹配
来源：http://ux.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ol.shxzukj.cn

[R11] case 多分支
来源：http://gb.nszjky.cn

case "$1" in
来源：http://zs.szxytkj.cn

start) echo "启动" ;;
来源：http://qj.521024.cn

stop)  echo "停止" ;;
来源：http://td.hahajie.cn

*)     echo "未知命令" ;;
来源：http://uy.yuntaijiaju.cn

esac
来源：http://ky.colortex.cn

[R12] for 遍历文件
来源：http://bm.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://nn.asd995.cn

[R13] for 计数循环
来源：http://tw.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://dj.bjjhwx.cn

[R14] C 风格 for
来源：http://vk.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dv.521024.cn

[R15] while 逐行读文件
来源：http://om.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sk.colortex.cn

[R16] until 等待条件
来源：http://je.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cu.hahajie.cn

[R17] 数组定义与取值
来源：http://yp.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uw.shxzukj.cn

[R18] 遍历数组
来源：http://lz.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://md.huanxung.cn

[R19] 数组长度
来源：http://fy.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://xo.shxzskj.cn

[R20] 关联数组（字典）
来源：http://zw.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ee.wgjwhj.cn

[R21] 字符串长度
来源：http://uk.panjiajie.cn

echo "${#s}"
来源：http://ii.jianghongdianzi.cn

[R22] 截取子串
来源：http://mm.newstarts.cn

echo "${s:0:5}"
来源：http://wi.haigaiapp.cn

[R23] 字符串替换
来源：http://st.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gw.hahajie.cn

[R24] 大小写转换
来源：http://zw.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ix.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://vd.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zo.shxzskj.cn

[R26] 命令替换
来源：http://rb.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://cs.haigaiapp.cn

[R27] 算术展开
来源：http://cy.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://cx.gzmigu.cn

[R28] 浮点运算
来源：http://ki.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://jj.gzmigu.cn

[R29] 定义函数
来源：http://si.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fb.hnjuh.cn

[R30] 函数返回状态码
来源：http://bx.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://is.panjiajie.cn

[R31] 局部变量
来源：http://ym.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://gd.nicolike.cn

[R32] 参数个数校验
来源：http://mp.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cd.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://jv.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ej.panjiajie.cn

[R34] 退出时清理
来源：http://mn.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jh.shtwfgs.cn

[R35] 后台执行并等待
来源：http://cd.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://un.shxzskj.cn

[R36] 并发执行多个任务
来源：http://sb.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ck.szxytkj.cn

[R37] 把输出赋给变量
来源：http://lt.shxzskj.cn

files=$(ls -1)
来源：http://ob.shxzskj.cn

[R38] 管道串联
来源：http://ej.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://pr.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://aj.haigaiapp.cn

cmd > out.log 2>&1
来源：http://sp.yuexingan06.cn

[R40] 追加写日志
来源：http://yc.szxytkj.cn

echo "log" >> out.log
来源：http://uj.hnjuh.cn

[R41] 丢弃输出
来源：http://ga.colortex.cn

cmd >/dev/null 2>&1
来源：http://vj.newstarts.cn

[R42] 输入重定向
来源：http://jh.nicolike.cn

wc -l < a.txt
来源：http://hd.hahajie.cn

[R43] 按名字查找文件
来源：http://sf.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://to.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://lb.colortex.cn

find . -mtime -7 -type f
来源：http://fq.muxihuayi.cn

[R45] 批量删除
来源：http://gh.asd995.cn

find . -name "*.tmp" -delete
来源：http://ci.huanxung.cn

[R46] 递归替换文件内容
来源：http://pj.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://op.haigaiapp.cn

[R47] sed 单行替换
来源：http://as.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uw.hahajie.cn

[R48] awk 取指定列
来源：http://bc.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://rp.wgjwhj.cn

[R49] awk 带条件
来源：http://hv.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hm.chemitech.net.cn

[R50] awk 求和
来源：http://uj.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qu.muxihuayi.cn

[R51] 排序去重取前几
来源：http://jl.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tx.yuexingan06.cn

[R52] 统计行数
来源：http://ho.521024.cn

wc -l a.txt
来源：http://sr.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://of.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ug.gzmigu.cn

[R54] 比较两个文件
来源：http://jw.shxzskj.cn

diff a.txt b.txt
来源：http://sd.szxytkj.cn

[R55] 压缩与解压
来源：http://dj.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cf.haigaiapp.cn

[R56] 远程拷贝
来源：http://wj.shxzskj.cn

scp file user@host:/path/
来源：http://zt.521024.cn

[R57] 远程执行命令
来源：http://bb.muxihuayi.cn

ssh user@host 'uptime'
来源：http://tu.bookmarksfly.cn

[R58] 下载文件
来源：http://bq.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cs.szsharing.cn

[R59] 发 POST JSON
来源：http://jz.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lc.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://zc.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ff.521024.cn

[R61] 磁盘占用
来源：http://yr.hahajie.cn

df -h;  du -sh *
来源：http://tn.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://ei.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://dq.yuexingan06.cn

[R63] 内存与进程
来源：http://gj.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://bk.gzmigu.cn

[R64] 结束进程
来源：http://ko.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://mh.szxytkj.cn

[R65] 查看端口占用
来源：http://ec.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qx.bookmarksfly.cn

[R66] 定时任务
来源：http://rx.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://xo.huanxung.cn

[R67] 生成随机十六进制串
来源：http://eq.panjiajie.cn

openssl rand -hex 16
来源：http://gf.yuexingan06.cn

[R68] 计算文件校验值
来源：http://vp.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dd.hahajie.cn

[R69] 生成随机密码
来源：http://dg.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://lt.shxzukj.cn

[R70] 时间戳与互转
来源：http://ox.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://wk.szxytkj.cn

[R71] 日期格式化
来源：http://xn.panjiajie.cn


<!-- 参考信息 -->