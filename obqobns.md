代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://fl.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pa.colortex.cn

[Q43] 标量子查询
来源：http://qj.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://or.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://cy.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vv.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://pb.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ap.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kq.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://de.yuexingan06.cn

[Q47] 与平均值比较
来源：http://yb.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bd.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://ya.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ga.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://le.nszjky.cn

[Q49] 更新单行
来源：http://il.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rl.chemitech.net.cn

[Q50] 批量更新
来源：http://do.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iq.szsharing.cn

[Q51] 用子查询更新
来源：http://we.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mp.lnxyls.cn

[Q52] 删除指定行
来源：http://kl.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://ib.nszjky.cn

[Q53] 按条件删除
来源：http://rv.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zu.shtwfgs.cn

[Q54] 清空表
来源：http://no.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://km.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://kq.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lb.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://ti.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cg.jctech888.com.cn

[Q57] 行号
来源：http://md.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://da.asd995.cn

[Q58] 累计求和
来源：http://gr.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://en.asd995.cn

[Q59] 分组内累计
来源：http://qq.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jv.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://pt.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pu.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mf.bookmarksfly.cn

[Q61] 移动平均
来源：http://wb.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qo.hahajie.cn

[Q62] 分组占比
来源：http://rx.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vf.newstarts.cn

[Q63] 开启事务
来源：http://lu.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ue.hahajie.cn

[Q64] 提交事务
来源：http://on.hahajie.cn

COMMIT;
来源：http://ud.panjiajie.cn

[Q65] 回滚事务
来源：http://el.haigaiapp.cn

ROLLBACK;
来源：http://rh.yuexingan06.cn

[Q66] 行锁查询
来源：http://nn.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://au.asd995.cn

[Q67] 设置隔离级别
来源：http://br.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vr.huixiangedu.cn

[Q68] 保存点
来源：http://bh.lnxyls.cn

SAVEPOINT sp1;
来源：http://po.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://ot.nszjky.cn

[Q69] 查看执行计划
来源：http://if.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ti.bjjhwx.cn

[Q70] 更新统计信息
来源：http://rk.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://oh.szsharing.cn

[Q71] 查看建表语句
来源：http://ey.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ji.jctech888.com.cn

[Q72] 查看索引
来源：http://qd.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://ul.gzmigu.cn

[Q73] 查看表状态
来源：http://mm.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xg.haigaiapp.cn

[Q74] 强制使用索引
来源：http://wy.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sc.gzmigu.cn

[Q75] 日期格式化
来源：http://ix.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://le.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ix.hnjuh.cn

[Q76] 按天统计
来源：http://mv.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://us.huixinmuqiang.cn

[Q77] 时间加减
来源：http://wc.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zo.chemitech.net.cn

[Q78] 当前时间
来源：http://bj.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ny.9csxet.cn

[Q79] 字符串拼接
来源：http://xg.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qv.newstarts.cn

[Q80] 字符串截取
来源：http://ds.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rp.nicolike.cn

[Q81] 字符串替换
来源：http://rx.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zi.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://ms.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://je.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://he.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mz.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://ee.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://my.yuexingan06.cn

[Q85] 数值取整
来源：http://nj.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mh.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://gh.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rn.521024.cn

[Q87] JSON 字段做条件
来源：http://ir.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ce.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://lr.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lj.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aq.szxytkj.cn

[Q89] 判断表是否存在
来源：http://fz.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zd.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://rs.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ax.521024.cn

================================================================================
来源：http://kq.huixinmuqiang.cn

R. Bash 专题
来源：http://vk.yuexingan06.cn

================================================================================
来源：http://ni.panjiajie.cn

[R01] shebang 与严格模式
来源：http://nz.bjjhwx.cn

#!/usr/bin/env bash
来源：http://tv.newstarts.cn

set -euo pipefail
来源：http://yv.9csxet.cn

[R02] 变量赋值与使用
来源：http://lo.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://pm.nicolike.cn

[R03] 只读变量
来源：http://hr.hahajie.cn

readonly PI=3.14
来源：http://py.nicolike.cn

[R04] 位置参数
来源：http://ca.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xc.asd995.cn

[R05] 参数默认值
来源：http://fr.hahajie.cn

