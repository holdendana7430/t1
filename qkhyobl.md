代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wh.chemitech.net.cn

[Q20] IN 列表
来源：http://dx.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://le.szxytkj.cn

[Q21] 空值判断
来源：http://dn.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qa.nicolike.cn

[Q22] 排序
来源：http://xy.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bl.bjjhwx.cn

[Q23] 分页
来源：http://bz.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://me.nszjky.cn

[Q24] 去重
来源：http://un.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://vl.nszjky.cn

[Q25] 只取前 N 条
来源：http://we.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://up.huanxung.cn

[Q26] 计数
来源：http://zt.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://qp.yuexingan06.cn

[Q27] 条件计数
来源：http://ij.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ny.hahajie.cn

[Q28] 求和与平均
来源：http://ag.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pp.bjjhwx.cn

[Q29] 最大最小值
来源：http://pl.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mc.haigaiapp.cn

[Q30] 分组统计
来源：http://kv.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ts.shtwfgs.cn

[Q31] 分组后过滤
来源：http://wn.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lh.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://im.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ip.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vh.nicolike.cn

[Q33] 多列分组
来源：http://kj.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ly.newstarts.cn

[Q34] 每组取第一条
来源：http://ab.yuntaijiaju.cn

SELECT * FROM (
来源：http://id.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vv.muxihuayi.cn

) t WHERE rn = 1;
来源：http://xi.huixiangedu.cn

[Q35] 内连接
来源：http://vd.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ec.muxihuayi.cn

[Q36] 左连接
来源：http://nq.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bt.bjjhwx.cn

[Q37] 右连接
来源：http://gi.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qk.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wv.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hq.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://st.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://th.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yp.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kk.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kt.shxzskj.cn

[Q41] 多表连接
来源：http://uj.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pf.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://pn.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://fm.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://zn.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://xy.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hu.gzmigu.cn

[Q43] 标量子查询
来源：http://zd.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://da.muxihuayi.cn

[Q44] IN 子查询
来源：http://bh.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wg.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://or.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lq.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mt.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qy.jctech888.com.cn

[Q47] 与平均值比较
来源：http://pm.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pt.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://so.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://af.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://op.lnxyls.cn

[Q49] 更新单行
来源：http://fz.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://el.asd995.cn

[Q50] 批量更新
来源：http://ff.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cw.panjiajie.cn

[Q51] 用子查询更新
来源：http://ug.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yk.jctech888.com.cn

[Q52] 删除指定行
来源：http://nb.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://fv.9csxet.cn

[Q53] 按条件删除
来源：http://wl.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lz.yuntaijiaju.cn

[Q54] 清空表
来源：http://id.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://su.szsharing.cn

[Q55] 排名（并列占位）
来源：http://rh.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lu.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://go.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vj.huixinmuqiang.cn

[Q57] 行号
来源：http://eg.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wz.hahajie.cn

[Q58] 累计求和
来源：http://gc.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kd.nszjky.cn

[Q59] 分组内累计
来源：http://za.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xm.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://iu.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yk.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ox.9csxet.cn

[Q61] 移动平均
来源：http://zu.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zu.jctech888.com.cn

[Q62] 分组占比
来源：http://de.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zi.shxzskj.cn

[Q63] 开启事务
来源：http://yr.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mk.haigaiapp.cn

[Q64] 提交事务
来源：http://aj.hahajie.cn

COMMIT;
来源：http://gd.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://sb.wgjwhj.cn

ROLLBACK;
来源：http://tx.shtwfgs.cn

[Q66] 行锁查询
来源：http://gq.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://em.colortex.cn

[Q67] 设置隔离级别
来源：http://gh.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zo.9csxet.cn

[Q68] 保存点
来源：http://za.huixiangedu.cn

SAVEPOINT sp1;
来源：http://kv.gzmigu.cn

ROLLBACK TO sp1;
来源：http://eg.panjiajie.cn

[Q69] 查看执行计划
来源：http://hk.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ph.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://qy.colortex.cn

ANALYZE TABLE users;
来源：http://wd.shxzskj.cn

[Q71] 查看建表语句
来源：http://xu.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gp.newstarts.cn

