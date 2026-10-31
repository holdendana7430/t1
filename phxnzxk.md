代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://rh.hnjuh.cn

[Q22] 排序
来源：http://fn.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rg.nicolike.cn

[Q23] 分页
来源：http://ty.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rc.521024.cn

[Q24] 去重
来源：http://fm.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://bu.shxzskj.cn

[Q25] 只取前 N 条
来源：http://zh.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://en.wgjwhj.cn

[Q26] 计数
来源：http://ji.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://xk.nszjky.cn

[Q27] 条件计数
来源：http://zm.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ma.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://hs.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ai.bookmarksfly.cn

[Q29] 最大最小值
来源：http://hs.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://di.panjiajie.cn

[Q30] 分组统计
来源：http://tb.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kv.colortex.cn

[Q31] 分组后过滤
来源：http://ag.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nm.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://xp.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kj.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xk.newstarts.cn

[Q33] 多列分组
来源：http://mj.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xe.hnjuh.cn

[Q34] 每组取第一条
来源：http://dq.panjiajie.cn

SELECT * FROM (
来源：http://qv.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ra.gzmigu.cn

) t WHERE rn = 1;
来源：http://ku.wgjwhj.cn

[Q35] 内连接
来源：http://pr.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ub.nszjky.cn

[Q36] 左连接
来源：http://ba.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zn.wgjwhj.cn

[Q37] 右连接
来源：http://lf.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wx.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tl.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dk.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://kv.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wg.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jr.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tc.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ue.lnxyls.cn

[Q41] 多表连接
来源：http://jy.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xg.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://uy.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://nd.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://mz.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://zu.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qy.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://ty.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ed.haigaiapp.cn

[Q44] IN 子查询
来源：http://mx.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hs.521024.cn

[Q45] EXISTS 判断存在
来源：http://ti.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wv.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wy.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mh.yuexingan06.cn

[Q47] 与平均值比较
来源：http://fg.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xv.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://jg.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pz.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://po.yuntaijiaju.cn

[Q49] 更新单行
来源：http://rv.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qc.jctech888.com.cn

[Q50] 批量更新
来源：http://yj.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fk.haigaiapp.cn

[Q51] 用子查询更新
来源：http://cd.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sp.asd995.cn

[Q52] 删除指定行
来源：http://ex.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://un.shtwfgs.cn

[Q53] 按条件删除
来源：http://xj.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iy.hnjuh.cn

[Q54] 清空表
来源：http://gh.szsharing.cn

TRUNCATE TABLE logs;
来源：http://jx.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://ur.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nh.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://ge.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zz.gzmigu.cn

[Q57] 行号
来源：http://xk.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://id.bookmarksfly.cn

[Q58] 累计求和
来源：http://zo.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ii.huanxung.cn

[Q59] 分组内累计
来源：http://uu.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rn.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://qj.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oa.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zi.521024.cn

[Q61] 移动平均
来源：http://fu.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ea.jianghongdianzi.cn

[Q62] 分组占比
来源：http://jm.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ad.newstarts.cn

[Q63] 开启事务
来源：http://kr.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://py.huixinmuqiang.cn

[Q64] 提交事务
来源：http://zb.shxzskj.cn

COMMIT;
来源：http://qy.huixiangedu.cn

[Q65] 回滚事务
来源：http://sb.bookmarksfly.cn

ROLLBACK;
来源：http://mh.shxzskj.cn

[Q66] 行锁查询
来源：http://aj.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cd.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://at.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ip.newstarts.cn

[Q68] 保存点
来源：http://in.newstarts.cn

SAVEPOINT sp1;
来源：http://ft.hahajie.cn

ROLLBACK TO sp1;
来源：http://ik.9csxet.cn

[Q69] 查看执行计划
来源：http://je.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ej.huanxung.cn

[Q70] 更新统计信息
来源：http://nx.huanxung.cn

ANALYZE TABLE users;
来源：http://kr.bjjhwx.cn

