代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://pm.lnxyls.cn

[Q22] 排序
来源：http://je.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://im.hnjuh.cn

[Q23] 分页
来源：http://ph.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://id.yuexingan06.cn

[Q24] 去重
来源：http://zg.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://tj.szxytkj.cn

[Q25] 只取前 N 条
来源：http://qm.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ap.9csxet.cn

[Q26] 计数
来源：http://en.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://ph.newstarts.cn

[Q27] 条件计数
来源：http://st.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ft.bookmarksfly.cn

[Q28] 求和与平均
来源：http://do.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jj.huanxung.cn

[Q29] 最大最小值
来源：http://fj.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yb.muxihuayi.cn

[Q30] 分组统计
来源：http://mw.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lm.szxytkj.cn

[Q31] 分组后过滤
来源：http://tv.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ac.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://vr.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sr.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sa.yuexingan06.cn

[Q33] 多列分组
来源：http://fi.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xn.hahajie.cn

[Q34] 每组取第一条
来源：http://oq.shxzskj.cn

SELECT * FROM (
来源：http://sy.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xl.521024.cn

) t WHERE rn = 1;
来源：http://pv.shxzukj.cn

[Q35] 内连接
来源：http://ik.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://av.shtwfgs.cn

[Q36] 左连接
来源：http://cz.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://do.nszjky.cn

[Q37] 右连接
来源：http://rs.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rv.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://is.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kj.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://ld.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mv.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pv.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xg.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yz.yuntaijiaju.cn

[Q41] 多表连接
来源：http://es.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ce.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://rj.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://sw.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://dt.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://gh.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pd.521024.cn

[Q43] 标量子查询
来源：http://ir.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gk.521024.cn

[Q44] IN 子查询
来源：http://qb.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bv.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://jz.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rc.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ad.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wb.panjiajie.cn

[Q47] 与平均值比较
来源：http://jy.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://df.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://od.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gm.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ht.nicolike.cn

[Q49] 更新单行
来源：http://eg.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ct.muxihuayi.cn

[Q50] 批量更新
来源：http://zp.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ab.huixiangedu.cn

[Q51] 用子查询更新
来源：http://wu.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ar.chemitech.net.cn

[Q52] 删除指定行
来源：http://hg.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://um.bookmarksfly.cn

[Q53] 按条件删除
来源：http://ax.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vs.panjiajie.cn

[Q54] 清空表
来源：http://yt.521024.cn

TRUNCATE TABLE logs;
来源：http://ay.hahajie.cn

[Q55] 排名（并列占位）
来源：http://pb.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yl.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://do.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jm.9csxet.cn

[Q57] 行号
来源：http://ii.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rj.huanxung.cn

[Q58] 累计求和
来源：http://xz.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jb.jctech888.com.cn

[Q59] 分组内累计
来源：http://ty.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://op.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://ga.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ab.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qm.bjjhwx.cn

[Q61] 移动平均
来源：http://kt.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ly.bjjhwx.cn

[Q62] 分组占比
来源：http://bb.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hb.bookmarksfly.cn

[Q63] 开启事务
来源：http://vo.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nm.huanxung.cn

[Q64] 提交事务
来源：http://aw.gzmigu.cn

COMMIT;
来源：http://js.szsharing.cn

[Q65] 回滚事务
来源：http://up.szxytkj.cn

ROLLBACK;
来源：http://qk.shtwfgs.cn

[Q66] 行锁查询
来源：http://yw.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rx.szsharing.cn

[Q67] 设置隔离级别
来源：http://jv.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pv.muxihuayi.cn

[Q68] 保存点
来源：http://xa.shxzukj.cn

SAVEPOINT sp1;
来源：http://tu.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://in.hnjuh.cn

[Q69] 查看执行计划
来源：http://be.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jv.521024.cn

[Q70] 更新统计信息
来源：http://mm.521024.cn

ANALYZE TABLE users;
来源：http://pw.panjiajie.cn

[Q71] 查看建表语句
来源：http://xc.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mt.shxzskj.cn

[Q72] 查看索引
来源：http://aa.gzmigu.cn

SHOW INDEX FROM users;
来源：http://dp.huanxung.cn

