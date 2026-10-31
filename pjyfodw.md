代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://as.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://yi.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://rg.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://op.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://zp.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kf.bjjhwx.cn

[Q43] 标量子查询
来源：http://vb.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ao.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://dz.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oz.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://ee.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eb.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mg.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pr.colortex.cn

[Q47] 与平均值比较
来源：http://uk.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rb.colortex.cn

[Q48] CTE 公用表表达式
来源：http://zw.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://po.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://mm.newstarts.cn

[Q49] 更新单行
来源：http://pa.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vo.lnxyls.cn

[Q50] 批量更新
来源：http://ci.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eo.bjjhwx.cn

[Q51] 用子查询更新
来源：http://hv.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uf.chemitech.net.cn

[Q52] 删除指定行
来源：http://pl.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://sp.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://xy.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sw.bjjhwx.cn

[Q54] 清空表
来源：http://zp.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://qs.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://yg.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tr.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://ov.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wv.nicolike.cn

[Q57] 行号
来源：http://qj.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dm.wgjwhj.cn

[Q58] 累计求和
来源：http://xe.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lj.newstarts.cn

[Q59] 分组内累计
来源：http://dr.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uj.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://po.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fi.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mp.huanxung.cn

[Q61] 移动平均
来源：http://er.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ye.colortex.cn

[Q62] 分组占比
来源：http://ab.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ba.asd995.cn

[Q63] 开启事务
来源：http://xq.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rt.bookmarksfly.cn

[Q64] 提交事务
来源：http://hj.jianghongdianzi.cn

COMMIT;
来源：http://fv.bjjhwx.cn

[Q65] 回滚事务
来源：http://bm.lnxyls.cn

ROLLBACK;
来源：http://sg.9csxet.cn

[Q66] 行锁查询
来源：http://bs.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vm.gzmigu.cn

[Q67] 设置隔离级别
来源：http://ag.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ae.chemitech.net.cn

[Q68] 保存点
来源：http://qf.yuexingan06.cn

SAVEPOINT sp1;
来源：http://gs.hnjuh.cn

ROLLBACK TO sp1;
来源：http://ui.asd995.cn

[Q69] 查看执行计划
来源：http://dv.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rf.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://zx.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://kn.nszjky.cn

[Q71] 查看建表语句
来源：http://of.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jl.nicolike.cn

[Q72] 查看索引
来源：http://fh.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://fw.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://au.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xo.colortex.cn

[Q74] 强制使用索引
来源：http://hk.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ur.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://ys.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ee.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xz.nszjky.cn

[Q76] 按天统计
来源：http://nm.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rg.colortex.cn

[Q77] 时间加减
来源：http://fd.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ay.shtwfgs.cn

[Q78] 当前时间
来源：http://cx.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tr.newstarts.cn

[Q79] 字符串拼接
来源：http://wd.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aa.huixiangedu.cn

[Q80] 字符串截取
来源：http://hz.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wb.bjjhwx.cn

[Q81] 字符串替换
来源：http://mb.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yg.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://hg.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zs.shxzskj.cn

[Q83] 大小写转换
来源：http://xh.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://md.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://zp.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://js.huixiangedu.cn

[Q85] 数值取整
来源：http://kb.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://je.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://au.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gv.9csxet.cn

[Q87] JSON 字段做条件
来源：http://br.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sg.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://gc.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yt.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ml.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://or.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nv.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://af.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zn.shxzskj.cn

================================================================================
来源：http://ab.nicolike.cn

R. Bash 专题
来源：http://lp.chemitech.net.cn

================================================================================
来源：http://tb.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://zy.nszjky.cn

#!/usr/bin/env bash
来源：http://ai.shxzskj.cn

set -euo pipefail
来源：http://vf.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://au.9csxet.cn

name="Tom"; echo "$name"
来源：http://oi.chemitech.net.cn

[R03] 只读变量
来源：http://jf.yuntaijiaju.cn

readonly PI=3.14
来源：http://cp.huixiangedu.cn

[R04] 位置参数
来源：http://ui.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cd.asd995.cn

