代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://ms.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ry.panjiajie.cn

[Q43] 标量子查询
来源：http://qd.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bp.yuexingan06.cn

[Q44] IN 子查询
来源：http://pd.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jg.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://mv.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vb.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pe.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lw.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://us.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ty.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://nn.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fq.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://av.newstarts.cn

[Q49] 更新单行
来源：http://cm.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kt.lnxyls.cn

[Q50] 批量更新
来源：http://fu.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://si.yuexingan06.cn

[Q51] 用子查询更新
来源：http://tj.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yu.huixiangedu.cn

[Q52] 删除指定行
来源：http://oa.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://jf.nicolike.cn

[Q53] 按条件删除
来源：http://hn.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sc.szxytkj.cn

[Q54] 清空表
来源：http://nw.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://zu.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://dr.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ym.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://mo.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jh.huixinmuqiang.cn

[Q57] 行号
来源：http://js.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://it.newstarts.cn

[Q58] 累计求和
来源：http://bw.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xf.chemitech.net.cn

[Q59] 分组内累计
来源：http://wu.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bk.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://kg.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pg.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jx.muxihuayi.cn

[Q61] 移动平均
来源：http://ps.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nr.nicolike.cn

[Q62] 分组占比
来源：http://cm.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ln.panjiajie.cn

[Q63] 开启事务
来源：http://cz.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ba.huixiangedu.cn

[Q64] 提交事务
来源：http://qv.huanxung.cn

COMMIT;
来源：http://ap.colortex.cn

[Q65] 回滚事务
来源：http://qk.szsharing.cn

ROLLBACK;
来源：http://ck.jctech888.com.cn

[Q66] 行锁查询
来源：http://ny.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ky.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://aw.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pc.yuexingan06.cn

[Q68] 保存点
来源：http://lk.lnxyls.cn

SAVEPOINT sp1;
来源：http://id.lnxyls.cn

ROLLBACK TO sp1;
来源：http://dh.chemitech.net.cn

[Q69] 查看执行计划
来源：http://kb.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xf.nszjky.cn

[Q70] 更新统计信息
来源：http://ww.bjjhwx.cn

ANALYZE TABLE users;
来源：http://tr.gzmigu.cn

[Q71] 查看建表语句
来源：http://fw.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mw.bjjhwx.cn

[Q72] 查看索引
来源：http://xt.shxzukj.cn

SHOW INDEX FROM users;
来源：http://um.lnxyls.cn

[Q73] 查看表状态
来源：http://iu.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ez.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://aa.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://su.yuexingan06.cn

[Q75] 日期格式化
来源：http://va.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cg.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wf.yuntaijiaju.cn

[Q76] 按天统计
来源：http://gi.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uy.bjjhwx.cn

[Q77] 时间加减
来源：http://tg.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://go.newstarts.cn

[Q78] 当前时间
来源：http://so.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tw.nszjky.cn

[Q79] 字符串拼接
来源：http://sg.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bo.asd995.cn

[Q80] 字符串截取
来源：http://gt.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cd.521024.cn

[Q81] 字符串替换
来源：http://ie.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hp.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://px.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xv.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://po.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gl.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://wg.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://fg.huixiangedu.cn

[Q85] 数值取整
来源：http://nf.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wm.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://ts.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ez.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://kb.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sa.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://mm.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://is.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ty.shxzskj.cn

[Q89] 判断表是否存在
来源：http://zv.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zi.panjiajie.cn

[Q90] 生成序号列
来源：http://fe.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cb.9csxet.cn

================================================================================
来源：http://wz.jctech888.com.cn

R. Bash 专题
来源：http://jn.panjiajie.cn

================================================================================
来源：http://xu.nicolike.cn

[R01] shebang 与严格模式
来源：http://eq.hahajie.cn

#!/usr/bin/env bash
来源：http://in.colortex.cn

set -euo pipefail
来源：http://cx.shxzskj.cn

[R02] 变量赋值与使用
来源：http://fe.9csxet.cn

name="Tom"; echo "$name"
来源：http://bk.huanxung.cn

[R03] 只读变量
来源：http://jk.bookmarksfly.cn

