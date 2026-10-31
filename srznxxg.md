代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zk.bjjhwx.cn

) t WHERE rn = 1;
来源：http://yf.muxihuayi.cn

[Q35] 内连接
来源：http://xi.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fr.nicolike.cn

[Q36] 左连接
来源：http://js.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zx.muxihuayi.cn

[Q37] 右连接
来源：http://ki.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xm.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bs.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pc.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://xc.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uv.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gl.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lj.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://me.gzmigu.cn

[Q41] 多表连接
来源：http://or.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gi.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://nk.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://zt.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://jh.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://ob.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gc.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://ho.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wj.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://dz.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://er.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://ke.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kc.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gc.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://am.newstarts.cn

[Q47] 与平均值比较
来源：http://tg.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lh.colortex.cn

[Q48] CTE 公用表表达式
来源：http://ia.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bm.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ip.hahajie.cn

[Q49] 更新单行
来源：http://ov.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://be.gzmigu.cn

[Q50] 批量更新
来源：http://cs.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fy.colortex.cn

[Q51] 用子查询更新
来源：http://lo.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pj.jctech888.com.cn

[Q52] 删除指定行
来源：http://zf.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://mh.haigaiapp.cn

[Q53] 按条件删除
来源：http://lh.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bk.9csxet.cn

[Q54] 清空表
来源：http://qs.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://zc.nszjky.cn

[Q55] 排名（并列占位）
来源：http://hd.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oe.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://li.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hl.szsharing.cn

[Q57] 行号
来源：http://sv.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://of.huixiangedu.cn

[Q58] 累计求和
来源：http://ji.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nb.wgjwhj.cn

[Q59] 分组内累计
来源：http://su.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://su.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://tp.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ta.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pd.nicolike.cn

[Q61] 移动平均
来源：http://tw.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dv.colortex.cn

[Q62] 分组占比
来源：http://pw.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tc.haigaiapp.cn

[Q63] 开启事务
来源：http://tw.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hr.muxihuayi.cn

[Q64] 提交事务
来源：http://rp.szxytkj.cn

COMMIT;
来源：http://fi.yuexingan06.cn

[Q65] 回滚事务
来源：http://nw.huixinmuqiang.cn

ROLLBACK;
来源：http://bj.szsharing.cn

[Q66] 行锁查询
来源：http://wd.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://br.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://po.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iy.chemitech.net.cn

[Q68] 保存点
来源：http://zi.nszjky.cn

SAVEPOINT sp1;
来源：http://zp.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://fv.bjjhwx.cn

[Q69] 查看执行计划
来源：http://al.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tj.chemitech.net.cn

[Q70] 更新统计信息
来源：http://lc.szxytkj.cn

ANALYZE TABLE users;
来源：http://il.nicolike.cn

[Q71] 查看建表语句
来源：http://yu.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wf.shtwfgs.cn

[Q72] 查看索引
来源：http://cy.hnjuh.cn

SHOW INDEX FROM users;
来源：http://qb.lnxyls.cn

[Q73] 查看表状态
来源：http://qg.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ah.newstarts.cn

[Q74] 强制使用索引
来源：http://ge.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jb.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://kb.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://le.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sf.huanxung.cn

[Q76] 按天统计
来源：http://vz.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vz.hnjuh.cn

[Q77] 时间加减
来源：http://mr.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fa.shxzukj.cn

[Q78] 当前时间
来源：http://xp.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lg.shxzukj.cn

[Q79] 字符串拼接
来源：http://br.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ib.hahajie.cn

[Q80] 字符串截取
来源：http://yn.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wu.gzmigu.cn

[Q81] 字符串替换
来源：http://te.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ib.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://uc.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rq.521024.cn

[Q83] 大小写转换
来源：http://el.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://so.szxytkj.cn

[Q84] 去除首尾空格
来源：http://wo.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://vk.szsharing.cn

[Q85] 数值取整
来源：http://cj.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://en.colortex.cn

[Q86] 读取 JSON 字段
来源：http://ra.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qp.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://sv.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qh.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://ok.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wn.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hu.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://ql.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iv.hnjuh.cn

[Q90] 生成序号列
来源：http://kp.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://um.huanxung.cn

