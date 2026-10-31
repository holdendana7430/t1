代发 wailian999

[Q44] IN 子查询
来源：http://jj.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hs.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://cs.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ek.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cr.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mv.hnjuh.cn

[Q47] 与平均值比较
来源：http://ud.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ya.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://ly.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qu.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://bp.lnxyls.cn

[Q49] 更新单行
来源：http://bg.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rd.asd995.cn

[Q50] 批量更新
来源：http://ew.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://et.newstarts.cn

[Q51] 用子查询更新
来源：http://zq.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wy.hnjuh.cn

[Q52] 删除指定行
来源：http://jo.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://ip.nszjky.cn

[Q53] 按条件删除
来源：http://nn.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rh.521024.cn

[Q54] 清空表
来源：http://gd.9csxet.cn

TRUNCATE TABLE logs;
来源：http://mn.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://ct.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://es.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://fy.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dd.nszjky.cn

[Q57] 行号
来源：http://au.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pe.huixinmuqiang.cn

[Q58] 累计求和
来源：http://ss.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jz.nicolike.cn

[Q59] 分组内累计
来源：http://do.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vq.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://pu.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dj.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://az.gzmigu.cn

[Q61] 移动平均
来源：http://mv.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mf.huixinmuqiang.cn

[Q62] 分组占比
来源：http://fz.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ti.nszjky.cn

[Q63] 开启事务
来源：http://hf.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bv.haigaiapp.cn

[Q64] 提交事务
来源：http://jr.bjjhwx.cn

COMMIT;
来源：http://nv.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://xn.huixinmuqiang.cn

ROLLBACK;
来源：http://jm.newstarts.cn

[Q66] 行锁查询
来源：http://ko.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zj.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://kf.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oq.haigaiapp.cn

[Q68] 保存点
来源：http://vs.newstarts.cn

SAVEPOINT sp1;
来源：http://vy.newstarts.cn

ROLLBACK TO sp1;
来源：http://cp.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://yh.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dc.szxytkj.cn

[Q70] 更新统计信息
来源：http://ka.hahajie.cn

ANALYZE TABLE users;
来源：http://zf.bjjhwx.cn

[Q71] 查看建表语句
来源：http://au.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gg.521024.cn

[Q72] 查看索引
来源：http://fh.huanxung.cn

SHOW INDEX FROM users;
来源：http://he.gzmigu.cn

[Q73] 查看表状态
来源：http://ul.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uz.yuexingan06.cn

[Q74] 强制使用索引
来源：http://kd.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bx.lnxyls.cn

[Q75] 日期格式化
来源：http://nm.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tw.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://to.yuntaijiaju.cn

[Q76] 按天统计
来源：http://br.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oo.yuntaijiaju.cn

[Q77] 时间加减
来源：http://si.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oh.colortex.cn

[Q78] 当前时间
来源：http://bh.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nc.shtwfgs.cn

[Q79] 字符串拼接
来源：http://mu.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wq.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://sn.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://im.bookmarksfly.cn

[Q81] 字符串替换
来源：http://el.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ex.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://cu.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ow.nszjky.cn

[Q83] 大小写转换
来源：http://dl.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ee.9csxet.cn

[Q84] 去除首尾空格
来源：http://yy.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://nq.shtwfgs.cn

[Q85] 数值取整
来源：http://mf.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://op.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://oh.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pz.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://ic.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vz.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://et.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wk.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://if.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://hr.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mw.gzmigu.cn

[Q90] 生成序号列
来源：http://yr.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://el.panjiajie.cn

================================================================================
来源：http://eg.hahajie.cn

R. Bash 专题
来源：http://tg.9csxet.cn

================================================================================
来源：http://av.shxzukj.cn

[R01] shebang 与严格模式
来源：http://lf.9csxet.cn

#!/usr/bin/env bash
来源：http://eb.hahajie.cn

set -euo pipefail
来源：http://vo.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://vf.lnxyls.cn

name="Tom"; echo "$name"
来源：http://dh.nszjky.cn

[R03] 只读变量
来源：http://pl.hahajie.cn

readonly PI=3.14
来源：http://je.szxytkj.cn

[R04] 位置参数
来源：http://kv.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://is.shxzskj.cn

