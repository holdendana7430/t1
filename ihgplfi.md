代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jt.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ju.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uw.bjjhwx.cn

[Q41] 多表连接
来源：http://do.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yu.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://nk.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://qo.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://ft.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://kg.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ps.lnxyls.cn

[Q43] 标量子查询
来源：http://tz.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xa.nicolike.cn

[Q44] IN 子查询
来源：http://lj.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gf.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://tg.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tg.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ey.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tc.hahajie.cn

[Q47] 与平均值比较
来源：http://th.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://za.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://qr.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ip.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://lo.huanxung.cn

[Q49] 更新单行
来源：http://qu.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gt.shxzukj.cn

[Q50] 批量更新
来源：http://zj.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uw.gzmigu.cn

[Q51] 用子查询更新
来源：http://ps.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wb.gzmigu.cn

[Q52] 删除指定行
来源：http://wk.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://ru.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://yl.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://em.haigaiapp.cn

[Q54] 清空表
来源：http://xf.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://jx.521024.cn

[Q55] 排名（并列占位）
来源：http://yo.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xp.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://og.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yi.muxihuayi.cn

[Q57] 行号
来源：http://vq.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qh.nicolike.cn

[Q58] 累计求和
来源：http://pu.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ga.wgjwhj.cn

[Q59] 分组内累计
来源：http://pu.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rn.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://dn.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gm.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ml.9csxet.cn

[Q61] 移动平均
来源：http://uv.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ed.nicolike.cn

[Q62] 分组占比
来源：http://in.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://te.wgjwhj.cn

[Q63] 开启事务
来源：http://wf.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fa.szsharing.cn

[Q64] 提交事务
来源：http://af.nszjky.cn

COMMIT;
来源：http://nz.gzmigu.cn

[Q65] 回滚事务
来源：http://zr.wgjwhj.cn

ROLLBACK;
来源：http://be.nszjky.cn

[Q66] 行锁查询
来源：http://hk.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rm.lnxyls.cn

[Q67] 设置隔离级别
来源：http://gi.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ex.9csxet.cn

[Q68] 保存点
来源：http://xe.shtwfgs.cn

SAVEPOINT sp1;
来源：http://hx.shxzukj.cn

ROLLBACK TO sp1;
来源：http://zd.colortex.cn

[Q69] 查看执行计划
来源：http://ck.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rn.yuexingan06.cn

[Q70] 更新统计信息
来源：http://zx.nicolike.cn

ANALYZE TABLE users;
来源：http://up.nicolike.cn

[Q71] 查看建表语句
来源：http://lw.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zy.shxzskj.cn

[Q72] 查看索引
来源：http://ua.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://zl.huanxung.cn

[Q73] 查看表状态
来源：http://wb.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ay.521024.cn

[Q74] 强制使用索引
来源：http://en.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pv.huixiangedu.cn

[Q75] 日期格式化
来源：http://vd.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jx.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yq.colortex.cn

[Q76] 按天统计
来源：http://nc.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cp.hahajie.cn

[Q77] 时间加减
来源：http://em.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jg.szxytkj.cn

[Q78] 当前时间
来源：http://va.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vs.yuexingan06.cn

[Q79] 字符串拼接
来源：http://bl.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fn.huixiangedu.cn

[Q80] 字符串截取
来源：http://qa.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hg.hnjuh.cn

[Q81] 字符串替换
来源：http://yp.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ef.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://ee.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yi.colortex.cn

[Q83] 大小写转换
来源：http://vl.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ep.panjiajie.cn

[Q84] 去除首尾空格
来源：http://az.521024.cn

SELECT TRIM(name) FROM users;
来源：http://yq.colortex.cn

[Q85] 数值取整
来源：http://sa.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nq.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://vx.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rq.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://uw.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qi.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://aw.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kj.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://su.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://ou.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pd.hnjuh.cn

[Q90] 生成序号列
来源：http://qz.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wv.hnjuh.cn

================================================================================
来源：http://ta.hahajie.cn

R. Bash 专题
来源：http://dv.lnxyls.cn

================================================================================
来源：http://qs.szsharing.cn

[R01] shebang 与严格模式
来源：http://xc.shxzukj.cn

