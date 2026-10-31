代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://au.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zq.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://og.huixinmuqiang.cn

[Q41] 多表连接
来源：http://vl.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gm.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://bb.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://ga.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://gj.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://sn.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ek.huanxung.cn

[Q43] 标量子查询
来源：http://vi.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jt.chemitech.net.cn

[Q44] IN 子查询
来源：http://zs.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ld.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://vv.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dg.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fa.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hp.asd995.cn

[Q47] 与平均值比较
来源：http://ox.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://el.colortex.cn

[Q48] CTE 公用表表达式
来源：http://ze.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xb.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://te.521024.cn

[Q49] 更新单行
来源：http://ok.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gm.yuexingan06.cn

[Q50] 批量更新
来源：http://ot.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vh.521024.cn

[Q51] 用子查询更新
来源：http://so.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ac.9csxet.cn

[Q52] 删除指定行
来源：http://sj.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://le.9csxet.cn

[Q53] 按条件删除
来源：http://hk.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://di.hnjuh.cn

[Q54] 清空表
来源：http://bq.hahajie.cn

TRUNCATE TABLE logs;
来源：http://wu.newstarts.cn

[Q55] 排名（并列占位）
来源：http://hq.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bl.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://xl.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hn.szsharing.cn

[Q57] 行号
来源：http://zk.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ab.9csxet.cn

[Q58] 累计求和
来源：http://jm.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yh.yuexingan06.cn

[Q59] 分组内累计
来源：http://vo.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pr.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://gv.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qb.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bg.szxytkj.cn

[Q61] 移动平均
来源：http://zt.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://un.szsharing.cn

[Q62] 分组占比
来源：http://qu.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lx.9csxet.cn

[Q63] 开启事务
来源：http://rw.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ij.muxihuayi.cn

[Q64] 提交事务
来源：http://qx.shxzskj.cn

COMMIT;
来源：http://og.shtwfgs.cn

[Q65] 回滚事务
来源：http://vm.shxzskj.cn

ROLLBACK;
来源：http://vh.haigaiapp.cn

[Q66] 行锁查询
来源：http://hg.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rc.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://hr.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ir.hnjuh.cn

[Q68] 保存点
来源：http://jy.shtwfgs.cn

SAVEPOINT sp1;
来源：http://fc.gzmigu.cn

ROLLBACK TO sp1;
来源：http://vx.jctech888.com.cn

[Q69] 查看执行计划
来源：http://uh.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wq.panjiajie.cn

[Q70] 更新统计信息
来源：http://ta.newstarts.cn

ANALYZE TABLE users;
来源：http://ys.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://gv.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cm.lnxyls.cn

[Q72] 查看索引
来源：http://ef.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://qy.colortex.cn

[Q73] 查看表状态
来源：http://pp.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kl.jctech888.com.cn

[Q74] 强制使用索引
来源：http://fk.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ee.panjiajie.cn

[Q75] 日期格式化
来源：http://iw.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rs.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ap.panjiajie.cn

[Q76] 按天统计
来源：http://og.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oq.chemitech.net.cn

[Q77] 时间加减
来源：http://zg.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uu.hnjuh.cn

[Q78] 当前时间
来源：http://ec.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cl.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://rd.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zc.jctech888.com.cn

[Q80] 字符串截取
来源：http://fi.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uy.bookmarksfly.cn

[Q81] 字符串替换
来源：http://uo.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hk.521024.cn

[Q82] 字符长度与字节长度
来源：http://ys.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qz.nicolike.cn

[Q83] 大小写转换
来源：http://gw.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nd.hahajie.cn

[Q84] 去除首尾空格
来源：http://hb.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://tn.521024.cn

[Q85] 数值取整
来源：http://wi.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fg.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://ds.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xj.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://jr.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ue.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://zq.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dg.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ca.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://jf.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zb.szxytkj.cn

[Q90] 生成序号列
来源：http://vj.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cr.shxzukj.cn

================================================================================
来源：http://cr.huixiangedu.cn

R. Bash 专题
来源：http://ak.lnxyls.cn

================================================================================
来源：http://pl.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://rx.gzmigu.cn

#!/usr/bin/env bash
来源：http://oi.shtwfgs.cn

set -euo pipefail
来源：http://um.colortex.cn