name="${1:-default}"
来源：http://ry.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://by.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bf.yuntaijiaju.cn

[R07] if 判断文件
来源：http://qi.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://im.huixiangedu.cn

[R08] 数值比较
来源：http://hj.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cz.shxzukj.cn

[R09] 字符串比较
来源：http://bi.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yp.nicolike.cn

[R10] 正则匹配
来源：http://lm.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jj.yuntaijiaju.cn

[R11] case 多分支
来源：http://qt.nicolike.cn

case "$1" in
来源：http://eu.lnxyls.cn

start) echo "启动" ;;
来源：http://gm.newstarts.cn

stop)  echo "停止" ;;
来源：http://tc.nszjky.cn

*)     echo "未知命令" ;;
来源：http://dv.hnjuh.cn

esac
来源：http://ug.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://eb.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://bb.gzmigu.cn

[R13] for 计数循环
来源：http://oi.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://dx.521024.cn

[R14] C 风格 for
来源：http://uk.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rz.szsharing.cn

[R15] while 逐行读文件
来源：http://hn.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ww.szxytkj.cn

[R16] until 等待条件
来源：http://ae.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ll.haigaiapp.cn

[R17] 数组定义与取值
来源：http://ed.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ke.lnxyls.cn

[R18] 遍历数组
来源：http://vf.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ju.nszjky.cn

[R19] 数组长度
来源：http://ug.gzmigu.cn

echo "${#arr[@]}"
来源：http://ug.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://qk.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dp.muxihuayi.cn

[R21] 字符串长度
来源：http://mt.shxzskj.cn

echo "${#s}"
来源：http://pe.yuntaijiaju.cn

[R22] 截取子串
来源：http://qb.bookmarksfly.cn

echo "${s:0:5}"
来源：http://vq.bjjhwx.cn

[R23] 字符串替换
来源：http://qh.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wo.huanxung.cn

[R24] 大小写转换
来源：http://dq.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yt.521024.cn

[R25] 去后缀 / 去前缀
来源：http://bf.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://la.asd995.cn

[R26] 命令替换
来源：http://oz.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://ks.lnxyls.cn

[R27] 算术展开
来源：http://zg.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://gf.yuexingan06.cn

[R28] 浮点运算
来源：http://xl.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://js.hnjuh.cn

[R29] 定义函数
来源：http://en.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hl.bjjhwx.cn

[R30] 函数返回状态码
来源：http://gr.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://zu.gzmigu.cn

[R31] 局部变量
来源：http://ik.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://id.haigaiapp.cn

[R32] 参数个数校验
来源：http://qu.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rl.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://zx.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sf.9csxet.cn

[R34] 退出时清理
来源：http://wp.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ww.huanxung.cn

[R35] 后台执行并等待
来源：http://mf.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://we.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://nl.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pi.nszjky.cn

[R37] 把输出赋给变量
来源：http://tj.bookmarksfly.cn

files=$(ls -1)
来源：http://eb.hnjuh.cn

[R38] 管道串联
来源：http://kk.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://xi.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://ab.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://nc.gzmigu.cn

[R40] 追加写日志
来源：http://gs.nszjky.cn

echo "log" >> out.log
来源：http://mc.muxihuayi.cn

[R41] 丢弃输出
来源：http://hg.asd995.cn

cmd >/dev/null 2>&1
来源：http://zk.lnxyls.cn

[R42] 输入重定向
来源：http://mt.shtwfgs.cn

wc -l < a.txt
来源：http://dn.haigaiapp.cn

[R43] 按名字查找文件
来源：http://hy.wgjwhj.cn

find . -name "*.log" -type f
来源：http://vm.wgjwhj.cn

[R44] 按修改时间查找
来源：http://dn.shxzukj.cn

find . -mtime -7 -type f
来源：http://oi.huixinmuqiang.cn

[R45] 批量删除
来源：http://ns.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://fh.colortex.cn

[R46] 递归替换文件内容
来源：http://qh.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nd.gzmigu.cn

[R47] sed 单行替换
来源：http://oh.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jt.colortex.cn

[R48] awk 取指定列
来源：http://ix.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://gr.szxytkj.cn