#!/usr/bin/env bash
来源：http://cg.bookmarksfly.cn

set -euo pipefail
来源：http://or.shxzukj.cn

[R02] 变量赋值与使用
来源：http://ry.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://cl.gzmigu.cn

[R03] 只读变量
来源：http://mc.nszjky.cn

readonly PI=3.14
来源：http://nu.bjjhwx.cn

[R04] 位置参数
来源：http://xi.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ng.muxihuayi.cn

[R05] 参数默认值
来源：http://bk.nszjky.cn

name="${1:-default}"
来源：http://tb.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://ko.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zg.yuexingan06.cn

[R07] if 判断文件
来源：http://hk.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hn.newstarts.cn

[R08] 数值比较
来源：http://lt.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xq.panjiajie.cn

[R09] 字符串比较
来源：http://du.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jy.newstarts.cn

[R10] 正则匹配
来源：http://eo.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hg.hahajie.cn

[R11] case 多分支
来源：http://ye.newstarts.cn

case "$1" in
来源：http://vi.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://nt.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://hq.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://uh.huixiangedu.cn

esac
来源：http://kj.gzmigu.cn

[R12] for 遍历文件
来源：http://qv.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://px.yuexingan06.cn

[R13] for 计数循环
来源：http://xp.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://zx.asd995.cn

[R14] C 风格 for
来源：http://xf.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xx.gzmigu.cn

[R15] while 逐行读文件
来源：http://lb.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fs.lnxyls.cn

[R16] until 等待条件
来源：http://mn.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bi.nicolike.cn

[R17] 数组定义与取值
来源：http://ic.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uo.shxzukj.cn

[R18] 遍历数组
来源：http://ev.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://do.hahajie.cn

[R19] 数组长度
来源：http://fj.hahajie.cn

echo "${#arr[@]}"
来源：http://rq.521024.cn

[R20] 关联数组（字典）
来源：http://mw.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tv.szsharing.cn

[R21] 字符串长度
来源：http://jx.muxihuayi.cn

echo "${#s}"
来源：http://yt.chemitech.net.cn

[R22] 截取子串
来源：http://ln.lnxyls.cn

echo "${s:0:5}"
来源：http://ku.nicolike.cn

[R23] 字符串替换
来源：http://qs.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xa.bookmarksfly.cn

[R24] 大小写转换
来源：http://jx.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ii.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://hb.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://by.huixinmuqiang.cn

[R26] 命令替换
来源：http://wn.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://vt.jctech888.com.cn

[R27] 算术展开
来源：http://pp.521024.cn

echo $((1 + 2 * 3))
来源：http://jf.huixiangedu.cn

[R28] 浮点运算
来源：http://uu.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://wa.huixinmuqiang.cn

[R29] 定义函数
来源：http://eh.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kc.bjjhwx.cn

[R30] 函数返回状态码
来源：http://nj.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://az.asd995.cn

[R31] 局部变量
来源：http://ow.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://pa.lnxyls.cn

[R32] 参数个数校验
来源：http://ft.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fr.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://kz.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fo.asd995.cn

[R34] 退出时清理
来源：http://qv.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bc.shxzukj.cn

[R35] 后台执行并等待
来源：http://mw.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ah.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://jc.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bw.huanxung.cn

[R37] 把输出赋给变量
来源：http://zj.gzmigu.cn

files=$(ls -1)
来源：http://fn.521024.cn

[R38] 管道串联
来源：http://gm.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://co.asd995.cn

[R39] 重定向标准输出与错误
来源：http://ok.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://tt.szsharing.cn

[R40] 追加写日志
来源：http://qh.nszjky.cn

echo "log" >> out.log
来源：http://bb.szsharing.cn

[R41] 丢弃输出
来源：http://bu.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://wq.wgjwhj.cn

[R42] 输入重定向
来源：http://ow.shxzskj.cn

wc -l < a.txt
来源：http://rh.bjjhwx.cn

[R43] 按名字查找文件
来源：http://vo.jctech888.com.cn

find . -name "*.log" -type f
来源：http://bk.9csxet.cn

[R44] 按修改时间查找
来源：http://yt.newstarts.cn

