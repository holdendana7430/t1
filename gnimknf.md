代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ot.haigaiapp.cn

[Q20] IN 列表
来源：http://ey.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sa.colortex.cn

[Q21] 空值判断
来源：http://lj.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mm.asd995.cn

[Q22] 排序
来源：http://yq.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kz.huanxung.cn

[Q23] 分页
来源：http://kt.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ug.521024.cn

[Q24] 去重
来源：http://og.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://xu.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://qt.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tn.gzmigu.cn

[Q26] 计数
来源：http://vl.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://xe.panjiajie.cn

[Q27] 条件计数
来源：http://eg.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lq.shtwfgs.cn

[Q28] 求和与平均
来源：http://lp.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gg.szxytkj.cn

[Q29] 最大最小值
来源：http://km.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ar.huixinmuqiang.cn

[Q30] 分组统计
来源：http://zd.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ya.hahajie.cn

[Q31] 分组后过滤
来源：http://tp.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bd.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://rw.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nn.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zy.muxihuayi.cn

[Q33] 多列分组
来源：http://fc.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qv.szxytkj.cn

[Q34] 每组取第一条
来源：http://pu.haigaiapp.cn

SELECT * FROM (
来源：http://kq.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hw.colortex.cn

) t WHERE rn = 1;
来源：http://ov.jctech888.com.cn

[Q35] 内连接
来源：http://pg.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mq.haigaiapp.cn

[Q36] 左连接
来源：http://er.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qy.521024.cn

[Q37] 右连接
来源：http://uv.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wo.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dw.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sx.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://on.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://du.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nm.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lv.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wx.newstarts.cn

[Q41] 多表连接
来源：http://rc.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://at.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://zb.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://jz.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://xe.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://de.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ir.shtwfgs.cn

[Q43] 标量子查询
来源：http://pk.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jh.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://ps.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sv.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://bo.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ro.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xy.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gs.asd995.cn

[Q47] 与平均值比较
来源：http://sx.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dr.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://jg.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://km.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://bl.jctech888.com.cn

[Q49] 更新单行
来源：http://wg.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fw.shtwfgs.cn

[Q50] 批量更新
来源：http://pu.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xu.haigaiapp.cn

[Q51] 用子查询更新
来源：http://lz.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mz.huanxung.cn

[Q52] 删除指定行
来源：http://tp.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://qz.panjiajie.cn

[Q53] 按条件删除
来源：http://hu.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dz.huixinmuqiang.cn

[Q54] 清空表
来源：http://pr.nszjky.cn

TRUNCATE TABLE logs;
来源：http://no.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://di.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nq.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://de.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jb.lnxyls.cn

[Q57] 行号
来源：http://lf.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ar.chemitech.net.cn

[Q58] 累计求和
来源：http://fl.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://po.shxzskj.cn

[Q59] 分组内累计
来源：http://yn.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bp.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://tb.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qe.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sd.yuexingan06.cn

[Q61] 移动平均
来源：http://lu.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xt.newstarts.cn

[Q62] 分组占比
来源：http://xg.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gj.nszjky.cn

[Q63] 开启事务
来源：http://ca.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ie.colortex.cn

[Q64] 提交事务
来源：http://ky.shxzukj.cn

COMMIT;
来源：http://ft.szxytkj.cn

[Q65] 回滚事务
来源：http://yr.hnjuh.cn

ROLLBACK;
来源：http://oc.huanxung.cn

[Q66] 行锁查询
来源：http://gn.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wi.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://sv.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fg.gzmigu.cn

[Q68] 保存点
来源：http://nd.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://xl.hahajie.cn

ROLLBACK TO sp1;
来源：http://xm.lnxyls.cn

[Q69] 查看执行计划
来源：http://yr.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qa.muxihuayi.cn

[Q70] 更新统计信息
来源：http://zg.muxihuayi.cn

ANALYZE TABLE users;
来源：http://qy.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://fd.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lo.bjjhwx.cn

[Q72] 查看索引
来源：http://xh.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://zj.gzmigu.cn