[R49] awk 带条件
来源：http://mc.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tb.chemitech.net.cn

[R50] awk 求和
来源：http://ln.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fd.chemitech.net.cn

[R51] 排序去重取前几
来源：http://mx.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ay.huixinmuqiang.cn

[R52] 统计行数
来源：http://qv.lnxyls.cn

wc -l a.txt
来源：http://ga.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://ou.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ok.yuexingan06.cn

[R54] 比较两个文件
来源：http://xm.chemitech.net.cn

diff a.txt b.txt
来源：http://vt.huanxung.cn

[R55] 压缩与解压
来源：http://mk.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uc.nszjky.cn

[R56] 远程拷贝
来源：http://lh.lnxyls.cn

scp file user@host:/path/
来源：http://am.szxytkj.cn

[R57] 远程执行命令
来源：http://hg.nicolike.cn

ssh user@host 'uptime'
来源：http://mf.huixinmuqiang.cn

[R58] 下载文件
来源：http://ri.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://df.shxzskj.cn

[R59] 发 POST JSON
来源：http://ze.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ld.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://gz.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xj.newstarts.cn

[R61] 磁盘占用
来源：http://hd.newstarts.cn

df -h;  du -sh *
来源：http://xi.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://ti.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://kw.colortex.cn

[R63] 内存与进程
来源：http://nx.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://se.nicolike.cn

[R64] 结束进程
来源：http://wf.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://qz.hahajie.cn

[R65] 查看端口占用
来源：http://ni.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pz.wgjwhj.cn

[R66] 定时任务
来源：http://yd.hnjuh.cn

crontab -e;  crontab -l
来源：http://zc.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://xg.jianghongdianzi.cn

openssl rand -hex 16
来源：http://qm.szsharing.cn

[R68] 计算文件校验值
来源：http://tj.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vo.colortex.cn

[R69] 生成随机密码
来源：http://hk.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://fq.chemitech.net.cn

[R70] 时间戳与互转
来源：http://qx.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://pw.jctech888.com.cn

[R71] 日期格式化
来源：http://gh.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rj.chemitech.net.cn

[R72] 等待端口就绪
来源：http://xb.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eo.wgjwhj.cn

[R73] 分割大日志
来源：http://lf.hahajie.cn

split -l 1000 big.log part_
来源：http://xr.bjjhwx.cn

[R74] 批量重命名
来源：http://tv.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dg.newstarts.cn

[R75] 导出环境变量
来源：http://am.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://xt.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://qj.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nx.gzmigu.cn

[R77] 读取用户输入
来源：http://bd.hnjuh.cn

read -rp "请输入: " ans
来源：http://vu.nicolike.cn

[R78] 交互式菜单
来源：http://ti.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ql.521024.cn

[R79] 解析命令行选项
来源：http://ru.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xw.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://so.colortex.cn

time ./run.sh
来源：http://qm.jctech888.com.cn

================================================================================
来源：http://gb.lnxyls.cn

S. C / C++ 专题
来源：http://wv.huixiangedu.cn

================================================================================
来源：http://td.szxytkj.cn

[S01] C：Hello World
来源：http://cg.jianghongdianzi.cn

#include <stdio.h>
来源：http://bl.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qs.szsharing.cn

[S02] C：变量与格式化输出
来源：http://zs.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://us.asd995.cn

[S03] C：读入整数
来源：http://is.hnjuh.cn

int x; scanf("%d", &x);
来源：http://mw.gzmigu.cn

[S04] C：字符串复制
来源：http://pq.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rs.wgjwhj.cn

[S05] C：字符串长度
来源：http://mr.colortex.cn

strlen(s)
来源：http://lg.yuexingan06.cn

[S06] C：字符串比较
来源：http://iq.asd995.cn

strcmp(a, b) == 0
来源：http://zy.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://wq.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zj.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://zc.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eh.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://ak.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://of.asd995.cn

[S10] C：指针与解引用
来源：http://gi.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://ql.lnxyls.cn

[S11] C：逐行读文件
来源：http://dm.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://lg.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ni.szxytkj.cn

fclose(f);
来源：http://gn.szsharing.cn

[S12] C：写文件
来源：http://la.nszjky.cn


<!-- 参考信息 -->