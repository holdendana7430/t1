代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://uq.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xj.nszjky.cn

[Q43] 标量子查询
来源：http://nb.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tt.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://cc.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nv.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://wi.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zi.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oi.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qa.gzmigu.cn

[Q47] 与平均值比较
来源：http://mz.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tq.521024.cn

[Q48] CTE 公用表表达式
来源：http://zs.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tb.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://cr.shxzukj.cn

[Q49] 更新单行
来源：http://sn.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dl.huixiangedu.cn

[Q50] 批量更新
来源：http://az.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://in.gzmigu.cn

[Q51] 用子查询更新
来源：http://jv.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sd.nszjky.cn

[Q52] 删除指定行
来源：http://mf.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://kv.wgjwhj.cn

[Q53] 按条件删除
来源：http://qq.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kw.yuexingan06.cn

[Q54] 清空表
来源：http://kw.nicolike.cn

TRUNCATE TABLE logs;
来源：http://tj.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://qf.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tm.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://ro.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://um.yuntaijiaju.cn

[Q57] 行号
来源：http://ab.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ct.haigaiapp.cn

[Q58] 累计求和
来源：http://zu.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sk.hnjuh.cn

[Q59] 分组内累计
来源：http://bs.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vz.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://gq.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rl.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ny.colortex.cn

[Q61] 移动平均
来源：http://og.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xk.shxzskj.cn

[Q62] 分组占比
来源：http://gz.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gg.huanxung.cn

[Q63] 开启事务
来源：http://nu.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pv.huanxung.cn

[Q64] 提交事务
来源：http://gt.colortex.cn

COMMIT;
来源：http://ff.jctech888.com.cn

[Q65] 回滚事务
来源：http://xy.huixinmuqiang.cn

ROLLBACK;
来源：http://aj.hnjuh.cn

[Q66] 行锁查询
来源：http://jg.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ge.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://ee.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iw.newstarts.cn

[Q68] 保存点
来源：http://uo.hnjuh.cn

SAVEPOINT sp1;
来源：http://dt.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://pf.gzmigu.cn

[Q69] 查看执行计划
来源：http://ph.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rb.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://tz.shxzukj.cn

ANALYZE TABLE users;
来源：http://pp.hnjuh.cn

[Q71] 查看建表语句
来源：http://wn.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://df.nicolike.cn

[Q72] 查看索引
来源：http://xv.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://fq.newstarts.cn

[Q73] 查看表状态
来源：http://ty.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ha.szsharing.cn

[Q74] 强制使用索引
来源：http://jk.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rs.hahajie.cn

[Q75] 日期格式化
来源：http://hq.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bp.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nl.szsharing.cn

[Q76] 按天统计
来源：http://ru.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yp.szsharing.cn

[Q77] 时间加减
来源：http://zc.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vm.shxzskj.cn

[Q78] 当前时间
来源：http://qk.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wu.huixiangedu.cn

[Q79] 字符串拼接
来源：http://ur.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://to.lnxyls.cn

[Q80] 字符串截取
来源：http://tn.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://du.colortex.cn

[Q81] 字符串替换
来源：http://qa.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iu.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://vo.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qx.shxzskj.cn

[Q83] 大小写转换
来源：http://fm.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oi.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://du.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://jo.szxytkj.cn

[Q85] 数值取整
来源：http://kx.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yh.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://ob.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vy.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://ka.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bw.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://sc.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bt.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mq.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://sr.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rd.huixiangedu.cn

[Q90] 生成序号列
来源：http://xg.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mu.colortex.cn

================================================================================
来源：http://ee.muxihuayi.cn

R. Bash 专题
来源：http://kc.shxzukj.cn

================================================================================
来源：http://zc.huanxung.cn

[R01] shebang 与严格模式
来源：http://sb.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://ia.panjiajie.cn

set -euo pipefail
来源：http://of.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://wn.gzmigu.cn

name="Tom"; echo "$name"
来源：http://nq.huixiangedu.cn

[R03] 只读变量
来源：http://uh.nszjky.cn

readonly PI=3.14
来源：http://qw.jctech888.com.cn

[R04] 位置参数
来源：http://vh.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jg.shxzukj.cn

[R05] 参数默认值
来源：http://nd.gzmigu.cn