[Q73] 查看表状态
来源：http://pv.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bv.haigaiapp.cn

[Q74] 强制使用索引
来源：http://ry.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nj.nszjky.cn

[Q75] 日期格式化
来源：http://aq.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qh.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bm.colortex.cn

[Q76] 按天统计
来源：http://im.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ka.yuntaijiaju.cn

[Q77] 时间加减
来源：http://lb.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tc.gzmigu.cn

[Q78] 当前时间
来源：http://fy.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iz.huanxung.cn

[Q79] 字符串拼接
来源：http://ec.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uj.newstarts.cn

[Q80] 字符串截取
来源：http://df.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jb.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://do.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ht.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://ve.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nj.newstarts.cn

[Q83] 大小写转换
来源：http://cj.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jz.szsharing.cn

[Q84] 去除首尾空格
来源：http://fh.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://on.521024.cn

[Q85] 数值取整
来源：http://su.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ft.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://ci.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://om.szsharing.cn

[Q87] JSON 字段做条件
来源：http://tk.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lr.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://gt.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sr.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bq.shxzskj.cn

[Q89] 判断表是否存在
来源：http://ve.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ex.nszjky.cn

[Q90] 生成序号列
来源：http://sa.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dq.lnxyls.cn

================================================================================
来源：http://yk.panjiajie.cn

R. Bash 专题
来源：http://jz.jianghongdianzi.cn

================================================================================
来源：http://uq.521024.cn

[R01] shebang 与严格模式
来源：http://do.gzmigu.cn

#!/usr/bin/env bash
来源：http://gq.huixiangedu.cn

set -euo pipefail
来源：http://od.hnjuh.cn

[R02] 变量赋值与使用
来源：http://ms.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://ai.chemitech.net.cn

[R03] 只读变量
来源：http://dv.bjjhwx.cn

readonly PI=3.14
来源：http://lg.hnjuh.cn

[R04] 位置参数
来源：http://bw.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nd.yuexingan06.cn

[R05] 参数默认值
来源：http://me.asd995.cn

name="${1:-default}"
来源：http://cq.shxzukj.cn

[R06] 判断命令是否存在
来源：http://ud.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zv.9csxet.cn

[R07] if 判断文件
来源：http://ax.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fh.jctech888.com.cn

[R08] 数值比较
来源：http://hq.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hg.jianghongdianzi.cn

[R09] 字符串比较
来源：http://mv.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ue.hahajie.cn

[R10] 正则匹配
来源：http://zi.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aw.nicolike.cn

[R11] case 多分支
来源：http://ag.huanxung.cn

case "$1" in
来源：http://aq.szxytkj.cn

start) echo "启动" ;;
来源：http://mx.shxzukj.cn

stop)  echo "停止" ;;
来源：http://rh.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://na.asd995.cn

esac
来源：http://ah.nszjky.cn

[R12] for 遍历文件
来源：http://hd.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://ry.panjiajie.cn

[R13] for 计数循环
来源：http://gj.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://mb.gzmigu.cn

[R14] C 风格 for
来源：http://uu.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tw.huixiangedu.cn

[R15] while 逐行读文件
来源：http://be.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hx.shxzukj.cn

[R16] until 等待条件
来源：http://dc.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hg.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://hy.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dp.yuexingan06.cn

[R18] 遍历数组
来源：http://th.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://um.9csxet.cn

[R19] 数组长度
来源：http://of.lnxyls.cn

echo "${#arr[@]}"
来源：http://ev.hahajie.cn

[R20] 关联数组（字典）
来源：http://sa.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vm.colortex.cn

[R21] 字符串长度
来源：http://vh.hahajie.cn

echo "${#s}"
来源：http://lv.huixiangedu.cn

[R22] 截取子串
来源：http://um.newstarts.cn

echo "${s:0:5}"
来源：http://hj.huixiangedu.cn

[R23] 字符串替换
来源：http://yo.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fz.huanxung.cn