================================================================================
来源：http://cd.jianghongdianzi.cn

R. Bash 专题
来源：http://zp.huixinmuqiang.cn

================================================================================
来源：http://sj.shxzskj.cn

[R01] shebang 与严格模式
来源：http://nd.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://pa.bookmarksfly.cn

set -euo pipefail
来源：http://ix.colortex.cn

[R02] 变量赋值与使用
来源：http://gc.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://iv.jianghongdianzi.cn

[R03] 只读变量
来源：http://jp.hahajie.cn

readonly PI=3.14
来源：http://ed.yuexingan06.cn

[R04] 位置参数
来源：http://in.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://do.521024.cn

[R05] 参数默认值
来源：http://gs.lnxyls.cn

name="${1:-default}"
来源：http://dn.nicolike.cn

[R06] 判断命令是否存在
来源：http://zd.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wu.chemitech.net.cn

[R07] if 判断文件
来源：http://lr.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oj.muxihuayi.cn

[R08] 数值比较
来源：http://ro.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wh.newstarts.cn

[R09] 字符串比较
来源：http://wd.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yt.szxytkj.cn

[R10] 正则匹配
来源：http://gl.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://id.haigaiapp.cn

[R11] case 多分支
来源：http://yc.muxihuayi.cn

case "$1" in
来源：http://fl.panjiajie.cn

start) echo "启动" ;;
来源：http://kv.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://ri.colortex.cn

*)     echo "未知命令" ;;
来源：http://ya.wgjwhj.cn

esac
来源：http://kd.newstarts.cn

[R12] for 遍历文件
来源：http://zd.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://tr.yuexingan06.cn

[R13] for 计数循环
来源：http://ob.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://uq.gzmigu.cn

[R14] C 风格 for
来源：http://dy.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wk.panjiajie.cn

[R15] while 逐行读文件
来源：http://ej.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jq.jctech888.com.cn

[R16] until 等待条件
来源：http://bg.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vt.9csxet.cn

[R17] 数组定义与取值
来源：http://rs.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fo.gzmigu.cn

[R18] 遍历数组
来源：http://zs.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uv.nicolike.cn

[R19] 数组长度
来源：http://il.nszjky.cn

echo "${#arr[@]}"
来源：http://th.asd995.cn

[R20] 关联数组（字典）
来源：http://zk.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ao.chemitech.net.cn

[R21] 字符串长度
来源：http://jj.hahajie.cn

echo "${#s}"
来源：http://id.yuexingan06.cn

[R22] 截取子串
来源：http://bb.shxzskj.cn

echo "${s:0:5}"
来源：http://yy.wgjwhj.cn

[R23] 字符串替换
来源：http://gu.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ek.521024.cn

[R24] 大小写转换
来源：http://lm.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uy.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://yw.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dd.haigaiapp.cn

[R26] 命令替换
来源：http://bp.asd995.cn

now=$(date +%F); echo "$now"
来源：http://bb.yuexingan06.cn

[R27] 算术展开
来源：http://od.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://bp.shtwfgs.cn

[R28] 浮点运算
来源：http://nr.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://hg.nszjky.cn

[R29] 定义函数
来源：http://tn.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aj.shxzukj.cn

[R30] 函数返回状态码
来源：http://uw.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://qp.gzmigu.cn

[R31] 局部变量
来源：http://ez.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://lu.newstarts.cn

[R32] 参数个数校验
来源：http://pz.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://as.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://dv.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zu.jctech888.com.cn

[R34] 退出时清理
来源：http://sv.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lk.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://hi.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zt.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://ih.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cj.hnjuh.cn

[R37] 把输出赋给变量
来源：http://fl.521024.cn

files=$(ls -1)
来源：http://va.szsharing.cn

[R38] 管道串联
来源：http://nn.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://xo.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://tk.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://qk.panjiajie.cn

[R40] 追加写日志
来源：http://iv.colortex.cn

echo "log" >> out.log
来源：http://pr.colortex.cn

[R41] 丢弃输出
来源：http://bd.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://ke.szsharing.cn

[R42] 输入重定向
来源：http://no.shxzukj.cn