[R02] 变量赋值与使用
来源：http://ii.hnjuh.cn

name="Tom"; echo "$name"
来源：http://qs.gzmigu.cn

[R03] 只读变量
来源：http://re.chemitech.net.cn

readonly PI=3.14
来源：http://ps.shxzskj.cn

[R04] 位置参数
来源：http://vz.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vi.shtwfgs.cn

[R05] 参数默认值
来源：http://ku.huanxung.cn

name="${1:-default}"
来源：http://wo.panjiajie.cn

[R06] 判断命令是否存在
来源：http://qi.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gf.panjiajie.cn

[R07] if 判断文件
来源：http://sx.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jy.huixiangedu.cn

[R08] 数值比较
来源：http://cu.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lt.shtwfgs.cn

[R09] 字符串比较
来源：http://aw.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cn.shxzukj.cn

[R10] 正则匹配
来源：http://wr.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ow.muxihuayi.cn

[R11] case 多分支
来源：http://dj.hahajie.cn

case "$1" in
来源：http://us.yuexingan06.cn

start) echo "启动" ;;
来源：http://no.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://zr.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://bp.panjiajie.cn

esac
来源：http://fp.bookmarksfly.cn

[R12] for 遍历文件
来源：http://ey.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://tp.huanxung.cn

[R13] for 计数循环
来源：http://vw.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://fh.wgjwhj.cn

[R14] C 风格 for
来源：http://hf.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ao.gzmigu.cn

[R15] while 逐行读文件
来源：http://vi.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vb.szsharing.cn

[R16] until 等待条件
来源：http://ma.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://um.bjjhwx.cn

[R17] 数组定义与取值
来源：http://pg.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lg.newstarts.cn

[R18] 遍历数组
来源：http://ya.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zl.nicolike.cn

[R19] 数组长度
来源：http://np.shxzukj.cn

echo "${#arr[@]}"
来源：http://sj.newstarts.cn

[R20] 关联数组（字典）
来源：http://gz.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bs.haigaiapp.cn

[R21] 字符串长度
来源：http://qc.huixinmuqiang.cn

echo "${#s}"
来源：http://vh.yuntaijiaju.cn

[R22] 截取子串
来源：http://mr.szxytkj.cn

echo "${s:0:5}"
来源：http://ks.bookmarksfly.cn

[R23] 字符串替换
来源：http://ir.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qs.bjjhwx.cn

[R24] 大小写转换
来源：http://mz.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ja.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://ms.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ur.nicolike.cn

[R26] 命令替换
来源：http://az.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://pi.9csxet.cn

[R27] 算术展开
来源：http://gj.colortex.cn

echo $((1 + 2 * 3))
来源：http://ch.chemitech.net.cn

[R28] 浮点运算
来源：http://mf.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://ih.shxzukj.cn

[R29] 定义函数
来源：http://up.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rq.bjjhwx.cn

[R30] 函数返回状态码
来源：http://mu.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://ch.hahajie.cn

[R31] 局部变量
来源：http://qo.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://vi.lnxyls.cn

[R32] 参数个数校验
来源：http://ad.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xt.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://xc.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jq.hnjuh.cn

[R34] 退出时清理
来源：http://fv.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ej.nicolike.cn

[R35] 后台执行并等待
来源：http://qw.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lm.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://tt.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gj.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://am.wgjwhj.cn

files=$(ls -1)
来源：http://cs.hahajie.cn

[R38] 管道串联
来源：http://ny.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://dz.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://vm.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://jy.shxzskj.cn

[R40] 追加写日志
来源：http://jk.yuexingan06.cn

echo "log" >> out.log
来源：http://gy.colortex.cn

[R41] 丢弃输出
来源：http://xt.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://gp.lnxyls.cn

[R42] 输入重定向
来源：http://ti.szsharing.cn

wc -l < a.txt
来源：http://il.asd995.cn

[R43] 按名字查找文件
来源：http://sv.colortex.cn

find . -name "*.log" -type f
来源：http://zk.newstarts.cn

[R44] 按修改时间查找
来源：http://tn.szsharing.cn

find . -mtime -7 -type f
来源：http://yt.szxytkj.cn

[R45] 批量删除
来源：http://ci.asd995.cn

