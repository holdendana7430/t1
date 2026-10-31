代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://xn.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://no.asd995.cn

[Q39] 自连接（查上下级）
来源：http://rp.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ei.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nu.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xw.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://es.jianghongdianzi.cn

[Q41] 多表连接
来源：http://ur.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oh.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://iu.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://rq.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://rf.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://ep.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ff.nszjky.cn

[Q43] 标量子查询
来源：http://hu.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ku.gzmigu.cn

[Q44] IN 子查询
来源：http://lw.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pe.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://bc.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ld.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://um.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rr.szsharing.cn

[Q47] 与平均值比较
来源：http://ij.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ye.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://zu.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tb.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://gu.yuexingan06.cn

[Q49] 更新单行
来源：http://pd.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lt.huanxung.cn

[Q50] 批量更新
来源：http://ad.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://st.jctech888.com.cn

[Q51] 用子查询更新
来源：http://xd.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uz.gzmigu.cn

[Q52] 删除指定行
来源：http://rr.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://lo.yuexingan06.cn

[Q53] 按条件删除
来源：http://vf.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tl.huixinmuqiang.cn

[Q54] 清空表
来源：http://lp.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://oc.asd995.cn

[Q55] 排名（并列占位）
来源：http://ig.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lo.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://dn.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qv.hnjuh.cn

[Q57] 行号
来源：http://ar.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zf.jianghongdianzi.cn

[Q58] 累计求和
来源：http://gh.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jv.colortex.cn

[Q59] 分组内累计
来源：http://iu.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tk.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://zv.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://by.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cd.asd995.cn

[Q61] 移动平均
来源：http://zt.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iy.wgjwhj.cn

[Q62] 分组占比
来源：http://yp.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tr.jianghongdianzi.cn

[Q63] 开启事务
来源：http://du.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://be.szsharing.cn

[Q64] 提交事务
来源：http://tb.newstarts.cn

COMMIT;
来源：http://wz.nicolike.cn

[Q65] 回滚事务
来源：http://qm.szsharing.cn

ROLLBACK;
来源：http://mq.newstarts.cn

[Q66] 行锁查询
来源：http://hc.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tk.szsharing.cn

[Q67] 设置隔离级别
来源：http://gr.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nf.panjiajie.cn

[Q68] 保存点
来源：http://mb.lnxyls.cn

SAVEPOINT sp1;
来源：http://oa.hnjuh.cn

ROLLBACK TO sp1;
来源：http://jd.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://xj.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pp.hnjuh.cn

[Q70] 更新统计信息
来源：http://qb.bjjhwx.cn

ANALYZE TABLE users;
来源：http://ms.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://tm.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qf.huixinmuqiang.cn

[Q72] 查看索引
来源：http://mc.9csxet.cn

SHOW INDEX FROM users;
来源：http://wu.521024.cn

[Q73] 查看表状态
来源：http://aw.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ue.shxzskj.cn

[Q74] 强制使用索引
来源：http://nr.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jo.hahajie.cn

[Q75] 日期格式化
来源：http://op.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dc.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cb.shtwfgs.cn

[Q76] 按天统计
来源：http://kb.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wp.shxzskj.cn

[Q77] 时间加减
来源：http://nk.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gq.hahajie.cn

[Q78] 当前时间
来源：http://ay.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jp.shxzskj.cn

[Q79] 字符串拼接
来源：http://wz.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gm.shtwfgs.cn

[Q80] 字符串截取
来源：http://cc.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hh.muxihuayi.cn

[Q81] 字符串替换
来源：http://jr.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sk.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://kk.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gk.shxzskj.cn

[Q83] 大小写转换
来源：http://jj.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ni.szxytkj.cn

[Q84] 去除首尾空格
来源：http://zf.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://jq.huixiangedu.cn

[Q85] 数值取整
来源：http://kw.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ad.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://dn.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sj.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://tu.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://om.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://mf.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xz.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jz.shxzskj.cn

[Q89] 判断表是否存在
来源：http://fy.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ro.panjiajie.cn

[Q90] 生成序号列
来源：http://ze.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://la.bjjhwx.cn

================================================================================
来源：http://tl.yuexingan06.cn

R. Bash 专题
来源：http://rg.hnjuh.cn

================================================================================
来源：http://xt.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://ug.yuexingan06.cn

