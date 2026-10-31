代发 wailian999

[Q44] IN 子查询
来源：http://xn.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ku.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://kk.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nl.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fj.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qz.bjjhwx.cn

[Q47] 与平均值比较
来源：http://up.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ut.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://kp.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cr.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://dp.muxihuayi.cn

[Q49] 更新单行
来源：http://gs.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dq.huanxung.cn

[Q50] 批量更新
来源：http://de.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bu.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://vf.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kt.asd995.cn

[Q52] 删除指定行
来源：http://qe.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://hh.hnjuh.cn

[Q53] 按条件删除
来源：http://gw.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rn.newstarts.cn

[Q54] 清空表
来源：http://ri.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://mp.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://wk.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ju.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://ez.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vd.yuntaijiaju.cn

[Q57] 行号
来源：http://ut.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ja.huixinmuqiang.cn

[Q58] 累计求和
来源：http://sf.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wl.nszjky.cn

[Q59] 分组内累计
来源：http://iw.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wy.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://vv.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yo.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ac.bookmarksfly.cn

[Q61] 移动平均
来源：http://dw.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://np.huixiangedu.cn

[Q62] 分组占比
来源：http://zd.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dc.bookmarksfly.cn

[Q63] 开启事务
来源：http://pt.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uh.gzmigu.cn

[Q64] 提交事务
来源：http://nq.colortex.cn

COMMIT;
来源：http://zq.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://ss.hahajie.cn

ROLLBACK;
来源：http://rz.colortex.cn

[Q66] 行锁查询
来源：http://qq.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pa.szxytkj.cn

[Q67] 设置隔离级别
来源：http://oi.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bc.yuexingan06.cn

[Q68] 保存点
来源：http://xc.nicolike.cn

SAVEPOINT sp1;
来源：http://di.shxzskj.cn

ROLLBACK TO sp1;
来源：http://el.shtwfgs.cn

[Q69] 查看执行计划
来源：http://zn.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hf.wgjwhj.cn

[Q70] 更新统计信息
来源：http://mw.wgjwhj.cn

ANALYZE TABLE users;
来源：http://ff.wgjwhj.cn

[Q71] 查看建表语句
来源：http://sz.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://la.nszjky.cn

[Q72] 查看索引
来源：http://uu.hahajie.cn

SHOW INDEX FROM users;
来源：http://gs.shtwfgs.cn

[Q73] 查看表状态
来源：http://lv.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cy.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://ql.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uw.9csxet.cn

[Q75] 日期格式化
来源：http://zj.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ao.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://og.asd995.cn

[Q76] 按天统计
来源：http://bt.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mm.huixiangedu.cn

[Q77] 时间加减
来源：http://as.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qr.szxytkj.cn

[Q78] 当前时间
来源：http://bn.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ou.nicolike.cn

[Q79] 字符串拼接
来源：http://fx.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xv.szsharing.cn

[Q80] 字符串截取
来源：http://hs.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ul.gzmigu.cn

[Q81] 字符串替换
来源：http://rl.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sh.521024.cn

[Q82] 字符长度与字节长度
来源：http://wg.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cp.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://xo.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nh.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://os.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://yn.yuexingan06.cn

[Q85] 数值取整
来源：http://ak.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fm.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://fw.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ta.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://lj.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gu.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://fq.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gw.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sl.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://uy.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wr.wgjwhj.cn

[Q90] 生成序号列
来源：http://tc.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xg.haigaiapp.cn

================================================================================
来源：http://om.chemitech.net.cn

R. Bash 专题
来源：http://wc.newstarts.cn

================================================================================
来源：http://oq.nicolike.cn

[R01] shebang 与严格模式
来源：http://pu.nszjky.cn

#!/usr/bin/env bash
来源：http://qe.521024.cn

set -euo pipefail
来源：http://sv.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://ir.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://pm.yuexingan06.cn

[R03] 只读变量
来源：http://pb.hahajie.cn

readonly PI=3.14
来源：http://kf.szxytkj.cn

[R04] 位置参数
来源：http://cg.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tw.wgjwhj.cn

[R05] 参数默认值
来源：http://ft.haigaiapp.cn