find . -name "*.tmp" -delete
来源：http://dd.szxytkj.cn

[R46] 递归替换文件内容
来源：http://cq.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sv.panjiajie.cn

[R47] sed 单行替换
来源：http://cv.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ey.nicolike.cn

[R48] awk 取指定列
来源：http://tl.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://wj.yuexingan06.cn

[R49] awk 带条件
来源：http://pb.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nu.lnxyls.cn

[R50] awk 求和
来源：http://oy.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mj.muxihuayi.cn

[R51] 排序去重取前几
来源：http://me.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sv.huixinmuqiang.cn

[R52] 统计行数
来源：http://zr.szsharing.cn

wc -l a.txt
来源：http://du.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://rb.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qo.lnxyls.cn

[R54] 比较两个文件
来源：http://iw.huanxung.cn

diff a.txt b.txt
来源：http://eq.muxihuayi.cn

[R55] 压缩与解压
来源：http://tn.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cw.lnxyls.cn

[R56] 远程拷贝
来源：http://bn.521024.cn

scp file user@host:/path/
来源：http://lh.muxihuayi.cn

[R57] 远程执行命令
来源：http://ct.colortex.cn

ssh user@host 'uptime'
来源：http://wn.bookmarksfly.cn

[R58] 下载文件
来源：http://gc.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tq.nicolike.cn

[R59] 发 POST JSON
来源：http://sx.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bx.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://ja.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ms.panjiajie.cn

[R61] 磁盘占用
来源：http://au.nicolike.cn

df -h;  du -sh *
来源：http://qh.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://ke.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://xp.9csxet.cn

[R63] 内存与进程
来源：http://ec.asd995.cn

free -h;  ps aux | grep nginx
来源：http://jv.colortex.cn

[R64] 结束进程
来源：http://ww.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://jv.szsharing.cn

[R65] 查看端口占用
来源：http://ur.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ml.jianghongdianzi.cn

[R66] 定时任务
来源：http://fc.nicolike.cn

crontab -e;  crontab -l
来源：http://zh.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://qm.yuntaijiaju.cn

openssl rand -hex 16
来源：http://zg.panjiajie.cn

[R68] 计算文件校验值
来源：http://wj.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bw.muxihuayi.cn

[R69] 生成随机密码
来源：http://hd.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://cg.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://om.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://ak.yuexingan06.cn

[R71] 日期格式化
来源：http://jv.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yv.nszjky.cn

[R72] 等待端口就绪
来源：http://nk.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uw.yuexingan06.cn

[R73] 分割大日志
来源：http://ja.521024.cn

split -l 1000 big.log part_
来源：http://we.wgjwhj.cn

[R74] 批量重命名
来源：http://bh.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://be.chemitech.net.cn

[R75] 导出环境变量
来源：http://fa.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ik.bookmarksfly.cn

[R76] 使用临时文件
来源：http://xz.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mj.shxzskj.cn

[R77] 读取用户输入
来源：http://th.panjiajie.cn

read -rp "请输入: " ans
来源：http://ep.yuexingan06.cn

[R78] 交互式菜单
来源：http://mx.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pa.9csxet.cn

[R79] 解析命令行选项
来源：http://wy.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eo.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://mz.hahajie.cn

time ./run.sh
来源：http://yh.9csxet.cn

================================================================================
来源：http://pn.shtwfgs.cn

S. C / C++ 专题
来源：http://xh.haigaiapp.cn

================================================================================
来源：http://sw.chemitech.net.cn

[S01] C：Hello World
来源：http://wi.newstarts.cn

#include <stdio.h>
来源：http://qp.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ky.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://yu.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://or.521024.cn

[S03] C：读入整数
来源：http://ex.huanxung.cn

int x; scanf("%d", &x);
来源：http://cf.hnjuh.cn

[S04] C：字符串复制
来源：http://up.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ih.chemitech.net.cn

[S05] C：字符串长度
来源：http://jk.nszjky.cn

strlen(s)
来源：http://gh.shxzukj.cn

[S06] C：字符串比较
来源：http://cg.shxzukj.cn

strcmp(a, b) == 0
来源：http://eh.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://ow.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ov.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://vb.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://of.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://ba.panjiajie.cn


<!-- 参考信息 -->