[R05] 参数默认值
来源：http://dd.shtwfgs.cn

name="${1:-default}"
来源：http://ci.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://hx.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ac.huixiangedu.cn

[R07] if 判断文件
来源：http://lb.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fg.szxytkj.cn

[R08] 数值比较
来源：http://ix.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iy.colortex.cn

[R09] 字符串比较
来源：http://lm.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nb.9csxet.cn

[R10] 正则匹配
来源：http://ik.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tc.hahajie.cn

[R11] case 多分支
来源：http://qf.gzmigu.cn

case "$1" in
来源：http://on.9csxet.cn

start) echo "启动" ;;
来源：http://ri.lnxyls.cn

stop)  echo "停止" ;;
来源：http://lo.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://xm.521024.cn

esac
来源：http://pw.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://vz.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://oc.hnjuh.cn

[R13] for 计数循环
来源：http://hp.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://wv.bookmarksfly.cn

[R14] C 风格 for
来源：http://aj.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nt.nicolike.cn

[R15] while 逐行读文件
来源：http://jd.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yo.jctech888.com.cn

[R16] until 等待条件
来源：http://em.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tb.newstarts.cn

[R17] 数组定义与取值
来源：http://sr.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://li.haigaiapp.cn

[R18] 遍历数组
来源：http://ez.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fe.jianghongdianzi.cn

[R19] 数组长度
来源：http://ww.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://sa.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://td.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ud.nicolike.cn

[R21] 字符串长度
来源：http://lz.haigaiapp.cn

echo "${#s}"
来源：http://hn.yuntaijiaju.cn

[R22] 截取子串
来源：http://bg.shxzskj.cn

echo "${s:0:5}"
来源：http://to.hahajie.cn

[R23] 字符串替换
来源：http://to.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ny.chemitech.net.cn

[R24] 大小写转换
来源：http://mg.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ku.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://kq.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fa.lnxyls.cn

[R26] 命令替换
来源：http://wr.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://du.9csxet.cn

[R27] 算术展开
来源：http://uq.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://ny.jianghongdianzi.cn

[R28] 浮点运算
来源：http://fm.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://pc.9csxet.cn

[R29] 定义函数
来源：http://wj.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yq.haigaiapp.cn

[R30] 函数返回状态码
来源：http://jf.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://fs.jctech888.com.cn

[R31] 局部变量
来源：http://lk.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://uw.shtwfgs.cn

[R32] 参数个数校验
来源：http://yi.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gq.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://ob.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://es.szxytkj.cn

[R34] 退出时清理
来源：http://rb.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uu.newstarts.cn

[R35] 后台执行并等待
来源：http://hi.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gl.nszjky.cn

[R36] 并发执行多个任务
来源：http://ju.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cl.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://jh.szsharing.cn

files=$(ls -1)
来源：http://mv.jianghongdianzi.cn

[R38] 管道串联
来源：http://ge.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://ao.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://jp.wgjwhj.cn

cmd > out.log 2>&1
来源：http://lf.muxihuayi.cn

[R40] 追加写日志
来源：http://tj.yuntaijiaju.cn

echo "log" >> out.log
来源：http://lt.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://ak.asd995.cn

cmd >/dev/null 2>&1
来源：http://pc.panjiajie.cn

[R42] 输入重定向
来源：http://fv.shtwfgs.cn

wc -l < a.txt
来源：http://zg.huixiangedu.cn

[R43] 按名字查找文件
来源：http://zu.9csxet.cn

find . -name "*.log" -type f
来源：http://tg.hahajie.cn

[R44] 按修改时间查找
来源：http://je.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://wt.nicolike.cn

[R45] 批量删除
来源：http://nm.szsharing.cn

find . -name "*.tmp" -delete
来源：http://iv.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://iv.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sg.huanxung.cn

[R47] sed 单行替换
来源：http://gt.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vg.wgjwhj.cn

[R48] awk 取指定列
来源：http://gd.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://rf.jctech888.com.cn

[R49] awk 带条件
来源：http://oy.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fy.szsharing.cn

[R50] awk 求和
来源：http://pt.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lv.nszjky.cn

[R51] 排序去重取前几
来源：http://bw.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fb.lnxyls.cn

[R52] 统计行数
来源：http://jr.shxzukj.cn

