代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://di.9csxet.cn

[Q18] 模糊匹配
来源：http://jm.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nf.nicolike.cn

[Q19] 范围查询
来源：http://px.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wb.jianghongdianzi.cn

[Q20] IN 列表
来源：http://ns.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zm.huixiangedu.cn

[Q21] 空值判断
来源：http://eu.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://he.nicolike.cn

[Q22] 排序
来源：http://na.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://je.huanxung.cn

[Q23] 分页
来源：http://uk.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kg.hnjuh.cn

[Q24] 去重
来源：http://ux.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://bc.nszjky.cn

[Q25] 只取前 N 条
来源：http://dq.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ki.newstarts.cn

[Q26] 计数
来源：http://ht.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://lm.jianghongdianzi.cn

[Q27] 条件计数
来源：http://vm.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zu.bjjhwx.cn

[Q28] 求和与平均
来源：http://ay.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hi.shxzukj.cn

[Q29] 最大最小值
来源：http://jf.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://of.jianghongdianzi.cn

[Q30] 分组统计
来源：http://lv.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xp.chemitech.net.cn

[Q31] 分组后过滤
来源：http://ne.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wv.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://mm.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qi.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xt.nicolike.cn

[Q33] 多列分组
来源：http://dv.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pg.yuexingan06.cn

[Q34] 每组取第一条
来源：http://ep.gzmigu.cn

SELECT * FROM (
来源：http://hn.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zg.bjjhwx.cn

) t WHERE rn = 1;
来源：http://bc.szxytkj.cn

[Q35] 内连接
来源：http://rq.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iz.shtwfgs.cn

[Q36] 左连接
来源：http://px.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ps.huixinmuqiang.cn

[Q37] 右连接
来源：http://qp.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mf.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qx.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zt.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://fu.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pi.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uy.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wd.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wn.colortex.cn

[Q41] 多表连接
来源：http://tj.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tj.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://ze.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://gy.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://wy.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://of.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bu.bookmarksfly.cn

[Q43] 标量子查询
来源：http://wc.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bc.521024.cn

[Q44] IN 子查询
来源：http://im.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kp.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://ua.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uq.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sr.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qo.521024.cn

[Q47] 与平均值比较
来源：http://za.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mi.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://xd.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vw.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://ek.bjjhwx.cn

[Q49] 更新单行
来源：http://pg.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vo.lnxyls.cn

[Q50] 批量更新
来源：http://ca.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qp.jctech888.com.cn

[Q51] 用子查询更新
来源：http://xx.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wn.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://me.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://mb.bjjhwx.cn

[Q53] 按条件删除
来源：http://yj.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lu.hahajie.cn

[Q54] 清空表
来源：http://gs.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://un.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://kr.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ig.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://rv.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oi.bjjhwx.cn

[Q57] 行号
来源：http://as.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pz.huixinmuqiang.cn

[Q58] 累计求和
来源：http://th.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gc.hahajie.cn

[Q59] 分组内累计
来源：http://vs.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vd.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://lo.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jo.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rm.haigaiapp.cn

[Q61] 移动平均
来源：http://gr.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fk.hahajie.cn

[Q62] 分组占比
来源：http://po.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wx.yuexingan06.cn

[Q63] 开启事务
来源：http://mq.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rq.huixinmuqiang.cn

[Q64] 提交事务
来源：http://eo.nicolike.cn

COMMIT;
来源：http://ay.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://ez.chemitech.net.cn

ROLLBACK;
来源：http://nd.521024.cn

[Q66] 行锁查询
来源：http://zd.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ea.szxytkj.cn

[Q67] 设置隔离级别
来源：http://jk.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ad.yuexingan06.cn

[Q68] 保存点
来源：http://or.hnjuh.cn

SAVEPOINT sp1;
来源：http://qg.hnjuh.cn

ROLLBACK TO sp1;
来源：http://qu.gzmigu.cn

[Q69] 查看执行计划
来源：http://iz.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ue.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://hf.9csxet.cn

