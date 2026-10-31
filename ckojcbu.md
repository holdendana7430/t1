代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bg.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://zr.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://io.wgjwhj.cn

[Q19] 范围查询
来源：http://ks.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ot.yuexingan06.cn

[Q20] IN 列表
来源：http://hu.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gm.bookmarksfly.cn

[Q21] 空值判断
来源：http://vy.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://js.hnjuh.cn

[Q22] 排序
来源：http://cv.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hd.jianghongdianzi.cn

[Q23] 分页
来源：http://zr.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ey.9csxet.cn

[Q24] 去重
来源：http://gn.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://kc.huanxung.cn

[Q25] 只取前 N 条
来源：http://wb.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://py.521024.cn

[Q26] 计数
来源：http://nb.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://cm.bookmarksfly.cn

[Q27] 条件计数
来源：http://pm.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://er.panjiajie.cn

[Q28] 求和与平均
来源：http://sl.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cf.asd995.cn

[Q29] 最大最小值
来源：http://ht.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rl.shxzukj.cn

[Q30] 分组统计
来源：http://eu.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ja.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://xs.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pp.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://td.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jc.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hu.521024.cn

[Q33] 多列分组
来源：http://bx.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wb.colortex.cn

[Q34] 每组取第一条
来源：http://dw.asd995.cn

SELECT * FROM (
来源：http://an.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uv.bjjhwx.cn

) t WHERE rn = 1;
来源：http://zm.bjjhwx.cn

[Q35] 内连接
来源：http://zh.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hb.huixinmuqiang.cn

[Q36] 左连接
来源：http://fx.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dx.521024.cn

[Q37] 右连接
来源：http://xz.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qe.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jt.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hw.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://jc.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jx.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ha.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://im.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ok.huanxung.cn

[Q41] 多表连接
来源：http://ik.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fu.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://if.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://mg.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://ay.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://le.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xj.yuexingan06.cn

[Q43] 标量子查询
来源：http://bj.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pc.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://nv.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fw.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://iq.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xw.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sl.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bn.chemitech.net.cn

[Q47] 与平均值比较
来源：http://xn.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yf.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://cu.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://et.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://xb.shxzukj.cn

[Q49] 更新单行
来源：http://hb.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eh.hnjuh.cn

[Q50] 批量更新
来源：http://ts.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rc.521024.cn

[Q51] 用子查询更新
来源：http://jn.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nc.bjjhwx.cn

[Q52] 删除指定行
来源：http://as.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://vo.bjjhwx.cn

[Q53] 按条件删除
来源：http://vh.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lz.hahajie.cn

[Q54] 清空表
来源：http://js.521024.cn

TRUNCATE TABLE logs;
来源：http://kr.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://ug.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://za.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://bp.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gl.shxzskj.cn

[Q57] 行号
来源：http://gc.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yf.chemitech.net.cn

[Q58] 累计求和
来源：http://ru.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uy.shxzukj.cn

[Q59] 分组内累计
来源：http://do.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jn.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://sx.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ws.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://do.shxzskj.cn

[Q61] 移动平均
来源：http://un.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yq.colortex.cn

[Q62] 分组占比
来源：http://rf.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tq.bookmarksfly.cn

[Q63] 开启事务
来源：http://aj.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fp.muxihuayi.cn

[Q64] 提交事务
来源：http://nd.hnjuh.cn

COMMIT;
来源：http://xq.huixiangedu.cn

[Q65] 回滚事务
来源：http://fk.yuntaijiaju.cn

ROLLBACK;
来源：http://en.huixiangedu.cn

[Q66] 行锁查询
来源：http://xq.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gq.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://qa.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kx.asd995.cn

[Q68] 保存点
来源：http://zn.newstarts.cn

SAVEPOINT sp1;
来源：http://lh.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://zi.shtwfgs.cn

[Q69] 查看执行计划
来源：http://it.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xw.szsharing.cn

[Q70] 更新统计信息
来源：http://es.jctech888.com.cn

