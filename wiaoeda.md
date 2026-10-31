代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://zw.colortex.cn

[Q22] 排序
来源：http://ns.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ne.lnxyls.cn

[Q23] 分页
来源：http://hv.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://en.9csxet.cn

[Q24] 去重
来源：http://ck.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://az.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://sw.yuexingan06.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jk.wgjwhj.cn

[Q26] 计数
来源：http://im.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://vt.lnxyls.cn

[Q27] 条件计数
来源：http://cu.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iq.muxihuayi.cn

[Q28] 求和与平均
来源：http://ka.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nu.colortex.cn

[Q29] 最大最小值
来源：http://qc.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sh.shxzskj.cn

[Q30] 分组统计
来源：http://ks.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xl.colortex.cn

[Q31] 分组后过滤
来源：http://ai.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oc.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://zp.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jm.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://da.nszjky.cn

[Q33] 多列分组
来源：http://ff.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nl.szxytkj.cn

[Q34] 每组取第一条
来源：http://re.gzmigu.cn

SELECT * FROM (
来源：http://fw.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ug.yuexingan06.cn

) t WHERE rn = 1;
来源：http://rz.newstarts.cn

[Q35] 内连接
来源：http://nf.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mk.lnxyls.cn

[Q36] 左连接
来源：http://we.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wq.chemitech.net.cn

[Q37] 右连接
来源：http://al.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gy.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sw.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ni.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://ff.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xm.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sq.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dj.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://no.yuexingan06.cn

[Q41] 多表连接
来源：http://ln.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ul.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://ck.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://wh.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://xg.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://ul.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gs.shxzskj.cn

[Q43] 标量子查询
来源：http://pz.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zw.gzmigu.cn

[Q44] IN 子查询
来源：http://ku.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yq.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://ew.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ri.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vk.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://so.lnxyls.cn

[Q47] 与平均值比较
来源：http://fu.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yf.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://ve.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pq.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://bt.shtwfgs.cn

[Q49] 更新单行
来源：http://ga.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fw.hahajie.cn

[Q50] 批量更新
来源：http://or.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iz.gzmigu.cn

[Q51] 用子查询更新
来源：http://re.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pm.newstarts.cn

[Q52] 删除指定行
来源：http://dp.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://kv.muxihuayi.cn

[Q53] 按条件删除
来源：http://up.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xy.colortex.cn

[Q54] 清空表
来源：http://al.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://fw.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://jr.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ta.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://vl.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wf.haigaiapp.cn

[Q57] 行号
来源：http://vn.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iv.szxytkj.cn

[Q58] 累计求和
来源：http://zl.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nd.hahajie.cn

[Q59] 分组内累计
来源：http://mx.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ml.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://wl.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yx.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sh.asd995.cn

[Q61] 移动平均
来源：http://my.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uk.szxytkj.cn

[Q62] 分组占比
来源：http://sg.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ke.muxihuayi.cn

[Q63] 开启事务
来源：http://qc.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vn.panjiajie.cn

[Q64] 提交事务
来源：http://ry.muxihuayi.cn

COMMIT;
来源：http://dw.gzmigu.cn

[Q65] 回滚事务
来源：http://jp.jctech888.com.cn

ROLLBACK;
来源：http://mj.panjiajie.cn

[Q66] 行锁查询
来源：http://yz.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ao.huanxung.cn

[Q67] 设置隔离级别
来源：http://gl.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gx.chemitech.net.cn

[Q68] 保存点
来源：http://up.521024.cn

SAVEPOINT sp1;
来源：http://fe.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://wc.newstarts.cn

[Q69] 查看执行计划
来源：http://sv.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ik.szxytkj.cn

[Q70] 更新统计信息
来源：http://co.shxzukj.cn

ANALYZE TABLE users;
来源：http://pd.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://po.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dk.haigaiapp.cn

[Q72] 查看索引
来源：http://nf.shxzskj.cn

SHOW INDEX FROM users;
来源：http://qh.asd995.cn

[Q73] 查看表状态
来源：http://lq.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vk.yuexingan06.cn