wc -l < a.txt
来源：http://zc.huixiangedu.cn

[R43] 按名字查找文件
来源：http://ic.jctech888.com.cn

find . -name "*.log" -type f
来源：http://ht.szsharing.cn

[R44] 按修改时间查找
来源：http://wr.szsharing.cn

find . -mtime -7 -type f
来源：http://xv.huixinmuqiang.cn

[R45] 批量删除
来源：http://ki.nszjky.cn

find . -name "*.tmp" -delete
来源：http://qu.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://mk.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nx.haigaiapp.cn

[R47] sed 单行替换
来源：http://wc.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ir.huixiangedu.cn

[R48] awk 取指定列
来源：http://ui.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://kw.jianghongdianzi.cn

[R49] awk 带条件
来源：http://ay.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ep.521024.cn

[R50] awk 求和
来源：http://ku.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pe.huanxung.cn

[R51] 排序去重取前几
来源：http://xq.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://to.hnjuh.cn

[R52] 统计行数
来源：http://og.jctech888.com.cn

wc -l a.txt
来源：http://sl.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://vo.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vw.gzmigu.cn

[R54] 比较两个文件
来源：http://of.gzmigu.cn

diff a.txt b.txt
来源：http://oq.lnxyls.cn

[R55] 压缩与解压
来源：http://qu.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dv.yuexingan06.cn

[R56] 远程拷贝
来源：http://lf.huanxung.cn

scp file user@host:/path/
来源：http://vb.huixiangedu.cn

[R57] 远程执行命令
来源：http://md.newstarts.cn

ssh user@host 'uptime'
来源：http://tr.muxihuayi.cn

[R58] 下载文件
来源：http://pj.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kz.colortex.cn

[R59] 发 POST JSON
来源：http://xm.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nc.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://cm.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mr.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://ap.hnjuh.cn

df -h;  du -sh *
来源：http://eq.shxzukj.cn

[R62] 找最占空间的文件
来源：http://wi.asd995.cn

du -ah . | sort -rh | head -10
来源：http://zo.nszjky.cn

[R63] 内存与进程
来源：http://rm.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://qv.colortex.cn

[R64] 结束进程
来源：http://dd.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://fm.bookmarksfly.cn

[R65] 查看端口占用
来源：http://hj.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wi.shxzskj.cn

[R66] 定时任务
来源：http://pq.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://jy.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://ns.nszjky.cn

openssl rand -hex 16
来源：http://fu.haigaiapp.cn

[R68] 计算文件校验值
来源：http://kh.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hx.nicolike.cn

[R69] 生成随机密码
来源：http://xb.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://qr.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://ko.9csxet.cn

date +%s;  date -d @1700000000
来源：http://vp.chemitech.net.cn

[R71] 日期格式化
来源：http://oj.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ng.hnjuh.cn

[R72] 等待端口就绪
来源：http://im.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ix.lnxyls.cn

[R73] 分割大日志
来源：http://ro.bjjhwx.cn

split -l 1000 big.log part_
来源：http://yi.szxytkj.cn

[R74] 批量重命名
来源：http://en.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xh.hahajie.cn

[R75] 导出环境变量
来源：http://ra.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://vs.9csxet.cn

[R76] 使用临时文件
来源：http://yf.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kx.shxzukj.cn

[R77] 读取用户输入
来源：http://rp.gzmigu.cn

read -rp "请输入: " ans
来源：http://vj.newstarts.cn

[R78] 交互式菜单
来源：http://gg.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gy.colortex.cn

[R79] 解析命令行选项
来源：http://te.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gn.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://lh.haigaiapp.cn

time ./run.sh
来源：http://rw.huixinmuqiang.cn

================================================================================
来源：http://dq.bjjhwx.cn

S. C / C++ 专题
来源：http://qo.huanxung.cn

================================================================================
来源：http://lc.bookmarksfly.cn

[S01] C：Hello World
来源：http://xf.shxzskj.cn

#include <stdio.h>
来源：http://gk.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sx.colortex.cn

[S02] C：变量与格式化输出
来源：http://vz.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://zn.hnjuh.cn

[S03] C：读入整数
来源：http://tp.shxzukj.cn


<!-- 参考信息 -->