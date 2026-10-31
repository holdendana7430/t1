代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://ak.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://br.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://tt.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://da.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://kz.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://on.huixiangedu.cn

[Q43] 标量子查询
来源：http://ga.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ju.colortex.cn

[Q44] IN 子查询
来源：http://sa.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kq.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://en.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sr.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mq.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cc.muxihuayi.cn

[Q47] 与平均值比较
来源：http://kp.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xk.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://rt.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rj.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://iu.huixinmuqiang.cn

[Q49] 更新单行
来源：http://nn.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fr.shtwfgs.cn

[Q50] 批量更新
来源：http://qs.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://la.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://nx.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fz.szsharing.cn

[Q52] 删除指定行
来源：http://xe.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://tj.shtwfgs.cn

[Q53] 按条件删除
来源：http://ra.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lo.newstarts.cn

[Q54] 清空表
来源：http://jh.nicolike.cn

TRUNCATE TABLE logs;
来源：http://si.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://vg.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fh.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://yt.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tb.nszjky.cn

[Q57] 行号
来源：http://fa.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zx.wgjwhj.cn

[Q58] 累计求和
来源：http://qs.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yb.bookmarksfly.cn

[Q59] 分组内累计
来源：http://ky.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wp.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://tm.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sz.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pn.nszjky.cn

[Q61] 移动平均
来源：http://nr.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vl.shxzskj.cn

[Q62] 分组占比
来源：http://hv.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fz.9csxet.cn

[Q63] 开启事务
来源：http://zg.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://aw.jianghongdianzi.cn

[Q64] 提交事务
来源：http://uy.yuntaijiaju.cn

COMMIT;
来源：http://zd.521024.cn

[Q65] 回滚事务
来源：http://cc.yuexingan06.cn

ROLLBACK;
来源：http://oc.shtwfgs.cn

[Q66] 行锁查询
来源：http://ge.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://if.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://jh.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bp.shxzskj.cn

[Q68] 保存点
来源：http://dn.hnjuh.cn

SAVEPOINT sp1;
来源：http://hq.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://dg.jctech888.com.cn

[Q69] 查看执行计划
来源：http://uy.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kn.shtwfgs.cn

[Q70] 更新统计信息
来源：http://xq.chemitech.net.cn

ANALYZE TABLE users;
来源：http://iu.newstarts.cn

[Q71] 查看建表语句
来源：http://ck.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://es.yuexingan06.cn

[Q72] 查看索引
来源：http://jt.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://zv.shxzskj.cn

[Q73] 查看表状态
来源：http://sm.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xd.nszjky.cn

[Q74] 强制使用索引
来源：http://pa.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dr.521024.cn

[Q75] 日期格式化
来源：http://kr.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vo.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nz.haigaiapp.cn

[Q76] 按天统计
来源：http://kb.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://we.lnxyls.cn

[Q77] 时间加减
来源：http://tq.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yd.hahajie.cn

[Q78] 当前时间
来源：http://lc.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bg.bjjhwx.cn

[Q79] 字符串拼接
来源：http://uq.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mi.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://yj.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dn.yuexingan06.cn

[Q81] 字符串替换
来源：http://dz.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zp.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://cq.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fd.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://bp.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sd.hnjuh.cn

[Q84] 去除首尾空格
来源：http://fv.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://tm.panjiajie.cn

[Q85] 数值取整
来源：http://tm.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iq.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://kf.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yp.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://yp.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mv.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://ja.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rz.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cx.huanxung.cn

[Q89] 判断表是否存在
来源：http://gs.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xq.asd995.cn

[Q90] 生成序号列
来源：http://sk.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jo.chemitech.net.cn

================================================================================
来源：http://nt.hnjuh.cn

R. Bash 专题
来源：http://eg.wgjwhj.cn

================================================================================
来源：http://vn.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://qy.huanxung.cn

#!/usr/bin/env bash
来源：http://nb.huanxung.cn

set -euo pipefail
来源：http://yo.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://uo.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://qw.hahajie.cn

[R03] 只读变量
来源：http://de.nszjky.cn

readonly PI=3.14
来源：http://is.9csxet.cn