[Q73] 查看表状态
来源：http://rw.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vz.huixiangedu.cn

[Q74] 强制使用索引
来源：http://em.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ay.szsharing.cn

[Q75] 日期格式化
来源：http://aq.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://md.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mw.huanxung.cn

[Q76] 按天统计
来源：http://pg.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cf.shtwfgs.cn

[Q77] 时间加减
来源：http://pb.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ie.yuntaijiaju.cn

[Q78] 当前时间
来源：http://dv.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cc.hnjuh.cn

[Q79] 字符串拼接
来源：http://wj.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yn.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://fj.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ad.521024.cn

[Q81] 字符串替换
来源：http://ii.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rz.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://bt.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xq.shtwfgs.cn

[Q83] 大小写转换
来源：http://mi.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pb.gzmigu.cn

[Q84] 去除首尾空格
来源：http://kd.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://ui.shxzukj.cn

[Q85] 数值取整
来源：http://wt.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gd.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://li.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ox.521024.cn

[Q87] JSON 字段做条件
来源：http://af.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://if.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://qj.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gd.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sy.huanxung.cn

[Q89] 判断表是否存在
来源：http://wt.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iz.chemitech.net.cn

[Q90] 生成序号列
来源：http://oq.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hx.wgjwhj.cn

================================================================================
来源：http://it.wgjwhj.cn

R. Bash 专题
来源：http://fr.lnxyls.cn

================================================================================
来源：http://ak.521024.cn

[R01] shebang 与严格模式
来源：http://kv.panjiajie.cn

#!/usr/bin/env bash
来源：http://uz.gzmigu.cn

set -euo pipefail
来源：http://lo.huanxung.cn

[R02] 变量赋值与使用
来源：http://xf.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://rl.szsharing.cn

[R03] 只读变量
来源：http://bi.muxihuayi.cn

readonly PI=3.14
来源：http://ji.colortex.cn

[R04] 位置参数
来源：http://gw.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lh.szxytkj.cn

[R05] 参数默认值
来源：http://zb.newstarts.cn

name="${1:-default}"
来源：http://dr.521024.cn

[R06] 判断命令是否存在
来源：http://hq.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hi.nszjky.cn

[R07] if 判断文件
来源：http://zo.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jh.9csxet.cn

[R08] 数值比较
来源：http://rw.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eo.shxzukj.cn

[R09] 字符串比较
来源：http://nq.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://du.wgjwhj.cn

[R10] 正则匹配
来源：http://ys.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tc.lnxyls.cn

[R11] case 多分支
来源：http://vz.jctech888.com.cn

case "$1" in
来源：http://ln.shxzukj.cn

start) echo "启动" ;;
来源：http://hy.nszjky.cn

stop)  echo "停止" ;;
来源：http://my.huanxung.cn

*)     echo "未知命令" ;;
来源：http://mn.panjiajie.cn

esac
来源：http://xg.huanxung.cn

[R12] for 遍历文件
来源：http://br.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://kv.nszjky.cn

[R13] for 计数循环
来源：http://cx.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://bv.bookmarksfly.cn

[R14] C 风格 for
来源：http://ch.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ds.shtwfgs.cn

[R15] while 逐行读文件
来源：http://pk.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sa.szsharing.cn

[R16] until 等待条件
来源：http://ph.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uo.wgjwhj.cn

[R17] 数组定义与取值
来源：http://ku.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://en.shxzukj.cn

[R18] 遍历数组
来源：http://ym.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pz.shxzskj.cn

[R19] 数组长度
来源：http://iu.huixiangedu.cn

echo "${#arr[@]}"
来源：http://yu.nicolike.cn

[R20] 关联数组（字典）
来源：http://yc.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fr.chemitech.net.cn

[R21] 字符串长度
来源：http://hs.shxzskj.cn

echo "${#s}"
来源：http://hm.asd995.cn

[R22] 截取子串
来源：http://hd.521024.cn

echo "${s:0:5}"
来源：http://fl.hnjuh.cn

[R23] 字符串替换
来源：http://lf.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ds.haigaiapp.cn

[R24] 大小写转换
来源：http://ai.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vs.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://sw.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pl.jctech888.com.cn