readonly PI=3.14
来源：http://ph.huixinmuqiang.cn

[R04] 位置参数
来源：http://nk.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kr.colortex.cn

[R05] 参数默认值
来源：http://hd.jctech888.com.cn

name="${1:-default}"
来源：http://pt.newstarts.cn

[R06] 判断命令是否存在
来源：http://qb.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zd.nicolike.cn

[R07] if 判断文件
来源：http://gm.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dn.szsharing.cn

[R08] 数值比较
来源：http://gx.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sr.haigaiapp.cn

[R09] 字符串比较
来源：http://fu.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ou.bookmarksfly.cn

[R10] 正则匹配
来源：http://ud.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pt.gzmigu.cn

[R11] case 多分支
来源：http://bi.shxzskj.cn

case "$1" in
来源：http://cn.bjjhwx.cn

start) echo "启动" ;;
来源：http://eq.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://vs.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://qd.huixiangedu.cn

esac
来源：http://ff.newstarts.cn

[R12] for 遍历文件
来源：http://ta.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://uh.9csxet.cn

[R13] for 计数循环
来源：http://xr.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://bm.szxytkj.cn

[R14] C 风格 for
来源：http://ww.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qf.hnjuh.cn

[R15] while 逐行读文件
来源：http://bf.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rx.hahajie.cn

[R16] until 等待条件
来源：http://ts.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zl.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://qt.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mk.jianghongdianzi.cn

[R18] 遍历数组
来源：http://er.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wo.jianghongdianzi.cn

[R19] 数组长度
来源：http://ni.wgjwhj.cn

echo "${#arr[@]}"
来源：http://ak.521024.cn

[R20] 关联数组（字典）
来源：http://js.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xu.bjjhwx.cn

[R21] 字符串长度
来源：http://kq.jianghongdianzi.cn

echo "${#s}"
来源：http://cv.nicolike.cn

[R22] 截取子串
来源：http://yg.wgjwhj.cn

echo "${s:0:5}"
来源：http://kf.szxytkj.cn

[R23] 字符串替换
来源：http://no.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bb.bjjhwx.cn

[R24] 大小写转换
来源：http://yu.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gf.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://mh.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hv.bjjhwx.cn

[R26] 命令替换
来源：http://yj.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://yi.asd995.cn

[R27] 算术展开
来源：http://tp.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://di.bjjhwx.cn

[R28] 浮点运算
来源：http://ax.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://wv.hnjuh.cn

[R29] 定义函数
来源：http://by.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xh.newstarts.cn

[R30] 函数返回状态码
来源：http://gx.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://he.shxzukj.cn

[R31] 局部变量
来源：http://pb.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://qy.szxytkj.cn

[R32] 参数个数校验
来源：http://rn.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yd.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://qw.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://um.gzmigu.cn

[R34] 退出时清理
来源：http://jq.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://so.nicolike.cn

[R35] 后台执行并等待
来源：http://pd.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pc.shxzukj.cn

[R36] 并发执行多个任务
来源：http://by.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qf.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://ar.shxzskj.cn

files=$(ls -1)
来源：http://cn.haigaiapp.cn

[R38] 管道串联
来源：http://kc.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://pu.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://lp.shtwfgs.cn

cmd > out.log 2>&1
来源：http://re.huanxung.cn

[R40] 追加写日志
来源：http://hs.yuntaijiaju.cn

echo "log" >> out.log
来源：http://dp.szsharing.cn

[R41] 丢弃输出
来源：http://ya.9csxet.cn

cmd >/dev/null 2>&1
来源：http://nl.haigaiapp.cn

[R42] 输入重定向
来源：http://me.shtwfgs.cn

wc -l < a.txt
来源：http://fl.gzmigu.cn

[R43] 按名字查找文件
来源：http://su.yuexingan06.cn

find . -name "*.log" -type f
来源：http://ij.gzmigu.cn

[R44] 按修改时间查找
来源：http://vo.nszjky.cn

find . -mtime -7 -type f
来源：http://zv.yuexingan06.cn

[R45] 批量删除
来源：http://kk.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://ds.hahajie.cn

[R46] 递归替换文件内容
来源：http://co.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://is.szxytkj.cn