[Q71] 查看建表语句
来源：http://zh.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jn.huanxung.cn

[Q72] 查看索引
来源：http://zu.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://kh.huixiangedu.cn

[Q73] 查看表状态
来源：http://vo.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qi.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://yt.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ae.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://tw.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qo.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xe.bjjhwx.cn

[Q76] 按天统计
来源：http://vv.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ks.huanxung.cn

[Q77] 时间加减
来源：http://pg.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cl.lnxyls.cn

[Q78] 当前时间
来源：http://xa.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pt.nszjky.cn

[Q79] 字符串拼接
来源：http://sl.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zk.nszjky.cn

[Q80] 字符串截取
来源：http://io.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sy.huanxung.cn

[Q81] 字符串替换
来源：http://dg.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://do.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://wp.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oz.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://tg.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nz.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://cg.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://zl.chemitech.net.cn

[Q85] 数值取整
来源：http://yu.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vh.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://tb.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sd.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://sn.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yn.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://sa.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lm.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://un.huanxung.cn

[Q89] 判断表是否存在
来源：http://zk.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fv.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://jp.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fw.shxzukj.cn

================================================================================
来源：http://lu.521024.cn

R. Bash 专题
来源：http://hn.wgjwhj.cn

================================================================================
来源：http://ck.huanxung.cn

[R01] shebang 与严格模式
来源：http://za.newstarts.cn

#!/usr/bin/env bash
来源：http://vs.yuexingan06.cn

set -euo pipefail
来源：http://yd.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://ur.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://mz.bjjhwx.cn

[R03] 只读变量
来源：http://fi.yuntaijiaju.cn

readonly PI=3.14
来源：http://ll.nicolike.cn

[R04] 位置参数
来源：http://aj.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wg.hnjuh.cn

[R05] 参数默认值
来源：http://xn.huixinmuqiang.cn

name="${1:-default}"
来源：http://ir.szxytkj.cn

[R06] 判断命令是否存在
来源：http://ce.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ry.colortex.cn

[R07] if 判断文件
来源：http://te.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pu.chemitech.net.cn

[R08] 数值比较
来源：http://qt.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ug.colortex.cn

[R09] 字符串比较
来源：http://th.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ng.jctech888.com.cn

[R10] 正则匹配
来源：http://ek.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lz.szxytkj.cn

[R11] case 多分支
来源：http://bn.shxzukj.cn

case "$1" in
来源：http://vo.gzmigu.cn

start) echo "启动" ;;
来源：http://up.hnjuh.cn

stop)  echo "停止" ;;
来源：http://rz.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://zk.hnjuh.cn

esac
来源：http://rh.bjjhwx.cn

[R12] for 遍历文件
来源：http://bl.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://xw.wgjwhj.cn

[R13] for 计数循环
来源：http://sg.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://um.asd995.cn

[R14] C 风格 for
来源：http://cr.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ej.nszjky.cn

[R15] while 逐行读文件
来源：http://go.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dj.shtwfgs.cn

[R16] until 等待条件
来源：http://ay.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bb.haigaiapp.cn

[R17] 数组定义与取值
来源：http://zr.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pp.lnxyls.cn

[R18] 遍历数组
来源：http://us.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nl.gzmigu.cn

[R19] 数组长度
来源：http://ov.521024.cn

echo "${#arr[@]}"
来源：http://qh.shxzskj.cn

[R20] 关联数组（字典）
来源：http://fu.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uu.haigaiapp.cn

[R21] 字符串长度
来源：http://fm.hahajie.cn

echo "${#s}"
来源：http://pm.muxihuayi.cn

[R22] 截取子串
来源：http://rn.bookmarksfly.cn

echo "${s:0:5}"
来源：http://df.bookmarksfly.cn

[R23] 字符串替换
来源：http://ih.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rx.hnjuh.cn

[R24] 大小写转换
来源：http://up.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lr.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://ic.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lf.huixiangedu.cn

[R26] 命令替换
来源：http://fs.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://aq.shxzukj.cn