[R05] 参数默认值
来源：http://xv.hahajie.cn

name="${1:-default}"
来源：http://ji.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://hw.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ex.haigaiapp.cn

[R07] if 判断文件
来源：http://dq.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ru.hnjuh.cn

[R08] 数值比较
来源：http://fb.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cc.gzmigu.cn

[R09] 字符串比较
来源：http://vb.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xw.wgjwhj.cn

[R10] 正则匹配
来源：http://jm.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sd.huanxung.cn

[R11] case 多分支
来源：http://lu.colortex.cn

case "$1" in
来源：http://jb.bjjhwx.cn

start) echo "启动" ;;
来源：http://kl.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://ps.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://wi.lnxyls.cn

esac
来源：http://fw.bjjhwx.cn

[R12] for 遍历文件
来源：http://my.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://ln.szsharing.cn

[R13] for 计数循环
来源：http://xl.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://zo.wgjwhj.cn

[R14] C 风格 for
来源：http://oq.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gi.chemitech.net.cn

[R15] while 逐行读文件
来源：http://bv.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ya.szxytkj.cn

[R16] until 等待条件
来源：http://nc.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vy.bjjhwx.cn

[R17] 数组定义与取值
来源：http://fs.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vm.yuexingan06.cn

[R18] 遍历数组
来源：http://hh.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yb.asd995.cn

[R19] 数组长度
来源：http://if.wgjwhj.cn

echo "${#arr[@]}"
来源：http://ln.hnjuh.cn

[R20] 关联数组（字典）
来源：http://qc.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eg.newstarts.cn

[R21] 字符串长度
来源：http://wi.newstarts.cn

echo "${#s}"
来源：http://hz.szxytkj.cn

[R22] 截取子串
来源：http://gi.haigaiapp.cn

echo "${s:0:5}"
来源：http://sc.colortex.cn

[R23] 字符串替换
来源：http://ab.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uq.szxytkj.cn

[R24] 大小写转换
来源：http://on.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wl.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://pg.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uv.gzmigu.cn

[R26] 命令替换
来源：http://ww.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://lg.yuexingan06.cn

[R27] 算术展开
来源：http://ot.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://rx.lnxyls.cn

[R28] 浮点运算
来源：http://uu.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://nv.muxihuayi.cn

[R29] 定义函数
来源：http://nx.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ud.szsharing.cn

[R30] 函数返回状态码
来源：http://mb.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://xm.muxihuayi.cn

[R31] 局部变量
来源：http://oi.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://vt.521024.cn

[R32] 参数个数校验
来源：http://qw.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zu.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://fw.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zn.haigaiapp.cn

[R34] 退出时清理
来源：http://mn.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gf.gzmigu.cn

[R35] 后台执行并等待
来源：http://vz.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gc.nicolike.cn

[R36] 并发执行多个任务
来源：http://rg.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lf.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://pb.chemitech.net.cn

files=$(ls -1)
来源：http://yf.nicolike.cn

[R38] 管道串联
来源：http://ec.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://pr.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://qz.haigaiapp.cn

cmd > out.log 2>&1
来源：http://ah.jianghongdianzi.cn

[R40] 追加写日志
来源：http://wc.jctech888.com.cn

echo "log" >> out.log
来源：http://sn.szsharing.cn

[R41] 丢弃输出
来源：http://kj.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://wl.yuntaijiaju.cn

[R42] 输入重定向
来源：http://fh.panjiajie.cn

wc -l < a.txt
来源：http://ce.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://gf.chemitech.net.cn

find . -name "*.log" -type f
来源：http://av.szxytkj.cn

[R44] 按修改时间查找
来源：http://bb.huixiangedu.cn

find . -mtime -7 -type f
来源：http://aw.521024.cn

[R45] 批量删除
来源：http://ro.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://nr.9csxet.cn

[R46] 递归替换文件内容
来源：http://jj.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ql.lnxyls.cn

[R47] sed 单行替换
来源：http://pc.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ns.jctech888.com.cn

[R48] awk 取指定列
来源：http://od.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://mp.shxzskj.cn