[R47] sed 单行替换
来源：http://rt.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hw.jctech888.com.cn

[R48] awk 取指定列
来源：http://zn.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://em.gzmigu.cn

[R49] awk 带条件
来源：http://vw.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://li.haigaiapp.cn

[R50] awk 求和
来源：http://wa.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://az.lnxyls.cn

[R51] 排序去重取前几
来源：http://pw.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://el.szxytkj.cn

[R52] 统计行数
来源：http://jy.hahajie.cn

wc -l a.txt
来源：http://xx.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://xg.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aq.colortex.cn

[R54] 比较两个文件
来源：http://ok.muxihuayi.cn

diff a.txt b.txt
来源：http://yo.panjiajie.cn

[R55] 压缩与解压
来源：http://iq.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pe.bjjhwx.cn

[R56] 远程拷贝
来源：http://ul.bjjhwx.cn

scp file user@host:/path/
来源：http://hp.hahajie.cn

[R57] 远程执行命令
来源：http://tw.9csxet.cn

ssh user@host 'uptime'
来源：http://vb.nszjky.cn

[R58] 下载文件
来源：http://wz.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qo.szsharing.cn

[R59] 发 POST JSON
来源：http://ce.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ax.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://yv.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ds.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://ld.panjiajie.cn

df -h;  du -sh *
来源：http://rx.lnxyls.cn

[R62] 找最占空间的文件
来源：http://qh.colortex.cn

du -ah . | sort -rh | head -10
来源：http://cm.jianghongdianzi.cn

[R63] 内存与进程
来源：http://wo.colortex.cn

free -h;  ps aux | grep nginx
来源：http://rn.szxytkj.cn

[R64] 结束进程
来源：http://ql.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://zh.chemitech.net.cn

[R65] 查看端口占用
来源：http://vg.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pz.bjjhwx.cn

[R66] 定时任务
来源：http://bh.nszjky.cn

crontab -e;  crontab -l
来源：http://pz.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://wl.shxzskj.cn

openssl rand -hex 16
来源：http://vp.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://bo.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mk.shtwfgs.cn

[R69] 生成随机密码
来源：http://df.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://da.521024.cn

[R70] 时间戳与互转
来源：http://fd.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://kw.yuntaijiaju.cn

[R71] 日期格式化
来源：http://uk.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://om.wgjwhj.cn

[R72] 等待端口就绪
来源：http://xn.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ae.yuntaijiaju.cn

[R73] 分割大日志
来源：http://pt.521024.cn

split -l 1000 big.log part_
来源：http://kf.bjjhwx.cn

[R74] 批量重命名
来源：http://tx.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qy.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://od.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://fq.shxzskj.cn

[R76] 使用临时文件
来源：http://gs.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nf.huixiangedu.cn

[R77] 读取用户输入
来源：http://tl.colortex.cn

read -rp "请输入: " ans
来源：http://vv.colortex.cn

[R78] 交互式菜单
来源：http://uk.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ks.newstarts.cn

[R79] 解析命令行选项
来源：http://mv.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ff.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://ge.nicolike.cn

time ./run.sh
来源：http://xe.haigaiapp.cn

================================================================================
来源：http://po.haigaiapp.cn

S. C / C++ 专题
来源：http://vy.huixinmuqiang.cn

================================================================================
来源：http://ow.szxytkj.cn

[S01] C：Hello World
来源：http://td.chemitech.net.cn

#include <stdio.h>
来源：http://dr.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lg.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://lx.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://px.szxytkj.cn

[S03] C：读入整数
来源：http://xf.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://pn.wgjwhj.cn

[S04] C：字符串复制
来源：http://lc.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ou.nszjky.cn

[S05] C：字符串长度
来源：http://pj.bookmarksfly.cn

strlen(s)
来源：http://zk.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://ce.yuexingan06.cn

strcmp(a, b) == 0
来源：http://ng.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://or.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://va.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://tv.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://um.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://mc.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ur.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://az.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://di.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://xo.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://vx.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fh.huixiangedu.cn

fclose(f);
来源：http://hg.panjiajie.cn

[S12] C：写文件
来源：http://or.jianghongdianzi.cn


<!-- 参考信息 -->