ANALYZE TABLE users;
来源：http://yv.muxihuayi.cn

[Q71] 查看建表语句
来源：http://gp.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ox.bookmarksfly.cn

[Q72] 查看索引
来源：http://qi.szxytkj.cn

SHOW INDEX FROM users;
来源：http://eo.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://ro.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sn.wgjwhj.cn

[Q74] 强制使用索引
来源：http://da.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dz.shxzskj.cn

[Q75] 日期格式化
来源：http://tr.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nx.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ha.szxytkj.cn

[Q76] 按天统计
来源：http://sv.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qu.nicolike.cn

[Q77] 时间加减
来源：http://ki.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dp.shtwfgs.cn

[Q78] 当前时间
来源：http://cg.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://la.jctech888.com.cn

[Q79] 字符串拼接
来源：http://ur.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ik.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://uq.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ak.9csxet.cn

[Q81] 字符串替换
来源：http://ej.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yo.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://ey.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kt.szxytkj.cn

[Q83] 大小写转换
来源：http://yd.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qz.lnxyls.cn

[Q84] 去除首尾空格
来源：http://hc.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://mt.lnxyls.cn

[Q85] 数值取整
来源：http://dr.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sa.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://fk.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://af.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://et.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rg.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://bb.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qr.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://im.9csxet.cn

[Q89] 判断表是否存在
来源：http://xs.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sw.muxihuayi.cn

[Q90] 生成序号列
来源：http://rq.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ou.szsharing.cn

================================================================================
来源：http://ky.bjjhwx.cn

R. Bash 专题
来源：http://af.gzmigu.cn

================================================================================
来源：http://va.szsharing.cn

[R01] shebang 与严格模式
来源：http://ae.muxihuayi.cn

#!/usr/bin/env bash
来源：http://qo.hnjuh.cn

set -euo pipefail
来源：http://ic.hnjuh.cn

[R02] 变量赋值与使用
来源：http://ik.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://gj.9csxet.cn

[R03] 只读变量
来源：http://at.521024.cn

readonly PI=3.14
来源：http://cn.bookmarksfly.cn

[R04] 位置参数
来源：http://he.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bu.shxzskj.cn

[R05] 参数默认值
来源：http://bg.muxihuayi.cn

name="${1:-default}"
来源：http://fn.szxytkj.cn

[R06] 判断命令是否存在
来源：http://rt.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xl.asd995.cn

[R07] if 判断文件
来源：http://xx.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gh.shtwfgs.cn

[R08] 数值比较
来源：http://qu.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ki.shxzukj.cn

[R09] 字符串比较
来源：http://uw.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ic.jctech888.com.cn

[R10] 正则匹配
来源：http://dy.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dd.lnxyls.cn

[R11] case 多分支
来源：http://yo.jianghongdianzi.cn

case "$1" in
来源：http://qq.huanxung.cn

start) echo "启动" ;;
来源：http://mn.szsharing.cn

stop)  echo "停止" ;;
来源：http://cu.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://hw.bjjhwx.cn

esac
来源：http://qw.gzmigu.cn

[R12] for 遍历文件
来源：http://ew.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://vi.hnjuh.cn

[R13] for 计数循环
来源：http://kr.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://xn.chemitech.net.cn

[R14] C 风格 for
来源：http://em.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://np.asd995.cn

[R15] while 逐行读文件
来源：http://dq.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xe.jctech888.com.cn

[R16] until 等待条件
来源：http://ni.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jt.huixiangedu.cn

[R17] 数组定义与取值
来源：http://gk.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://js.huixinmuqiang.cn

[R18] 遍历数组
来源：http://wj.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lf.nicolike.cn

[R19] 数组长度
来源：http://xb.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://si.asd995.cn

[R20] 关联数组（字典）
来源：http://am.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sw.yuexingan06.cn

[R21] 字符串长度
来源：http://og.szsharing.cn

echo "${#s}"
来源：http://kr.szxytkj.cn