[R27] 算术展开
来源：http://lf.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://yt.huixinmuqiang.cn

[R28] 浮点运算
来源：http://ul.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://vk.huixiangedu.cn

[R29] 定义函数
来源：http://fm.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ko.panjiajie.cn

[R30] 函数返回状态码
来源：http://kw.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://rq.huanxung.cn

[R31] 局部变量
来源：http://xs.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://qd.9csxet.cn

[R32] 参数个数校验
来源：http://zs.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wp.colortex.cn

[R33] 捕获错误并提示行号
来源：http://yq.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cc.colortex.cn

[R34] 退出时清理
来源：http://ce.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vq.lnxyls.cn

[R35] 后台执行并等待
来源：http://cm.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yk.lnxyls.cn

[R36] 并发执行多个任务
来源：http://bc.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://li.newstarts.cn

[R37] 把输出赋给变量
来源：http://zr.521024.cn

files=$(ls -1)
来源：http://rt.lnxyls.cn

[R38] 管道串联
来源：http://ar.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://gg.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://gl.panjiajie.cn

cmd > out.log 2>&1
来源：http://ri.bookmarksfly.cn

[R40] 追加写日志
来源：http://ql.jctech888.com.cn

echo "log" >> out.log
来源：http://ay.szsharing.cn

[R41] 丢弃输出
来源：http://ze.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://dd.hnjuh.cn

[R42] 输入重定向
来源：http://iv.gzmigu.cn

wc -l < a.txt
来源：http://bj.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://xm.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://yy.bjjhwx.cn

[R44] 按修改时间查找
来源：http://ry.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://lb.nicolike.cn

[R45] 批量删除
来源：http://rn.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://wy.szsharing.cn

[R46] 递归替换文件内容
来源：http://xy.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rs.lnxyls.cn

[R47] sed 单行替换
来源：http://qj.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kj.nszjky.cn

[R48] awk 取指定列
来源：http://fc.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://nn.huanxung.cn

[R49] awk 带条件
来源：http://zp.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fa.lnxyls.cn

[R50] awk 求和
来源：http://gh.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vr.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://rt.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cx.wgjwhj.cn

[R52] 统计行数
来源：http://mp.hahajie.cn

wc -l a.txt
来源：http://jh.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://js.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mu.szsharing.cn

[R54] 比较两个文件
来源：http://px.panjiajie.cn

diff a.txt b.txt
来源：http://fa.hahajie.cn

[R55] 压缩与解压
来源：http://kt.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mk.gzmigu.cn

[R56] 远程拷贝
来源：http://tu.nicolike.cn

scp file user@host:/path/
来源：http://gq.wgjwhj.cn

[R57] 远程执行命令
来源：http://gm.huanxung.cn

ssh user@host 'uptime'
来源：http://hb.9csxet.cn

[R58] 下载文件
来源：http://dm.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dh.panjiajie.cn

[R59] 发 POST JSON
来源：http://hd.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ij.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://gm.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://km.szxytkj.cn

[R61] 磁盘占用
来源：http://sw.huixiangedu.cn

df -h;  du -sh *
来源：http://sf.panjiajie.cn

[R62] 找最占空间的文件
来源：http://wr.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://wn.lnxyls.cn

[R63] 内存与进程
来源：http://gu.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://ek.gzmigu.cn

[R64] 结束进程
来源：http://nq.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://za.bookmarksfly.cn

[R65] 查看端口占用
来源：http://av.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nr.bjjhwx.cn

[R66] 定时任务
来源：http://ay.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://vw.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://zh.asd995.cn

openssl rand -hex 16
来源：http://mr.colortex.cn

[R68] 计算文件校验值
来源：http://co.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lr.shxzukj.cn

[R69] 生成随机密码
来源：http://fc.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://mg.lnxyls.cn

[R70] 时间戳与互转
来源：http://qe.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://fv.jianghongdianzi.cn

[R71] 日期格式化
来源：http://qs.shxzskj.cn


<!-- 参考信息 -->