[R26] 命令替换
来源：http://nc.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://lz.panjiajie.cn

[R27] 算术展开
来源：http://dl.newstarts.cn

echo $((1 + 2 * 3))
来源：http://nc.haigaiapp.cn

[R28] 浮点运算
来源：http://ov.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://ee.wgjwhj.cn

[R29] 定义函数
来源：http://qc.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xv.shtwfgs.cn

[R30] 函数返回状态码
来源：http://qs.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://rr.wgjwhj.cn

[R31] 局部变量
来源：http://nh.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://fs.wgjwhj.cn

[R32] 参数个数校验
来源：http://hp.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rs.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://ut.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ck.newstarts.cn

[R34] 退出时清理
来源：http://pp.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fq.asd995.cn

[R35] 后台执行并等待
来源：http://vv.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vc.panjiajie.cn

[R36] 并发执行多个任务
来源：http://zw.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iw.asd995.cn

[R37] 把输出赋给变量
来源：http://gd.asd995.cn

files=$(ls -1)
来源：http://tr.newstarts.cn

[R38] 管道串联
来源：http://ws.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://vv.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://dk.colortex.cn

cmd > out.log 2>&1
来源：http://tr.yuexingan06.cn

[R40] 追加写日志
来源：http://ad.hahajie.cn

echo "log" >> out.log
来源：http://ya.colortex.cn

[R41] 丢弃输出
来源：http://or.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://ud.yuntaijiaju.cn

[R42] 输入重定向
来源：http://pi.panjiajie.cn

wc -l < a.txt
来源：http://xv.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://vq.haigaiapp.cn

find . -name "*.log" -type f
来源：http://mp.szxytkj.cn

[R44] 按修改时间查找
来源：http://sk.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://ci.lnxyls.cn

[R45] 批量删除
来源：http://te.hahajie.cn

find . -name "*.tmp" -delete
来源：http://vq.lnxyls.cn

[R46] 递归替换文件内容
来源：http://ai.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hn.szsharing.cn

[R47] sed 单行替换
来源：http://wo.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fa.hnjuh.cn

[R48] awk 取指定列
来源：http://do.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://rw.huixiangedu.cn

[R49] awk 带条件
来源：http://gl.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fg.lnxyls.cn

[R50] awk 求和
来源：http://in.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eu.szxytkj.cn

[R51] 排序去重取前几
来源：http://xr.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xy.nicolike.cn

[R52] 统计行数
来源：http://py.szsharing.cn

wc -l a.txt
来源：http://ax.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://yp.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ga.nicolike.cn

[R54] 比较两个文件
来源：http://tk.nszjky.cn

diff a.txt b.txt
来源：http://wr.lnxyls.cn

[R55] 压缩与解压
来源：http://ub.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mi.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://be.muxihuayi.cn

scp file user@host:/path/
来源：http://qi.asd995.cn

[R57] 远程执行命令
来源：http://tt.huixiangedu.cn

ssh user@host 'uptime'
来源：http://po.nicolike.cn

[R58] 下载文件
来源：http://bl.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hu.yuexingan06.cn

[R59] 发 POST JSON
来源：http://rd.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dx.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://is.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rv.bjjhwx.cn

[R61] 磁盘占用
来源：http://lo.nicolike.cn

df -h;  du -sh *
来源：http://ab.panjiajie.cn

[R62] 找最占空间的文件
来源：http://wt.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://gv.hahajie.cn

[R63] 内存与进程
来源：http://mr.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://hz.bjjhwx.cn

[R64] 结束进程
来源：http://gr.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://aa.521024.cn

[R65] 查看端口占用
来源：http://vl.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vx.shxzskj.cn

[R66] 定时任务
来源：http://xj.yuexingan06.cn

crontab -e;  crontab -l
来源：http://km.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://cv.nicolike.cn

openssl rand -hex 16
来源：http://tb.asd995.cn

[R68] 计算文件校验值
来源：http://qf.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wr.bookmarksfly.cn

[R69] 生成随机密码
来源：http://ne.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://pl.huanxung.cn

[R70] 时间戳与互转
来源：http://bp.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://sc.muxihuayi.cn

[R71] 日期格式化
来源：http://xp.521024.cn


<!-- 参考信息 -->