[R22] 截取子串
来源：http://fc.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://dc.9csxet.cn

[R23] 字符串替换
来源：http://pp.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dd.muxihuayi.cn

[R24] 大小写转换
来源：http://lb.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rk.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://da.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eq.szxytkj.cn

[R26] 命令替换
来源：http://dl.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://pq.jianghongdianzi.cn

[R27] 算术展开
来源：http://pi.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://fw.9csxet.cn

[R28] 浮点运算
来源：http://nu.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://ge.shtwfgs.cn

[R29] 定义函数
来源：http://lq.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pf.chemitech.net.cn

[R30] 函数返回状态码
来源：http://hu.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://vj.nicolike.cn

[R31] 局部变量
来源：http://kg.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://iy.szxytkj.cn

[R32] 参数个数校验
来源：http://do.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jh.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://ct.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ac.huixinmuqiang.cn

[R34] 退出时清理
来源：http://nw.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lw.521024.cn

[R35] 后台执行并等待
来源：http://ek.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://id.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://pj.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uz.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://gn.bookmarksfly.cn

files=$(ls -1)
来源：http://xw.bjjhwx.cn

[R38] 管道串联
来源：http://ua.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://sc.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://yh.521024.cn

cmd > out.log 2>&1
来源：http://vt.panjiajie.cn

[R40] 追加写日志
来源：http://jq.szxytkj.cn

echo "log" >> out.log
来源：http://bp.bookmarksfly.cn

[R41] 丢弃输出
来源：http://kx.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://kg.haigaiapp.cn

[R42] 输入重定向
来源：http://kf.newstarts.cn

wc -l < a.txt
来源：http://hm.521024.cn

[R43] 按名字查找文件
来源：http://fo.szxytkj.cn

find . -name "*.log" -type f
来源：http://ek.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://vz.521024.cn

find . -mtime -7 -type f
来源：http://ue.gzmigu.cn

[R45] 批量删除
来源：http://gk.asd995.cn

find . -name "*.tmp" -delete
来源：http://il.colortex.cn

[R46] 递归替换文件内容
来源：http://bg.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kb.521024.cn

[R47] sed 单行替换
来源：http://oe.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rp.newstarts.cn

[R48] awk 取指定列
来源：http://vy.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://vq.huixiangedu.cn

[R49] awk 带条件
来源：http://jh.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bu.nszjky.cn

[R50] awk 求和
来源：http://ze.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ld.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://tv.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ek.shtwfgs.cn

[R52] 统计行数
来源：http://hg.nszjky.cn

wc -l a.txt
来源：http://eo.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://ax.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nx.lnxyls.cn

[R54] 比较两个文件
来源：http://lz.lnxyls.cn

diff a.txt b.txt
来源：http://tr.lnxyls.cn

[R55] 压缩与解压
来源：http://vc.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ek.shxzskj.cn

[R56] 远程拷贝
来源：http://wo.panjiajie.cn

scp file user@host:/path/
来源：http://zd.bookmarksfly.cn

[R57] 远程执行命令
来源：http://rv.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://yv.huanxung.cn

[R58] 下载文件
来源：http://sl.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ew.haigaiapp.cn

[R59] 发 POST JSON
来源：http://yt.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gz.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ba.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rk.shxzukj.cn

[R61] 磁盘占用
来源：http://sv.nicolike.cn

df -h;  du -sh *
来源：http://ee.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://vu.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://fs.szxytkj.cn

[R63] 内存与进程
来源：http://ta.asd995.cn

free -h;  ps aux | grep nginx
来源：http://fo.huanxung.cn

[R64] 结束进程
来源：http://al.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://wh.521024.cn

[R65] 查看端口占用
来源：http://bn.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ir.hahajie.cn

[R66] 定时任务
来源：http://vw.panjiajie.cn

crontab -e;  crontab -l
来源：http://ta.9csxet.cn

[R67] 生成随机十六进制串
来源：http://lo.521024.cn


<!-- 参考信息 -->