[R24] 大小写转换
来源：http://ys.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qf.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://dx.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jn.muxihuayi.cn

[R26] 命令替换
来源：http://in.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://gr.bookmarksfly.cn

[R27] 算术展开
来源：http://wf.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://jn.bjjhwx.cn

[R28] 浮点运算
来源：http://mw.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://os.521024.cn

[R29] 定义函数
来源：http://ym.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xn.521024.cn

[R30] 函数返回状态码
来源：http://kv.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://fb.huanxung.cn

[R31] 局部变量
来源：http://wv.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://ic.huanxung.cn

[R32] 参数个数校验
来源：http://ov.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nc.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://ui.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://va.szxytkj.cn

[R34] 退出时清理
来源：http://qm.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hu.hahajie.cn

[R35] 后台执行并等待
来源：http://js.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lh.newstarts.cn

[R36] 并发执行多个任务
来源：http://bc.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jy.521024.cn

[R37] 把输出赋给变量
来源：http://yu.chemitech.net.cn

files=$(ls -1)
来源：http://ha.jctech888.com.cn

[R38] 管道串联
来源：http://oa.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://vd.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://ix.colortex.cn

cmd > out.log 2>&1
来源：http://tc.521024.cn

[R40] 追加写日志
来源：http://oh.shxzukj.cn

echo "log" >> out.log
来源：http://wz.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://wf.huanxung.cn

cmd >/dev/null 2>&1
来源：http://fk.shxzukj.cn

[R42] 输入重定向
来源：http://fq.hahajie.cn

wc -l < a.txt
来源：http://hf.chemitech.net.cn

[R43] 按名字查找文件
来源：http://fl.nicolike.cn

find . -name "*.log" -type f
来源：http://gw.shxzukj.cn

[R44] 按修改时间查找
来源：http://dh.huixiangedu.cn

find . -mtime -7 -type f
来源：http://af.shxzukj.cn

[R45] 批量删除
来源：http://ip.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://tv.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://rd.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mk.bookmarksfly.cn

[R47] sed 单行替换
来源：http://qi.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vi.szsharing.cn

[R48] awk 取指定列
来源：http://xq.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://tz.colortex.cn

[R49] awk 带条件
来源：http://jk.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://we.huixinmuqiang.cn

[R50] awk 求和
来源：http://ho.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yn.shxzskj.cn

[R51] 排序去重取前几
来源：http://he.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vy.9csxet.cn

[R52] 统计行数
来源：http://gj.huixinmuqiang.cn

wc -l a.txt
来源：http://ik.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://rm.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://it.colortex.cn

[R54] 比较两个文件
来源：http://yc.shtwfgs.cn

diff a.txt b.txt
来源：http://cs.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://kd.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://an.hahajie.cn

[R56] 远程拷贝
来源：http://bw.nicolike.cn

scp file user@host:/path/
来源：http://ux.chemitech.net.cn

[R57] 远程执行命令
来源：http://ah.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://iq.chemitech.net.cn

[R58] 下载文件
来源：http://ii.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hw.hnjuh.cn

[R59] 发 POST JSON
来源：http://kd.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nc.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://if.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bg.yuexingan06.cn

[R61] 磁盘占用
来源：http://qq.haigaiapp.cn

df -h;  du -sh *
来源：http://iz.panjiajie.cn

[R62] 找最占空间的文件
来源：http://gs.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://kg.hnjuh.cn

[R63] 内存与进程
来源：http://gf.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://gb.huixiangedu.cn

[R64] 结束进程
来源：http://wk.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://lj.colortex.cn

[R65] 查看端口占用
来源：http://bl.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kh.lnxyls.cn

[R66] 定时任务
来源：http://cp.huanxung.cn

crontab -e;  crontab -l
来源：http://yb.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://el.shtwfgs.cn

openssl rand -hex 16
来源：http://cb.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://ks.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mm.bjjhwx.cn

[R69] 生成随机密码
来源：http://xa.yuntaijiaju.cn


<!-- 参考信息 -->