[Q74] 强制使用索引
来源：http://iu.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vr.shxzskj.cn

[Q75] 日期格式化
来源：http://zc.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dp.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://js.lnxyls.cn

[Q76] 按天统计
来源：http://nf.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://or.huixiangedu.cn

[Q77] 时间加减
来源：http://ty.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sq.nszjky.cn

[Q78] 当前时间
来源：http://oq.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hn.newstarts.cn

[Q79] 字符串拼接
来源：http://du.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qt.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://ec.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vq.asd995.cn

[Q81] 字符串替换
来源：http://zz.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zj.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://jy.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fm.9csxet.cn

[Q83] 大小写转换
来源：http://gd.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yk.huanxung.cn

[Q84] 去除首尾空格
来源：http://hd.521024.cn

SELECT TRIM(name) FROM users;
来源：http://up.huixiangedu.cn

[Q85] 数值取整
来源：http://as.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ou.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://sy.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dw.521024.cn

[Q87] JSON 字段做条件
来源：http://rc.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hx.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://dg.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mm.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wy.colortex.cn

[Q89] 判断表是否存在
来源：http://kp.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tt.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://st.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://te.hnjuh.cn

================================================================================
来源：http://df.hnjuh.cn

R. Bash 专题
来源：http://zd.hahajie.cn

================================================================================
来源：http://xg.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://fk.szsharing.cn

#!/usr/bin/env bash
来源：http://ps.521024.cn

set -euo pipefail
来源：http://ay.nicolike.cn

[R02] 变量赋值与使用
来源：http://mj.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://zx.szsharing.cn

[R03] 只读变量
来源：http://jb.yuntaijiaju.cn

readonly PI=3.14
来源：http://br.shxzskj.cn

[R04] 位置参数
来源：http://sj.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hc.lnxyls.cn

[R05] 参数默认值
来源：http://uw.yuexingan06.cn

name="${1:-default}"
来源：http://ws.nszjky.cn

[R06] 判断命令是否存在
来源：http://tn.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ls.huixiangedu.cn

[R07] if 判断文件
来源：http://tk.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://th.szxytkj.cn

[R08] 数值比较
来源：http://kj.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://co.nicolike.cn

[R09] 字符串比较
来源：http://ql.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zm.wgjwhj.cn

[R10] 正则匹配
来源：http://rj.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fp.huixiangedu.cn

[R11] case 多分支
来源：http://fs.asd995.cn

case "$1" in
来源：http://li.lnxyls.cn

start) echo "启动" ;;
来源：http://oe.shxzskj.cn

stop)  echo "停止" ;;
来源：http://ja.521024.cn

*)     echo "未知命令" ;;
来源：http://ld.lnxyls.cn

esac
来源：http://or.gzmigu.cn

[R12] for 遍历文件
来源：http://mq.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://pl.shtwfgs.cn

[R13] for 计数循环
来源：http://vw.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://mj.shxzukj.cn

[R14] C 风格 for
来源：http://dj.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ps.yuexingan06.cn

[R15] while 逐行读文件
来源：http://pv.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ha.bjjhwx.cn

[R16] until 等待条件
来源：http://tv.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yy.colortex.cn

[R17] 数组定义与取值
来源：http://ey.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://du.muxihuayi.cn

[R18] 遍历数组
来源：http://xm.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tx.asd995.cn

[R19] 数组长度
来源：http://eo.yuexingan06.cn

echo "${#arr[@]}"
来源：http://ke.9csxet.cn

[R20] 关联数组（字典）
来源：http://qi.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bm.shxzukj.cn

[R21] 字符串长度
来源：http://vd.shtwfgs.cn

echo "${#s}"
来源：http://rl.lnxyls.cn

[R22] 截取子串
来源：http://sw.9csxet.cn

echo "${s:0:5}"
来源：http://ij.huixinmuqiang.cn

[R23] 字符串替换
来源：http://vz.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ek.shxzskj.cn

[R24] 大小写转换
来源：http://xl.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iz.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://eg.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://td.wgjwhj.cn