name="${1:-default}"
来源：http://tt.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://nk.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sq.nicolike.cn

[R07] if 判断文件
来源：http://ct.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xt.huanxung.cn

[R08] 数值比较
来源：http://cw.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vc.9csxet.cn

[R09] 字符串比较
来源：http://vy.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zv.panjiajie.cn

[R10] 正则匹配
来源：http://zk.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dn.muxihuayi.cn

[R11] case 多分支
来源：http://rj.hnjuh.cn

case "$1" in
来源：http://cj.huanxung.cn

start) echo "启动" ;;
来源：http://je.lnxyls.cn

stop)  echo "停止" ;;
来源：http://ny.nicolike.cn

*)     echo "未知命令" ;;
来源：http://zo.szxytkj.cn

esac
来源：http://qk.newstarts.cn

[R12] for 遍历文件
来源：http://cs.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://wy.521024.cn

[R13] for 计数循环
来源：http://ou.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://bo.colortex.cn

[R14] C 风格 for
来源：http://sq.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hh.muxihuayi.cn

[R15] while 逐行读文件
来源：http://bj.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jk.chemitech.net.cn

[R16] until 等待条件
来源：http://og.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://md.hahajie.cn

[R17] 数组定义与取值
来源：http://is.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cn.shxzukj.cn

[R18] 遍历数组
来源：http://nf.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cd.9csxet.cn

[R19] 数组长度
来源：http://di.bjjhwx.cn

echo "${#arr[@]}"
来源：http://bk.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://de.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wl.wgjwhj.cn

[R21] 字符串长度
来源：http://tx.shxzskj.cn

echo "${#s}"
来源：http://fj.huixiangedu.cn

[R22] 截取子串
来源：http://sp.shtwfgs.cn

echo "${s:0:5}"
来源：http://uy.muxihuayi.cn

[R23] 字符串替换
来源：http://va.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vc.bjjhwx.cn

[R24] 大小写转换
来源：http://pj.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qb.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://vy.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yk.hahajie.cn

[R26] 命令替换
来源：http://qp.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://fk.nszjky.cn

[R27] 算术展开
来源：http://by.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://gf.521024.cn

[R28] 浮点运算
来源：http://cl.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://eb.gzmigu.cn

[R29] 定义函数
来源：http://hh.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://md.gzmigu.cn

[R30] 函数返回状态码
来源：http://ai.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://ui.gzmigu.cn

[R31] 局部变量
来源：http://jp.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://jk.chemitech.net.cn

[R32] 参数个数校验
来源：http://et.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ma.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://wq.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eg.huixinmuqiang.cn

[R34] 退出时清理
来源：http://wa.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ka.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://tu.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zh.colortex.cn

[R36] 并发执行多个任务
来源：http://xf.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vt.newstarts.cn

[R37] 把输出赋给变量
来源：http://jq.9csxet.cn

files=$(ls -1)
来源：http://tp.shxzskj.cn

[R38] 管道串联
来源：http://cc.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://dt.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://tk.newstarts.cn

cmd > out.log 2>&1
来源：http://nn.9csxet.cn

[R40] 追加写日志
来源：http://dq.gzmigu.cn

echo "log" >> out.log
来源：http://kz.panjiajie.cn

[R41] 丢弃输出
来源：http://ep.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://hu.9csxet.cn

[R42] 输入重定向
来源：http://ka.shxzskj.cn

wc -l < a.txt
来源：http://hf.muxihuayi.cn

[R43] 按名字查找文件
来源：http://yz.newstarts.cn

find . -name "*.log" -type f
来源：http://rc.muxihuayi.cn

[R44] 按修改时间查找
来源：http://da.huixiangedu.cn

find . -mtime -7 -type f
来源：http://as.chemitech.net.cn

[R45] 批量删除
来源：http://zi.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://kr.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://zt.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mi.bjjhwx.cn

[R47] sed 单行替换
来源：http://vf.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sk.hahajie.cn

[R48] awk 取指定列
来源：http://mn.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://fc.hahajie.cn

[R49] awk 带条件
来源：http://jn.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nk.hnjuh.cn

[R50] awk 求和
来源：http://dg.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wq.szsharing.cn