ANALYZE TABLE users;
来源：http://tn.hnjuh.cn

[Q71] 查看建表语句
来源：http://qo.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sl.jctech888.com.cn

[Q72] 查看索引
来源：http://av.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://aq.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://rx.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rf.wgjwhj.cn

[Q74] 强制使用索引
来源：http://it.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://al.wgjwhj.cn

[Q75] 日期格式化
来源：http://lo.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jv.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fr.jianghongdianzi.cn

[Q76] 按天统计
来源：http://rt.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nc.bookmarksfly.cn

[Q77] 时间加减
来源：http://sz.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://or.chemitech.net.cn

[Q78] 当前时间
来源：http://gr.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rf.szxytkj.cn

[Q79] 字符串拼接
来源：http://rc.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tw.lnxyls.cn

[Q80] 字符串截取
来源：http://no.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wq.asd995.cn

[Q81] 字符串替换
来源：http://ol.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ng.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://zn.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wm.shxzskj.cn

[Q83] 大小写转换
来源：http://iu.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dq.panjiajie.cn

[Q84] 去除首尾空格
来源：http://ka.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://og.shxzukj.cn

[Q85] 数值取整
来源：http://af.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yg.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://iy.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ov.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://gq.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pb.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://hx.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ny.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pd.hahajie.cn

[Q89] 判断表是否存在
来源：http://ss.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pn.nicolike.cn

[Q90] 生成序号列
来源：http://fu.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ha.hnjuh.cn

================================================================================
来源：http://rx.lnxyls.cn

R. Bash 专题
来源：http://cy.hahajie.cn

================================================================================
来源：http://wr.nicolike.cn

[R01] shebang 与严格模式
来源：http://yb.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://bh.chemitech.net.cn

set -euo pipefail
来源：http://ey.panjiajie.cn

[R02] 变量赋值与使用
来源：http://ab.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://eg.521024.cn

[R03] 只读变量
来源：http://qc.nicolike.cn

readonly PI=3.14
来源：http://ok.colortex.cn

[R04] 位置参数
来源：http://tb.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://db.newstarts.cn

[R05] 参数默认值
来源：http://pk.jianghongdianzi.cn

name="${1:-default}"
来源：http://wv.lnxyls.cn

[R06] 判断命令是否存在
来源：http://vm.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rc.jianghongdianzi.cn

[R07] if 判断文件
来源：http://zg.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bg.jianghongdianzi.cn

[R08] 数值比较
来源：http://ri.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ny.muxihuayi.cn

[R09] 字符串比较
来源：http://jl.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sv.szsharing.cn

[R10] 正则匹配
来源：http://df.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vo.huanxung.cn

[R11] case 多分支
来源：http://md.jctech888.com.cn

case "$1" in
来源：http://wy.yuexingan06.cn

start) echo "启动" ;;
来源：http://lp.nszjky.cn

stop)  echo "停止" ;;
来源：http://kg.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://uj.asd995.cn

esac
来源：http://iz.shxzukj.cn

[R12] for 遍历文件
来源：http://jv.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://ww.shtwfgs.cn

[R13] for 计数循环
来源：http://py.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://al.newstarts.cn

[R14] C 风格 for
来源：http://mx.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tr.hahajie.cn

[R15] while 逐行读文件
来源：http://sx.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tl.hahajie.cn

[R16] until 等待条件
来源：http://na.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qs.nszjky.cn

[R17] 数组定义与取值
来源：http://gj.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aw.newstarts.cn

[R18] 遍历数组
来源：http://kd.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gv.huixiangedu.cn

[R19] 数组长度
来源：http://cy.nszjky.cn

echo "${#arr[@]}"
来源：http://hm.gzmigu.cn

[R20] 关联数组（字典）
来源：http://sw.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uf.bjjhwx.cn

[R21] 字符串长度
来源：http://fr.yuexingan06.cn

echo "${#s}"
来源：http://gs.wgjwhj.cn

[R22] 截取子串
来源：http://st.nicolike.cn

echo "${s:0:5}"
来源：http://wd.yuntaijiaju.cn