find . -mtime -7 -type f
来源：http://fy.hahajie.cn

[R45] 批量删除
来源：http://zx.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://lm.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://ea.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ue.nszjky.cn

[R47] sed 单行替换
来源：http://lx.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gy.yuexingan06.cn

[R48] awk 取指定列
来源：http://ph.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://gz.yuexingan06.cn

[R49] awk 带条件
来源：http://yh.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://it.wgjwhj.cn

[R50] awk 求和
来源：http://at.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ut.gzmigu.cn

[R51] 排序去重取前几
来源：http://rt.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wg.yuexingan06.cn

[R52] 统计行数
来源：http://wb.shxzskj.cn

wc -l a.txt
来源：http://sk.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://zu.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ia.nszjky.cn

[R54] 比较两个文件
来源：http://yr.panjiajie.cn

diff a.txt b.txt
来源：http://jn.yuexingan06.cn

[R55] 压缩与解压
来源：http://fa.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://br.yuexingan06.cn

[R56] 远程拷贝
来源：http://ck.huixiangedu.cn

scp file user@host:/path/
来源：http://hz.huanxung.cn

[R57] 远程执行命令
来源：http://nu.chemitech.net.cn

ssh user@host 'uptime'
来源：http://pq.chemitech.net.cn

[R58] 下载文件
来源：http://eh.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vw.shxzskj.cn

[R59] 发 POST JSON
来源：http://bg.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bx.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://nj.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://or.chemitech.net.cn

[R61] 磁盘占用
来源：http://qd.nicolike.cn

df -h;  du -sh *
来源：http://co.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://op.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://dl.hnjuh.cn

[R63] 内存与进程
来源：http://ch.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://bx.shtwfgs.cn

[R64] 结束进程
来源：http://kg.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://kb.szxytkj.cn

[R65] 查看端口占用
来源：http://gk.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fw.huanxung.cn

[R66] 定时任务
来源：http://rb.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://nw.9csxet.cn

[R67] 生成随机十六进制串
来源：http://ta.shxzukj.cn

openssl rand -hex 16
来源：http://qm.nicolike.cn

[R68] 计算文件校验值
来源：http://gs.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pg.shxzukj.cn

[R69] 生成随机密码
来源：http://ok.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://oh.lnxyls.cn

[R70] 时间戳与互转
来源：http://kz.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://dq.521024.cn

[R71] 日期格式化
来源：http://am.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nm.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://mj.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vq.chemitech.net.cn

[R73] 分割大日志
来源：http://ma.szsharing.cn

split -l 1000 big.log part_
来源：http://wj.hahajie.cn

[R74] 批量重命名
来源：http://qw.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ge.yuexingan06.cn

[R75] 导出环境变量
来源：http://gv.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://hv.9csxet.cn

[R76] 使用临时文件
来源：http://iu.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sc.yuexingan06.cn

[R77] 读取用户输入
来源：http://sq.hahajie.cn

read -rp "请输入: " ans
来源：http://vq.muxihuayi.cn

[R78] 交互式菜单
来源：http://sz.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://no.shtwfgs.cn

[R79] 解析命令行选项
来源：http://qb.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vv.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://cl.szsharing.cn

time ./run.sh
来源：http://go.haigaiapp.cn

================================================================================
来源：http://wx.panjiajie.cn

S. C / C++ 专题
来源：http://og.bjjhwx.cn

================================================================================
来源：http://us.nicolike.cn

[S01] C：Hello World
来源：http://ex.colortex.cn

#include <stdio.h>
来源：http://de.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://km.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://fh.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://gk.panjiajie.cn

[S03] C：读入整数
来源：http://jk.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://kc.haigaiapp.cn

[S04] C：字符串复制
来源：http://yp.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ar.shxzskj.cn

[S05] C：字符串长度
来源：http://on.hahajie.cn

strlen(s)
来源：http://yp.panjiajie.cn

[S06] C：字符串比较
来源：http://fl.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://dv.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://nh.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ki.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://gk.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://di.asd995.cn

[S09] C：结构体定义与初始化
来源：http://pv.szsharing.cn


<!-- 参考信息 -->