#!/usr/bin/env bash
来源：http://rc.9csxet.cn

set -euo pipefail
来源：http://ok.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://nf.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://wn.newstarts.cn

[R03] 只读变量
来源：http://fz.asd995.cn

readonly PI=3.14
来源：http://ix.chemitech.net.cn

[R04] 位置参数
来源：http://io.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tn.asd995.cn

[R05] 参数默认值
来源：http://qc.yuexingan06.cn

name="${1:-default}"
来源：http://mt.asd995.cn

[R06] 判断命令是否存在
来源：http://rx.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qr.jctech888.com.cn

[R07] if 判断文件
来源：http://pt.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sd.muxihuayi.cn

[R08] 数值比较
来源：http://tv.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ir.muxihuayi.cn

[R09] 字符串比较
来源：http://qs.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qg.huixinmuqiang.cn

[R10] 正则匹配
来源：http://ve.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://my.huixiangedu.cn

[R11] case 多分支
来源：http://bz.jctech888.com.cn

case "$1" in
来源：http://ms.521024.cn

start) echo "启动" ;;
来源：http://tj.9csxet.cn

stop)  echo "停止" ;;
来源：http://mr.newstarts.cn

*)     echo "未知命令" ;;
来源：http://dd.bjjhwx.cn

esac
来源：http://eb.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://yw.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://ou.yuntaijiaju.cn

[R13] for 计数循环
来源：http://tp.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://kl.shtwfgs.cn

[R14] C 风格 for
来源：http://jb.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jw.chemitech.net.cn

[R15] while 逐行读文件
来源：http://mm.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ao.panjiajie.cn

[R16] until 等待条件
来源：http://jp.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ok.bjjhwx.cn

[R17] 数组定义与取值
来源：http://cc.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vd.hahajie.cn

[R18] 遍历数组
来源：http://jp.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hv.shtwfgs.cn

[R19] 数组长度
来源：http://tz.muxihuayi.cn

echo "${#arr[@]}"
来源：http://mt.szxytkj.cn

[R20] 关联数组（字典）
来源：http://nk.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ch.colortex.cn

[R21] 字符串长度
来源：http://ua.huixinmuqiang.cn

echo "${#s}"
来源：http://sr.bookmarksfly.cn

[R22] 截取子串
来源：http://or.asd995.cn

echo "${s:0:5}"
来源：http://cv.shxzskj.cn

[R23] 字符串替换
来源：http://sk.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wd.huixiangedu.cn

[R24] 大小写转换
来源：http://vv.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kp.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://wc.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ix.wgjwhj.cn

[R26] 命令替换
来源：http://vu.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://kl.521024.cn

[R27] 算术展开
来源：http://sm.9csxet.cn

echo $((1 + 2 * 3))
来源：http://ag.chemitech.net.cn

[R28] 浮点运算
来源：http://qy.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://me.hahajie.cn

[R29] 定义函数
来源：http://qa.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://me.shxzskj.cn

[R30] 函数返回状态码
来源：http://uo.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://fm.bookmarksfly.cn

[R31] 局部变量
来源：http://qz.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://la.huixiangedu.cn

[R32] 参数个数校验
来源：http://pl.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ig.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://ne.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oz.chemitech.net.cn

[R34] 退出时清理
来源：http://bk.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://im.panjiajie.cn

[R35] 后台执行并等待
来源：http://bq.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xz.colortex.cn

[R36] 并发执行多个任务
来源：http://lg.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ld.hnjuh.cn

[R37] 把输出赋给变量
来源：http://xg.huixiangedu.cn

files=$(ls -1)
来源：http://en.bookmarksfly.cn

[R38] 管道串联
来源：http://ic.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://cm.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://pn.chemitech.net.cn

cmd > out.log 2>&1
来源：http://xo.521024.cn

[R40] 追加写日志
来源：http://js.huanxung.cn

echo "log" >> out.log
来源：http://ax.chemitech.net.cn

[R41] 丢弃输出
来源：http://be.521024.cn

cmd >/dev/null 2>&1
来源：http://mi.szsharing.cn

[R42] 输入重定向
来源：http://be.bjjhwx.cn

wc -l < a.txt
来源：http://hn.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://ql.nszjky.cn

find . -name "*.log" -type f
来源：http://is.panjiajie.cn