[R04] 位置参数
来源：http://bi.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://am.asd995.cn

[R05] 参数默认值
来源：http://hb.wgjwhj.cn

name="${1:-default}"
来源：http://qn.nicolike.cn

[R06] 判断命令是否存在
来源：http://vn.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vl.hahajie.cn

[R07] if 判断文件
来源：http://er.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eb.panjiajie.cn

[R08] 数值比较
来源：http://ng.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zy.yuntaijiaju.cn

[R09] 字符串比较
来源：http://gc.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zb.jctech888.com.cn

[R10] 正则匹配
来源：http://tu.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yc.nicolike.cn

[R11] case 多分支
来源：http://vn.bookmarksfly.cn

case "$1" in
来源：http://jb.yuexingan06.cn

start) echo "启动" ;;
来源：http://sc.hahajie.cn

stop)  echo "停止" ;;
来源：http://wn.9csxet.cn

*)     echo "未知命令" ;;
来源：http://bp.haigaiapp.cn

esac
来源：http://ov.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://lh.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://ce.hahajie.cn

[R13] for 计数循环
来源：http://hc.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ae.521024.cn

[R14] C 风格 for
来源：http://uj.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ye.szxytkj.cn

[R15] while 逐行读文件
来源：http://uc.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://by.lnxyls.cn

[R16] until 等待条件
来源：http://tn.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yk.nicolike.cn

[R17] 数组定义与取值
来源：http://wv.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hahajie.cn

[R18] 遍历数组
来源：http://sl.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ak.bookmarksfly.cn

[R19] 数组长度
来源：http://fh.nszjky.cn

echo "${#arr[@]}"
来源：http://lb.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://wm.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nb.szsharing.cn

[R21] 字符串长度
来源：http://nm.shxzukj.cn

echo "${#s}"
来源：http://ky.yuntaijiaju.cn

[R22] 截取子串
来源：http://qu.chemitech.net.cn

echo "${s:0:5}"
来源：http://iu.9csxet.cn

[R23] 字符串替换
来源：http://ed.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rf.jctech888.com.cn

[R24] 大小写转换
来源：http://yb.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ax.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://yz.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zg.521024.cn

[R26] 命令替换
来源：http://fl.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://px.colortex.cn

[R27] 算术展开
来源：http://pd.nicolike.cn

echo $((1 + 2 * 3))
来源：http://fs.lnxyls.cn

[R28] 浮点运算
来源：http://rj.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://tp.shtwfgs.cn

[R29] 定义函数
来源：http://un.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://po.szxytkj.cn

[R30] 函数返回状态码
来源：http://vs.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://bm.colortex.cn

[R31] 局部变量
来源：http://ca.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://na.shtwfgs.cn

[R32] 参数个数校验
来源：http://kf.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ee.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://bj.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fh.newstarts.cn

[R34] 退出时清理
来源：http://qu.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zv.jctech888.com.cn

[R35] 后台执行并等待
来源：http://ra.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://me.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://xn.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vj.shxzukj.cn

[R37] 把输出赋给变量
来源：http://mg.nicolike.cn

files=$(ls -1)
来源：http://zd.panjiajie.cn

[R38] 管道串联
来源：http://ko.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://ff.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://uw.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://nq.yuexingan06.cn

[R40] 追加写日志
来源：http://gd.colortex.cn

echo "log" >> out.log
来源：http://wr.shxzukj.cn

[R41] 丢弃输出
来源：http://jf.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://fd.szxytkj.cn

[R42] 输入重定向
来源：http://il.huixiangedu.cn

wc -l < a.txt
来源：http://gw.colortex.cn

[R43] 按名字查找文件
来源：http://tz.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://sj.shtwfgs.cn

[R44] 按修改时间查找
来源：http://ts.panjiajie.cn

find . -mtime -7 -type f
来源：http://zu.newstarts.cn

[R45] 批量删除
来源：http://ol.huanxung.cn

find . -name "*.tmp" -delete
来源：http://ly.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://iw.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dd.nszjky.cn

[R47] sed 单行替换
来源：http://bs.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dc.shxzukj.cn

[R48] awk 取指定列
来源：http://ff.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://ce.huanxung.cn