wc -l a.txt
来源：http://pd.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://jw.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yf.hnjuh.cn

[R54] 比较两个文件
来源：http://vy.panjiajie.cn

diff a.txt b.txt
来源：http://pi.haigaiapp.cn

[R55] 压缩与解压
来源：http://dz.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ai.newstarts.cn

[R56] 远程拷贝
来源：http://hg.asd995.cn

scp file user@host:/path/
来源：http://it.nicolike.cn

[R57] 远程执行命令
来源：http://nq.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://kg.szxytkj.cn

[R58] 下载文件
来源：http://om.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yc.newstarts.cn

[R59] 发 POST JSON
来源：http://wh.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ib.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://yh.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ez.szxytkj.cn

[R61] 磁盘占用
来源：http://wr.shtwfgs.cn

df -h;  du -sh *
来源：http://me.newstarts.cn

[R62] 找最占空间的文件
来源：http://ha.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://gr.jianghongdianzi.cn

[R63] 内存与进程
来源：http://ym.521024.cn

free -h;  ps aux | grep nginx
来源：http://ln.bjjhwx.cn

[R64] 结束进程
来源：http://qn.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://zr.colortex.cn

[R65] 查看端口占用
来源：http://tx.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jb.huanxung.cn

[R66] 定时任务
来源：http://es.nszjky.cn

crontab -e;  crontab -l
来源：http://lx.9csxet.cn

[R67] 生成随机十六进制串
来源：http://wz.colortex.cn

openssl rand -hex 16
来源：http://jy.wgjwhj.cn

[R68] 计算文件校验值
来源：http://eo.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ma.521024.cn

[R69] 生成随机密码
来源：http://bh.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://kk.nicolike.cn

[R70] 时间戳与互转
来源：http://sy.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://sr.newstarts.cn

[R71] 日期格式化
来源：http://pd.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cy.chemitech.net.cn

[R72] 等待端口就绪
来源：http://na.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fj.bjjhwx.cn

[R73] 分割大日志
来源：http://rp.nszjky.cn

split -l 1000 big.log part_
来源：http://fn.jianghongdianzi.cn

[R74] 批量重命名
来源：http://ll.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://me.muxihuayi.cn

[R75] 导出环境变量
来源：http://zm.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://xo.shtwfgs.cn

[R76] 使用临时文件
来源：http://pr.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vr.colortex.cn

[R77] 读取用户输入
来源：http://mx.asd995.cn

read -rp "请输入: " ans
来源：http://wd.szsharing.cn

[R78] 交互式菜单
来源：http://ny.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yp.shxzskj.cn

[R79] 解析命令行选项
来源：http://xu.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ye.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://qs.521024.cn

time ./run.sh
来源：http://jm.huanxung.cn

================================================================================
来源：http://bu.hahajie.cn

S. C / C++ 专题
来源：http://wx.huixinmuqiang.cn

================================================================================
来源：http://zr.shtwfgs.cn

[S01] C：Hello World
来源：http://cn.521024.cn

#include <stdio.h>
来源：http://bt.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fh.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://vz.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://ku.yuntaijiaju.cn

[S03] C：读入整数
来源：http://eq.newstarts.cn

int x; scanf("%d", &x);
来源：http://nn.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://tu.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lx.hnjuh.cn

[S05] C：字符串长度
来源：http://vl.yuexingan06.cn

strlen(s)
来源：http://eo.nszjky.cn

[S06] C：字符串比较
来源：http://qv.jctech888.com.cn

strcmp(a, b) == 0
来源：http://bp.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://hu.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wj.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://xe.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xt.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://dy.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bp.yuexingan06.cn

[S10] C：指针与解引用
来源：http://rt.521024.cn

int *p = &a;  *p = 5;
来源：http://sm.gzmigu.cn

[S11] C：逐行读文件
来源：http://tg.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://nr.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jw.jianghongdianzi.cn

fclose(f);
来源：http://mn.wgjwhj.cn

[S12] C：写文件
来源：http://jy.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dt.jctech888.com.cn

[S13] C：宏定义
来源：http://hs.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zq.bjjhwx.cn

[S14] C：枚举
来源：http://dg.yuexingan06.cn


<!-- 参考信息 -->