[R51] 排序去重取前几
来源：http://jg.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vi.gzmigu.cn

[R52] 统计行数
来源：http://az.9csxet.cn

wc -l a.txt
来源：http://ul.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://hm.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ez.hnjuh.cn

[R54] 比较两个文件
来源：http://pm.panjiajie.cn

diff a.txt b.txt
来源：http://ln.shxzukj.cn

[R55] 压缩与解压
来源：http://eh.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dr.huixiangedu.cn

[R56] 远程拷贝
来源：http://vc.haigaiapp.cn

scp file user@host:/path/
来源：http://el.huanxung.cn

[R57] 远程执行命令
来源：http://gh.panjiajie.cn

ssh user@host 'uptime'
来源：http://og.huixinmuqiang.cn

[R58] 下载文件
来源：http://op.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pa.haigaiapp.cn

[R59] 发 POST JSON
来源：http://pn.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://yr.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sp.shxzukj.cn

[R61] 磁盘占用
来源：http://lx.szsharing.cn

df -h;  du -sh *
来源：http://tu.szsharing.cn

[R62] 找最占空间的文件
来源：http://tl.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://fn.lnxyls.cn

[R63] 内存与进程
来源：http://gf.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://tq.jctech888.com.cn

[R64] 结束进程
来源：http://iz.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://qi.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://jn.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zu.yuexingan06.cn

[R66] 定时任务
来源：http://io.9csxet.cn

crontab -e;  crontab -l
来源：http://vs.nicolike.cn

[R67] 生成随机十六进制串
来源：http://mb.9csxet.cn

openssl rand -hex 16
来源：http://eq.panjiajie.cn

[R68] 计算文件校验值
来源：http://xh.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uq.newstarts.cn

[R69] 生成随机密码
来源：http://bn.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://qe.9csxet.cn

[R70] 时间戳与互转
来源：http://ih.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://pj.yuntaijiaju.cn

[R71] 日期格式化
来源：http://ro.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ne.hnjuh.cn

[R72] 等待端口就绪
来源：http://pt.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jw.shtwfgs.cn

[R73] 分割大日志
来源：http://bm.521024.cn

split -l 1000 big.log part_
来源：http://rj.panjiajie.cn

[R74] 批量重命名
来源：http://ol.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mf.asd995.cn

[R75] 导出环境变量
来源：http://wk.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://xp.nicolike.cn

[R76] 使用临时文件
来源：http://yt.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ai.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://ag.haigaiapp.cn

read -rp "请输入: " ans
来源：http://pj.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://cc.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://af.9csxet.cn

[R79] 解析命令行选项
来源：http://hq.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ga.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://rj.shxzukj.cn

time ./run.sh
来源：http://go.panjiajie.cn

================================================================================
来源：http://po.hnjuh.cn

S. C / C++ 专题
来源：http://nk.asd995.cn

================================================================================
来源：http://gt.shxzskj.cn

[S01] C：Hello World
来源：http://ir.haigaiapp.cn

#include <stdio.h>
来源：http://zx.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rz.nicolike.cn

[S02] C：变量与格式化输出
来源：http://hi.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://eh.bjjhwx.cn

[S03] C：读入整数
来源：http://nd.asd995.cn

int x; scanf("%d", &x);
来源：http://yw.bookmarksfly.cn

[S04] C：字符串复制
来源：http://so.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ad.haigaiapp.cn

[S05] C：字符串长度
来源：http://zt.hahajie.cn

strlen(s)
来源：http://na.szsharing.cn

[S06] C：字符串比较
来源：http://gr.yuexingan06.cn

strcmp(a, b) == 0
来源：http://nt.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://dd.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oh.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://qx.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yl.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://wk.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vb.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://zy.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://eu.colortex.cn

[S11] C：逐行读文件
来源：http://rz.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://oj.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ev.asd995.cn

fclose(f);
来源：http://lk.szsharing.cn

[S12] C：写文件
来源：http://ru.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fc.gzmigu.cn

[S13] C：宏定义
来源：http://jj.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nw.chemitech.net.cn

[S14] C：枚举
来源：http://mg.wgjwhj.cn


<!-- 参考信息 -->