[R26] 命令替换
来源：http://yf.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://sn.nicolike.cn

[R27] 算术展开
来源：http://kd.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://tv.hnjuh.cn

[R28] 浮点运算
来源：http://ce.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://wx.bookmarksfly.cn

[R29] 定义函数
来源：http://xr.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://si.shxzukj.cn

[R30] 函数返回状态码
来源：http://cg.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://rg.huixinmuqiang.cn

[R31] 局部变量
来源：http://my.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://zb.nicolike.cn

[R32] 参数个数校验
来源：http://va.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gu.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://ou.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vh.jctech888.com.cn

[R34] 退出时清理
来源：http://ow.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oo.shxzukj.cn

[R35] 后台执行并等待
来源：http://je.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lq.nicolike.cn

[R36] 并发执行多个任务
来源：http://ti.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hj.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://xr.lnxyls.cn

files=$(ls -1)
来源：http://lb.hnjuh.cn

[R38] 管道串联
来源：http://ij.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://ei.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://ww.hnjuh.cn

cmd > out.log 2>&1
来源：http://uq.9csxet.cn

[R40] 追加写日志
来源：http://ty.nicolike.cn

echo "log" >> out.log
来源：http://hv.chemitech.net.cn

[R41] 丢弃输出
来源：http://ml.asd995.cn

cmd >/dev/null 2>&1
来源：http://il.bookmarksfly.cn

[R42] 输入重定向
来源：http://xv.bjjhwx.cn

wc -l < a.txt
来源：http://bk.muxihuayi.cn

[R43] 按名字查找文件
来源：http://pr.shtwfgs.cn

find . -name "*.log" -type f
来源：http://wt.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://fq.huixiangedu.cn

find . -mtime -7 -type f
来源：http://rn.huixiangedu.cn

[R45] 批量删除
来源：http://ko.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://sm.szxytkj.cn

[R46] 递归替换文件内容
来源：http://tm.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://db.gzmigu.cn

[R47] sed 单行替换
来源：http://pt.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mx.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://nn.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://if.jianghongdianzi.cn

[R49] awk 带条件
来源：http://lf.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://um.shxzukj.cn

[R50] awk 求和
来源：http://cc.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ny.hahajie.cn

[R51] 排序去重取前几
来源：http://cm.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jv.shxzskj.cn

[R52] 统计行数
来源：http://fc.huanxung.cn

wc -l a.txt
来源：http://ty.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://wi.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kh.hnjuh.cn

[R54] 比较两个文件
来源：http://dg.colortex.cn

diff a.txt b.txt
来源：http://td.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://qk.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xh.9csxet.cn

[R56] 远程拷贝
来源：http://td.asd995.cn

scp file user@host:/path/
来源：http://iy.521024.cn

[R57] 远程执行命令
来源：http://pi.521024.cn

ssh user@host 'uptime'
来源：http://co.yuexingan06.cn

[R58] 下载文件
来源：http://uo.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aw.lnxyls.cn

[R59] 发 POST JSON
来源：http://bm.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vv.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://qf.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ph.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://hd.jctech888.com.cn

df -h;  du -sh *
来源：http://ue.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://zq.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://wu.hnjuh.cn

[R63] 内存与进程
来源：http://ei.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://oi.huixiangedu.cn

[R64] 结束进程
来源：http://mj.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://vh.szxytkj.cn

[R65] 查看端口占用
来源：http://wq.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ke.hahajie.cn

[R66] 定时任务
来源：http://dw.9csxet.cn

crontab -e;  crontab -l
来源：http://hm.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://aq.szxytkj.cn

openssl rand -hex 16
来源：http://fs.muxihuayi.cn

[R68] 计算文件校验值
来源：http://ub.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lq.521024.cn

[R69] 生成随机密码
来源：http://ap.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://zf.jctech888.com.cn

[R70] 时间戳与互转
来源：http://sd.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://dn.szxytkj.cn

[R71] 日期格式化
来源：http://tx.chemitech.net.cn


<!-- 参考信息 -->