[R44] 按修改时间查找
来源：http://fp.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://oe.shtwfgs.cn

[R45] 批量删除
来源：http://xe.colortex.cn

find . -name "*.tmp" -delete
来源：http://mr.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://uk.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zm.521024.cn

[R47] sed 单行替换
来源：http://bp.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://br.chemitech.net.cn

[R48] awk 取指定列
来源：http://kd.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://ja.bookmarksfly.cn

[R49] awk 带条件
来源：http://hv.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ki.shxzukj.cn

[R50] awk 求和
来源：http://zh.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mc.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://ss.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uo.521024.cn

[R52] 统计行数
来源：http://kf.newstarts.cn

wc -l a.txt
来源：http://qd.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://xi.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ar.huixiangedu.cn

[R54] 比较两个文件
来源：http://vj.colortex.cn

diff a.txt b.txt
来源：http://ny.yuexingan06.cn

[R55] 压缩与解压
来源：http://vf.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://we.newstarts.cn

[R56] 远程拷贝
来源：http://vd.muxihuayi.cn

scp file user@host:/path/
来源：http://xn.haigaiapp.cn

[R57] 远程执行命令
来源：http://hm.newstarts.cn

ssh user@host 'uptime'
来源：http://uk.shxzukj.cn

[R58] 下载文件
来源：http://ls.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cz.gzmigu.cn

[R59] 发 POST JSON
来源：http://ns.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wi.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://im.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://md.yuexingan06.cn

[R61] 磁盘占用
来源：http://ej.panjiajie.cn

df -h;  du -sh *
来源：http://ha.colortex.cn

[R62] 找最占空间的文件
来源：http://qz.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://ri.wgjwhj.cn

[R63] 内存与进程
来源：http://df.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://lp.hnjuh.cn

[R64] 结束进程
来源：http://pz.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://gb.colortex.cn

[R65] 查看端口占用
来源：http://zs.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://as.szxytkj.cn

[R66] 定时任务
来源：http://hg.muxihuayi.cn

crontab -e;  crontab -l
来源：http://jc.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://vx.newstarts.cn

openssl rand -hex 16
来源：http://ax.wgjwhj.cn

[R68] 计算文件校验值
来源：http://ng.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iu.9csxet.cn

[R69] 生成随机密码
来源：http://nf.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://io.nszjky.cn

[R70] 时间戳与互转
来源：http://yv.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://ji.colortex.cn

[R71] 日期格式化
来源：http://td.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oz.newstarts.cn

[R72] 等待端口就绪
来源：http://eo.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yw.huixiangedu.cn

[R73] 分割大日志
来源：http://pg.9csxet.cn

split -l 1000 big.log part_
来源：http://zh.szxytkj.cn

[R74] 批量重命名
来源：http://ac.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wy.shtwfgs.cn

[R75] 导出环境变量
来源：http://hx.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://zc.hnjuh.cn

[R76] 使用临时文件
来源：http://vw.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ef.szxytkj.cn

[R77] 读取用户输入
来源：http://yg.hnjuh.cn

read -rp "请输入: " ans
来源：http://bp.jctech888.com.cn

[R78] 交互式菜单
来源：http://xr.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hc.gzmigu.cn

[R79] 解析命令行选项
来源：http://gy.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oq.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://tx.bookmarksfly.cn

time ./run.sh
来源：http://tu.521024.cn

================================================================================
来源：http://gn.jctech888.com.cn

S. C / C++ 专题
来源：http://ln.muxihuayi.cn

================================================================================
来源：http://sg.bookmarksfly.cn

[S01] C：Hello World
来源：http://lt.yuexingan06.cn

#include <stdio.h>
来源：http://un.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zu.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://hp.521024.cn

int a = 10; printf("%d\n", a);
来源：http://mj.lnxyls.cn

[S03] C：读入整数
来源：http://tw.shxzukj.cn

int x; scanf("%d", &x);
来源：http://wg.huanxung.cn

[S04] C：字符串复制
来源：http://kf.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ls.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://aw.521024.cn

strlen(s)
来源：http://xs.newstarts.cn

[S06] C：字符串比较
来源：http://so.asd995.cn

strcmp(a, b) == 0
来源：http://xp.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://ci.nszjky.cn


<!-- 参考信息 -->