[Q72] 查看索引
来源：http://sr.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://fi.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://rx.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pg.521024.cn

[Q74] 强制使用索引
来源：http://qm.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oe.asd995.cn

[Q75] 日期格式化
来源：http://bw.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dq.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nb.newstarts.cn

[Q76] 按天统计
来源：http://uo.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vm.yuntaijiaju.cn

[Q77] 时间加减
来源：http://sr.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cs.asd995.cn

[Q78] 当前时间
来源：http://rl.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kg.lnxyls.cn

[Q79] 字符串拼接
来源：http://cd.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tk.gzmigu.cn

[Q80] 字符串截取
来源：http://pq.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dr.yuexingan06.cn

[Q81] 字符串替换
来源：http://cl.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nv.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://xm.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bt.gzmigu.cn

[Q83] 大小写转换
来源：http://vo.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hy.colortex.cn

[Q84] 去除首尾空格
来源：http://bd.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://pv.panjiajie.cn

[Q85] 数值取整
来源：http://zj.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pd.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://pk.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://el.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://jc.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lz.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://cv.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bh.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://os.shxzskj.cn

[Q89] 判断表是否存在
来源：http://bj.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zv.haigaiapp.cn

[Q90] 生成序号列
来源：http://ak.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cw.hnjuh.cn

================================================================================
来源：http://zg.yuntaijiaju.cn

R. Bash 专题
来源：http://mc.shtwfgs.cn

================================================================================
来源：http://yx.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://sz.shtwfgs.cn

#!/usr/bin/env bash
来源：http://yl.shtwfgs.cn

set -euo pipefail
来源：http://hu.nszjky.cn

[R02] 变量赋值与使用
来源：http://jf.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://ko.nicolike.cn

[R03] 只读变量
来源：http://ba.yuntaijiaju.cn

readonly PI=3.14
来源：http://yr.jctech888.com.cn

[R04] 位置参数
来源：http://ig.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zk.haigaiapp.cn

[R05] 参数默认值
来源：http://lt.huanxung.cn

name="${1:-default}"
来源：http://oo.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://sg.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zb.bjjhwx.cn

[R07] if 判断文件
来源：http://se.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fv.nicolike.cn

[R08] 数值比较
来源：http://yc.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ya.bjjhwx.cn

[R09] 字符串比较
来源：http://ck.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://at.jctech888.com.cn

[R10] 正则匹配
来源：http://sg.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xm.bjjhwx.cn

[R11] case 多分支
来源：http://dj.bjjhwx.cn

case "$1" in
来源：http://jb.gzmigu.cn

start) echo "启动" ;;
来源：http://wv.hnjuh.cn

stop)  echo "停止" ;;
来源：http://zg.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://bk.hahajie.cn

esac
来源：http://xn.asd995.cn

[R12] for 遍历文件
来源：http://qf.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://sz.hahajie.cn

[R13] for 计数循环
来源：http://tl.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://yr.yuexingan06.cn

[R14] C 风格 for
来源：http://bk.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ul.szxytkj.cn

[R15] while 逐行读文件
来源：http://fx.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fz.huixiangedu.cn

[R16] until 等待条件
来源：http://hp.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yo.lnxyls.cn

[R17] 数组定义与取值
来源：http://ba.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://it.colortex.cn

[R18] 遍历数组
来源：http://xd.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mu.nicolike.cn

[R19] 数组长度
来源：http://jc.nszjky.cn

echo "${#arr[@]}"
来源：http://bg.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://fm.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ji.shxzskj.cn

[R21] 字符串长度
来源：http://pc.nicolike.cn

echo "${#s}"
来源：http://oe.muxihuayi.cn

[R22] 截取子串
来源：http://sy.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://tj.panjiajie.cn

[R23] 字符串替换
来源：http://yy.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fz.shtwfgs.cn

[R24] 大小写转换
来源：http://xr.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iq.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://da.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://us.huixinmuqiang.cn

[R26] 命令替换
来源：http://xu.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://cj.huixiangedu.cn

[R27] 算术展开
来源：http://nk.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://iw.jianghongdianzi.cn

[R28] 浮点运算
来源：http://ec.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://aa.huixinmuqiang.cn