[R49] awk 带条件
来源：http://yy.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uf.hahajie.cn

[R50] awk 求和
来源：http://bp.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qi.lnxyls.cn

[R51] 排序去重取前几
来源：http://uw.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hh.chemitech.net.cn

[R52] 统计行数
来源：http://zs.huanxung.cn

wc -l a.txt
来源：http://kp.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://yj.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qv.szsharing.cn

[R54] 比较两个文件
来源：http://zt.521024.cn

diff a.txt b.txt
来源：http://kv.shtwfgs.cn

[R55] 压缩与解压
来源：http://io.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yp.asd995.cn

[R56] 远程拷贝
来源：http://mv.newstarts.cn

scp file user@host:/path/
来源：http://va.bookmarksfly.cn

[R57] 远程执行命令
来源：http://ak.gzmigu.cn

ssh user@host 'uptime'
来源：http://fu.hahajie.cn

[R58] 下载文件
来源：http://kl.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oq.chemitech.net.cn

[R59] 发 POST JSON
来源：http://xy.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ei.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://ud.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ol.szxytkj.cn

[R61] 磁盘占用
来源：http://ri.haigaiapp.cn

df -h;  du -sh *
来源：http://xv.nszjky.cn

[R62] 找最占空间的文件
来源：http://nu.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://ab.shxzukj.cn

[R63] 内存与进程
来源：http://tk.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://jv.nszjky.cn

[R64] 结束进程
来源：http://ds.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://co.hnjuh.cn

[R65] 查看端口占用
来源：http://wb.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ty.521024.cn

[R66] 定时任务
来源：http://jm.chemitech.net.cn

crontab -e;  crontab -l
来源：http://ab.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://xo.bjjhwx.cn

openssl rand -hex 16
来源：http://em.9csxet.cn

[R68] 计算文件校验值
来源：http://kr.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nt.hahajie.cn

[R69] 生成随机密码
来源：http://ca.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://yt.szxytkj.cn

[R70] 时间戳与互转
来源：http://zz.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://fl.lnxyls.cn

[R71] 日期格式化
来源：http://lk.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://es.521024.cn

[R72] 等待端口就绪
来源：http://pn.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eu.panjiajie.cn

[R73] 分割大日志
来源：http://hn.muxihuayi.cn

split -l 1000 big.log part_
来源：http://iv.jctech888.com.cn

[R74] 批量重命名
来源：http://wa.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tb.shxzukj.cn

[R75] 导出环境变量
来源：http://hk.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://pl.521024.cn

[R76] 使用临时文件
来源：http://fb.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ii.shxzukj.cn

[R77] 读取用户输入
来源：http://la.muxihuayi.cn

read -rp "请输入: " ans
来源：http://hp.yuexingan06.cn

[R78] 交互式菜单
来源：http://jv.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://my.huixiangedu.cn

[R79] 解析命令行选项
来源：http://cl.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dj.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://fz.hnjuh.cn

time ./run.sh
来源：http://ww.huixinmuqiang.cn

================================================================================
来源：http://pz.yuexingan06.cn

S. C / C++ 专题
来源：http://gb.colortex.cn

================================================================================
来源：http://xk.muxihuayi.cn

[S01] C：Hello World
来源：http://bu.jianghongdianzi.cn

#include <stdio.h>
来源：http://pk.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://na.colortex.cn

[S02] C：变量与格式化输出
来源：http://xs.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://tj.jctech888.com.cn

[S03] C：读入整数
来源：http://bb.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://yc.hnjuh.cn

[S04] C：字符串复制
来源：http://zh.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ya.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://pp.lnxyls.cn

strlen(s)
来源：http://et.521024.cn

[S06] C：字符串比较
来源：http://qu.nicolike.cn

strcmp(a, b) == 0
来源：http://sn.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://wj.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rd.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ed.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hh.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://xr.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vg.huixiangedu.cn

[S10] C：指针与解引用
来源：http://hs.colortex.cn

int *p = &a;  *p = 5;
来源：http://df.panjiajie.cn

[S11] C：逐行读文件
来源：http://it.szxytkj.cn


<!-- 参考信息 -->