name="${1:-default}"
来源：http://tv.9csxet.cn

[R06] 判断命令是否存在
来源：http://hd.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ql.jctech888.com.cn

[R07] if 判断文件
来源：http://qy.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qc.shtwfgs.cn

[R08] 数值比较
来源：http://ij.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mu.newstarts.cn

[R09] 字符串比较
来源：http://bs.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dv.nszjky.cn

[R10] 正则匹配
来源：http://zo.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jq.jianghongdianzi.cn

[R11] case 多分支
来源：http://wc.huixiangedu.cn

case "$1" in
来源：http://zd.9csxet.cn

start) echo "启动" ;;
来源：http://hx.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://ne.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://pa.bjjhwx.cn

esac
来源：http://em.huanxung.cn

[R12] for 遍历文件
来源：http://ea.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://if.9csxet.cn

[R13] for 计数循环
来源：http://uj.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://yb.hnjuh.cn

[R14] C 风格 for
来源：http://an.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tu.shxzskj.cn

[R15] while 逐行读文件
来源：http://km.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wo.bjjhwx.cn

[R16] until 等待条件
来源：http://at.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tf.shxzskj.cn

[R17] 数组定义与取值
来源：http://ip.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gx.hnjuh.cn

[R18] 遍历数组
来源：http://jn.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sx.bookmarksfly.cn

[R19] 数组长度
来源：http://hq.nicolike.cn

echo "${#arr[@]}"
来源：http://va.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://pt.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kx.panjiajie.cn

[R21] 字符串长度
来源：http://wm.huixinmuqiang.cn

echo "${#s}"
来源：http://pa.nszjky.cn

[R22] 截取子串
来源：http://pk.panjiajie.cn

echo "${s:0:5}"
来源：http://ry.wgjwhj.cn

[R23] 字符串替换
来源：http://di.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://db.panjiajie.cn

[R24] 大小写转换
来源：http://fb.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qg.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://pf.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zp.wgjwhj.cn

[R26] 命令替换
来源：http://zt.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://wv.gzmigu.cn

[R27] 算术展开
来源：http://vt.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://vi.colortex.cn

[R28] 浮点运算
来源：http://dl.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://cb.muxihuayi.cn

[R29] 定义函数
来源：http://nz.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hw.panjiajie.cn

[R30] 函数返回状态码
来源：http://kh.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ab.bjjhwx.cn

[R31] 局部变量
来源：http://it.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://zt.gzmigu.cn

[R32] 参数个数校验
来源：http://qu.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dt.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://su.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ws.huixinmuqiang.cn

[R34] 退出时清理
来源：http://km.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ox.huanxung.cn

[R35] 后台执行并等待
来源：http://sn.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://js.asd995.cn

[R36] 并发执行多个任务
来源：http://tc.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hi.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://ga.jianghongdianzi.cn

files=$(ls -1)
来源：http://gm.jianghongdianzi.cn

[R38] 管道串联
来源：http://yq.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://ia.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://mm.muxihuayi.cn

cmd > out.log 2>&1
来源：http://cl.huixinmuqiang.cn

[R40] 追加写日志
来源：http://ex.asd995.cn

echo "log" >> out.log
来源：http://xz.9csxet.cn

[R41] 丢弃输出
来源：http://zp.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://dm.huanxung.cn

[R42] 输入重定向
来源：http://bn.yuexingan06.cn

wc -l < a.txt
来源：http://ht.shxzskj.cn

[R43] 按名字查找文件
来源：http://xr.panjiajie.cn

find . -name "*.log" -type f
来源：http://ha.asd995.cn

[R44] 按修改时间查找
来源：http://yu.lnxyls.cn

find . -mtime -7 -type f
来源：http://ub.huixiangedu.cn

[R45] 批量删除
来源：http://mo.9csxet.cn

find . -name "*.tmp" -delete
来源：http://dm.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://tq.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://go.shxzskj.cn

[R47] sed 单行替换
来源：http://qi.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vn.521024.cn

[R48] awk 取指定列
来源：http://kk.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://wp.szxytkj.cn

[R49] awk 带条件
来源：http://dx.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://md.yuntaijiaju.cn

[R50] awk 求和
来源：http://uv.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gx.huixiangedu.cn