[R29] 定义函数
来源：http://oq.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://or.shtwfgs.cn

[R30] 函数返回状态码
来源：http://hn.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ek.shxzskj.cn

[R31] 局部变量
来源：http://go.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://sf.jctech888.com.cn

[R32] 参数个数校验
来源：http://sl.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bc.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://sa.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sv.panjiajie.cn

[R34] 退出时清理
来源：http://rr.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hf.nicolike.cn

[R35] 后台执行并等待
来源：http://ij.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gi.hnjuh.cn

[R36] 并发执行多个任务
来源：http://oj.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wy.panjiajie.cn

[R37] 把输出赋给变量
来源：http://pk.huixinmuqiang.cn

files=$(ls -1)
来源：http://hu.lnxyls.cn

[R38] 管道串联
来源：http://th.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://cg.521024.cn

[R39] 重定向标准输出与错误
来源：http://ja.jctech888.com.cn

cmd > out.log 2>&1
来源：http://aq.shxzskj.cn

[R40] 追加写日志
来源：http://fi.huixiangedu.cn

echo "log" >> out.log
来源：http://rp.wgjwhj.cn

[R41] 丢弃输出
来源：http://zh.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://ae.asd995.cn

[R42] 输入重定向
来源：http://ed.asd995.cn

wc -l < a.txt
来源：http://ck.muxihuayi.cn

[R43] 按名字查找文件
来源：http://mx.hahajie.cn

find . -name "*.log" -type f
来源：http://cy.shtwfgs.cn

[R44] 按修改时间查找
来源：http://sv.szsharing.cn

find . -mtime -7 -type f
来源：http://qq.huanxung.cn

[R45] 批量删除
来源：http://pq.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://ba.huanxung.cn

[R46] 递归替换文件内容
来源：http://la.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tr.colortex.cn

[R47] sed 单行替换
来源：http://wq.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zi.hahajie.cn

[R48] awk 取指定列
来源：http://gh.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://it.hahajie.cn

[R49] awk 带条件
来源：http://tx.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ox.hahajie.cn

[R50] awk 求和
来源：http://nx.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://db.newstarts.cn

[R51] 排序去重取前几
来源：http://cs.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://co.hahajie.cn

[R52] 统计行数
来源：http://uv.lnxyls.cn

wc -l a.txt
来源：http://re.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://tf.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kh.nicolike.cn

[R54] 比较两个文件
来源：http://yr.lnxyls.cn

diff a.txt b.txt
来源：http://cc.9csxet.cn

[R55] 压缩与解压
来源：http://ys.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ih.muxihuayi.cn

[R56] 远程拷贝
来源：http://eg.yuntaijiaju.cn

scp file user@host:/path/
来源：http://pz.hahajie.cn

[R57] 远程执行命令
来源：http://vh.shxzskj.cn

ssh user@host 'uptime'
来源：http://jl.9csxet.cn

[R58] 下载文件
来源：http://sy.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kc.szsharing.cn

[R59] 发 POST JSON
来源：http://wr.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xq.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://ps.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lp.chemitech.net.cn

[R61] 磁盘占用
来源：http://jl.yuexingan06.cn

df -h;  du -sh *
来源：http://hg.panjiajie.cn

[R62] 找最占空间的文件
来源：http://fn.colortex.cn

du -ah . | sort -rh | head -10
来源：http://jt.huixiangedu.cn

[R63] 内存与进程
来源：http://an.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://oc.szxytkj.cn

[R64] 结束进程
来源：http://xa.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://kn.wgjwhj.cn

[R65] 查看端口占用
来源：http://ix.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://db.muxihuayi.cn

[R66] 定时任务
来源：http://pv.shxzskj.cn

crontab -e;  crontab -l
来源：http://xg.huanxung.cn

[R67] 生成随机十六进制串
来源：http://kn.chemitech.net.cn

openssl rand -hex 16
来源：http://jo.hnjuh.cn

[R68] 计算文件校验值
来源：http://rb.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vp.shxzskj.cn

[R69] 生成随机密码
来源：http://fc.shxzukj.cn


<!-- 参考信息 -->