[R49] awk 带条件
来源：http://aa.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cz.hnjuh.cn

[R50] awk 求和
来源：http://yk.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://he.colortex.cn

[R51] 排序去重取前几
来源：http://lq.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://to.haigaiapp.cn

[R52] 统计行数
来源：http://cx.shtwfgs.cn

wc -l a.txt
来源：http://vk.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://rv.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vm.hnjuh.cn

[R54] 比较两个文件
来源：http://pw.yuexingan06.cn

diff a.txt b.txt
来源：http://ei.shtwfgs.cn

[R55] 压缩与解压
来源：http://bp.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://km.hnjuh.cn

[R56] 远程拷贝
来源：http://ze.shxzskj.cn

scp file user@host:/path/
来源：http://xg.lnxyls.cn

[R57] 远程执行命令
来源：http://un.9csxet.cn

ssh user@host 'uptime'
来源：http://uv.szxytkj.cn

[R58] 下载文件
来源：http://fn.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fr.shxzukj.cn

[R59] 发 POST JSON
来源：http://iq.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fo.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://fr.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nj.nszjky.cn

[R61] 磁盘占用
来源：http://jg.shtwfgs.cn

df -h;  du -sh *
来源：http://nb.hnjuh.cn

[R62] 找最占空间的文件
来源：http://qd.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://gi.nicolike.cn

[R63] 内存与进程
来源：http://ug.521024.cn

free -h;  ps aux | grep nginx
来源：http://nk.9csxet.cn

[R64] 结束进程
来源：http://rb.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://fg.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://nl.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hw.9csxet.cn

[R66] 定时任务
来源：http://nk.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://dl.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://yt.shxzskj.cn

openssl rand -hex 16
来源：http://yd.shxzskj.cn

[R68] 计算文件校验值
来源：http://ts.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wv.gzmigu.cn

[R69] 生成随机密码
来源：http://ko.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://th.chemitech.net.cn

[R70] 时间戳与互转
来源：http://cg.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://js.nszjky.cn

[R71] 日期格式化
来源：http://wg.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://in.jctech888.com.cn

[R72] 等待端口就绪
来源：http://aj.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jc.hnjuh.cn

[R73] 分割大日志
来源：http://uj.panjiajie.cn

split -l 1000 big.log part_
来源：http://qu.bjjhwx.cn

[R74] 批量重命名
来源：http://ot.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qv.shxzukj.cn

[R75] 导出环境变量
来源：http://xo.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://xg.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://pw.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ri.shtwfgs.cn

[R77] 读取用户输入
来源：http://hr.shxzukj.cn

read -rp "请输入: " ans
来源：http://qo.shtwfgs.cn

[R78] 交互式菜单
来源：http://mn.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cy.newstarts.cn

[R79] 解析命令行选项
来源：http://xy.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bt.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://us.asd995.cn

time ./run.sh
来源：http://hk.hahajie.cn

================================================================================
来源：http://xa.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ph.huanxung.cn

================================================================================
来源：http://hp.shxzskj.cn

[S01] C：Hello World
来源：http://fx.newstarts.cn

#include <stdio.h>
来源：http://bs.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pb.asd995.cn

[S02] C：变量与格式化输出
来源：http://nn.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://op.haigaiapp.cn

[S03] C：读入整数
来源：http://lo.szxytkj.cn

int x; scanf("%d", &x);
来源：http://pa.bookmarksfly.cn

[S04] C：字符串复制
来源：http://je.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xp.9csxet.cn

[S05] C：字符串长度
来源：http://bp.wgjwhj.cn

strlen(s)
来源：http://os.asd995.cn

[S06] C：字符串比较
来源：http://if.jctech888.com.cn

strcmp(a, b) == 0
来源：http://ee.asd995.cn

[S07] C：数组遍历求和
来源：http://oj.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://at.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://zy.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dh.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://nh.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tv.newstarts.cn

[S10] C：指针与解引用
来源：http://ox.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ax.9csxet.cn

[S11] C：逐行读文件
来源：http://uu.9csxet.cn


<!-- 参考信息 -->