[R51] 排序去重取前几
来源：http://cs.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jx.nicolike.cn

[R52] 统计行数
来源：http://pm.chemitech.net.cn

wc -l a.txt
来源：http://fp.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://df.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kq.lnxyls.cn

[R54] 比较两个文件
来源：http://rr.szsharing.cn

diff a.txt b.txt
来源：http://es.bookmarksfly.cn

[R55] 压缩与解压
来源：http://gr.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rc.muxihuayi.cn

[R56] 远程拷贝
来源：http://cx.nszjky.cn

scp file user@host:/path/
来源：http://lh.szsharing.cn

[R57] 远程执行命令
来源：http://rx.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ee.chemitech.net.cn

[R58] 下载文件
来源：http://vt.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://th.yuexingan06.cn

[R59] 发 POST JSON
来源：http://no.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ej.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://hf.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bu.colortex.cn

[R61] 磁盘占用
来源：http://vq.shxzukj.cn

df -h;  du -sh *
来源：http://xg.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://in.521024.cn

du -ah . | sort -rh | head -10
来源：http://ar.521024.cn

[R63] 内存与进程
来源：http://zg.colortex.cn

free -h;  ps aux | grep nginx
来源：http://pd.hahajie.cn

[R64] 结束进程
来源：http://ck.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://cx.muxihuayi.cn

[R65] 查看端口占用
来源：http://wo.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ut.9csxet.cn

[R66] 定时任务
来源：http://vg.wgjwhj.cn

crontab -e;  crontab -l
来源：http://fo.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://wc.asd995.cn

openssl rand -hex 16
来源：http://iy.yuexingan06.cn

[R68] 计算文件校验值
来源：http://ds.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pa.shtwfgs.cn

[R69] 生成随机密码
来源：http://ui.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://ps.shxzskj.cn

[R70] 时间戳与互转
来源：http://jh.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://jy.hahajie.cn

[R71] 日期格式化
来源：http://hx.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ek.szxytkj.cn

[R72] 等待端口就绪
来源：http://hk.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://en.bjjhwx.cn

[R73] 分割大日志
来源：http://wq.gzmigu.cn

split -l 1000 big.log part_
来源：http://rk.huanxung.cn

[R74] 批量重命名
来源：http://lj.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fl.hahajie.cn

[R75] 导出环境变量
来源：http://yv.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://ub.szsharing.cn

[R76] 使用临时文件
来源：http://rp.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ny.huanxung.cn

[R77] 读取用户输入
来源：http://qp.shtwfgs.cn

read -rp "请输入: " ans
来源：http://we.521024.cn

[R78] 交互式菜单
来源：http://kj.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ek.521024.cn

[R79] 解析命令行选项
来源：http://ul.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nl.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://wu.huixinmuqiang.cn

time ./run.sh
来源：http://ed.lnxyls.cn

================================================================================
来源：http://ba.shtwfgs.cn

S. C / C++ 专题
来源：http://qt.yuntaijiaju.cn

================================================================================
来源：http://lm.newstarts.cn

[S01] C：Hello World
来源：http://fo.hahajie.cn

#include <stdio.h>
来源：http://yk.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qo.hahajie.cn

[S02] C：变量与格式化输出
来源：http://fl.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://dl.jctech888.com.cn

[S03] C：读入整数
来源：http://em.asd995.cn

int x; scanf("%d", &x);
来源：http://ib.bookmarksfly.cn

[S04] C：字符串复制
来源：http://zy.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gd.asd995.cn

[S05] C：字符串长度
来源：http://ld.521024.cn

strlen(s)
来源：http://fj.haigaiapp.cn

[S06] C：字符串比较
来源：http://xs.wgjwhj.cn

strcmp(a, b) == 0
来源：http://ml.colortex.cn

[S07] C：数组遍历求和
来源：http://da.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ba.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://ci.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kr.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://yp.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gp.yuexingan06.cn

[S10] C：指针与解引用
来源：http://fr.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://qg.muxihuayi.cn

[S11] C：逐行读文件
来源：http://is.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://cs.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gk.yuexingan06.cn

fclose(f);
来源：http://ll.huixiangedu.cn

[S12] C：写文件
来源：http://oq.jianghongdianzi.cn


<!-- 参考信息 -->