[R23] 字符串替换
来源：http://en.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zm.colortex.cn

[R24] 大小写转换
来源：http://qb.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://df.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://sn.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mb.lnxyls.cn

[R26] 命令替换
来源：http://yk.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://by.huanxung.cn

[R27] 算术展开
来源：http://yt.szsharing.cn

echo $((1 + 2 * 3))
来源：http://zc.huanxung.cn

[R28] 浮点运算
来源：http://kk.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://da.gzmigu.cn

[R29] 定义函数
来源：http://wn.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ek.panjiajie.cn

[R30] 函数返回状态码
来源：http://yz.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://cb.yuntaijiaju.cn

[R31] 局部变量
来源：http://jn.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://nk.shxzukj.cn

[R32] 参数个数校验
来源：http://he.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://na.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://xr.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://os.szxytkj.cn

[R34] 退出时清理
来源：http://wj.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ki.muxihuayi.cn

[R35] 后台执行并等待
来源：http://jd.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uy.gzmigu.cn

[R36] 并发执行多个任务
来源：http://zz.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uz.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://tz.nszjky.cn

files=$(ls -1)
来源：http://zf.shxzukj.cn

[R38] 管道串联
来源：http://uc.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://wb.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://hy.yuexingan06.cn

cmd > out.log 2>&1
来源：http://xw.muxihuayi.cn

[R40] 追加写日志
来源：http://zf.hahajie.cn

echo "log" >> out.log
来源：http://ow.shtwfgs.cn

[R41] 丢弃输出
来源：http://qi.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://yp.szxytkj.cn

[R42] 输入重定向
来源：http://ed.yuexingan06.cn

wc -l < a.txt
来源：http://my.nszjky.cn

[R43] 按名字查找文件
来源：http://dy.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://ja.huixiangedu.cn

[R44] 按修改时间查找
来源：http://hz.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://pl.huixinmuqiang.cn

[R45] 批量删除
来源：http://gh.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://zk.shxzukj.cn

[R46] 递归替换文件内容
来源：http://dz.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pi.gzmigu.cn

[R47] sed 单行替换
来源：http://rr.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://if.yuexingan06.cn

[R48] awk 取指定列
来源：http://gn.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://zn.nszjky.cn

[R49] awk 带条件
来源：http://vp.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dl.wgjwhj.cn

[R50] awk 求和
来源：http://mw.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dv.lnxyls.cn

[R51] 排序去重取前几
来源：http://pr.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hx.9csxet.cn

[R52] 统计行数
来源：http://gl.nszjky.cn

wc -l a.txt
来源：http://ut.colortex.cn

[R53] 查看文件头与实时尾
来源：http://vl.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wo.colortex.cn

[R54] 比较两个文件
来源：http://tx.gzmigu.cn

diff a.txt b.txt
来源：http://ry.colortex.cn

[R55] 压缩与解压
来源：http://up.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rp.9csxet.cn

[R56] 远程拷贝
来源：http://jj.shxzukj.cn

scp file user@host:/path/
来源：http://za.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://kv.yuexingan06.cn

ssh user@host 'uptime'
来源：http://da.huixinmuqiang.cn

[R58] 下载文件
来源：http://ty.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iv.chemitech.net.cn

[R59] 发 POST JSON
来源：http://km.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ns.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://ot.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ko.newstarts.cn

[R61] 磁盘占用
来源：http://br.haigaiapp.cn

df -h;  du -sh *
来源：http://eu.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://ip.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://by.lnxyls.cn

[R63] 内存与进程
来源：http://dt.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://qg.chemitech.net.cn

[R64] 结束进程
来源：http://ja.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://tv.521024.cn

[R65] 查看端口占用
来源：http://dv.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qb.gzmigu.cn

[R66] 定时任务
来源：http://lq.521024.cn

crontab -e;  crontab -l
来源：http://pi.521024.cn

[R67] 生成随机十六进制串
来源：http://tp.yuntaijiaju.cn


<!-- 参考信息 -->