代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://qw.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ue.nszjky.cn

[Q47] 与平均值比较
来源：http://ok.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hg.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://pj.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vp.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ht.szxytkj.cn

[Q49] 更新单行
来源：http://qu.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://br.jctech888.com.cn

[Q50] 批量更新
来源：http://jv.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vo.521024.cn

[Q51] 用子查询更新
来源：http://xz.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hw.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://dd.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://nc.gzmigu.cn

[Q53] 按条件删除
来源：http://mo.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nb.shtwfgs.cn

[Q54] 清空表
来源：http://ps.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://jz.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://sc.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sb.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://xy.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ca.jctech888.com.cn

[Q57] 行号
来源：http://at.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hx.nszjky.cn

[Q58] 累计求和
来源：http://ys.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mw.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://sb.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hd.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://sy.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tg.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wr.colortex.cn

[Q61] 移动平均
来源：http://ky.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ap.asd995.cn

[Q62] 分组占比
来源：http://xa.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xb.nicolike.cn

[Q63] 开启事务
来源：http://ir.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ca.nicolike.cn

[Q64] 提交事务
来源：http://sj.hnjuh.cn

COMMIT;
来源：http://za.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://xq.yuexingan06.cn

ROLLBACK;
来源：http://bw.wgjwhj.cn

[Q66] 行锁查询
来源：http://se.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ot.panjiajie.cn

[Q67] 设置隔离级别
来源：http://jb.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yx.jctech888.com.cn

[Q68] 保存点
来源：http://gp.shxzukj.cn

SAVEPOINT sp1;
来源：http://hi.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://fn.jctech888.com.cn

[Q69] 查看执行计划
来源：http://gm.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tq.asd995.cn

[Q70] 更新统计信息
来源：http://in.9csxet.cn

ANALYZE TABLE users;
来源：http://by.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://fq.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pm.newstarts.cn

[Q72] 查看索引
来源：http://ca.colortex.cn

SHOW INDEX FROM users;
来源：http://dk.gzmigu.cn

[Q73] 查看表状态
来源：http://kv.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rf.bjjhwx.cn

[Q74] 强制使用索引
来源：http://yz.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fs.asd995.cn

[Q75] 日期格式化
来源：http://ux.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vk.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vf.gzmigu.cn

[Q76] 按天统计
来源：http://on.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lw.haigaiapp.cn

[Q77] 时间加减
来源：http://dj.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ge.szsharing.cn

[Q78] 当前时间
来源：http://zs.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fm.muxihuayi.cn

[Q79] 字符串拼接
来源：http://qm.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://di.bjjhwx.cn

[Q80] 字符串截取
来源：http://kv.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://im.chemitech.net.cn

[Q81] 字符串替换
来源：http://ss.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qb.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://xu.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wf.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://xb.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ki.panjiajie.cn

[Q84] 去除首尾空格
来源：http://zk.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://lx.wgjwhj.cn

[Q85] 数值取整
来源：http://sm.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nd.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://mt.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cl.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://bu.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wv.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://fc.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vk.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cq.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://sp.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ft.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://ei.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sc.asd995.cn

================================================================================
来源：http://kx.nicolike.cn

R. Bash 专题
来源：http://pf.521024.cn

================================================================================
来源：http://yj.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://uy.wgjwhj.cn

#!/usr/bin/env bash
来源：http://qs.hahajie.cn

set -euo pipefail
来源：http://wx.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://cd.nszjky.cn

name="Tom"; echo "$name"
来源：http://wn.haigaiapp.cn

[R03] 只读变量
来源：http://no.lnxyls.cn

readonly PI=3.14
来源：http://ek.jianghongdianzi.cn

[R04] 位置参数
来源：http://rv.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bx.jctech888.com.cn

[R05] 参数默认值
来源：http://xq.panjiajie.cn

name="${1:-default}"
来源：http://ge.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://wz.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mx.chemitech.net.cn

[R07] if 判断文件
来源：http://iu.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lj.huanxung.cn

[R08] 数值比较
来源：http://eu.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ca.hahajie.cn

[R09] 字符串比较
来源：http://ke.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kn.shxzukj.cn

[R10] 正则匹配
来源：http://qi.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cy.hahajie.cn

[R11] case 多分支
来源：http://jd.bjjhwx.cn

case "$1" in
来源：http://gg.asd995.cn

start) echo "启动" ;;
来源：http://fw.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://ev.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://bu.bookmarksfly.cn

esac
来源：http://pr.asd995.cn

[R12] for 遍历文件
来源：http://cy.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://fn.yuexingan06.cn

[R13] for 计数循环
来源：http://nh.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://dl.chemitech.net.cn

[R14] C 风格 for
来源：http://nq.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fk.nicolike.cn

[R15] while 逐行读文件
来源：http://qn.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hn.9csxet.cn

[R16] until 等待条件
来源：http://ms.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rd.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://vb.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ep.nszjky.cn

[R18] 遍历数组
来源：http://gh.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mc.shxzukj.cn

[R19] 数组长度
来源：http://qd.nszjky.cn

echo "${#arr[@]}"
来源：http://do.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://pp.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hy.yuexingan06.cn

[R21] 字符串长度
来源：http://hk.yuexingan06.cn

echo "${#s}"
来源：http://lz.huixiangedu.cn

[R22] 截取子串
来源：http://wg.chemitech.net.cn

echo "${s:0:5}"
来源：http://cq.hahajie.cn

[R23] 字符串替换
来源：http://am.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nw.shxzskj.cn

[R24] 大小写转换
来源：http://ax.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qt.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://ms.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xn.jianghongdianzi.cn

[R26] 命令替换
来源：http://pj.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://da.newstarts.cn

[R27] 算术展开
来源：http://ts.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://tw.nszjky.cn

[R28] 浮点运算
来源：http://rh.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://to.bjjhwx.cn

[R29] 定义函数
来源：http://va.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gi.shtwfgs.cn

[R30] 函数返回状态码
来源：http://vt.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://rd.huanxung.cn

[R31] 局部变量
来源：http://wa.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://rw.gzmigu.cn

[R32] 参数个数校验
来源：http://mv.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wf.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://mh.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xe.huixiangedu.cn

[R34] 退出时清理
来源：http://yq.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cv.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://yo.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zk.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://hx.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bl.9csxet.cn

[R37] 把输出赋给变量
来源：http://kd.huanxung.cn

files=$(ls -1)
来源：http://ya.jianghongdianzi.cn

[R38] 管道串联
来源：http://lx.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://di.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://ps.jctech888.com.cn

cmd > out.log 2>&1
来源：http://dc.shxzskj.cn

[R40] 追加写日志
来源：http://xy.nicolike.cn

echo "log" >> out.log
来源：http://ih.nszjky.cn

[R41] 丢弃输出
来源：http://zt.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://mx.gzmigu.cn

[R42] 输入重定向
来源：http://ve.panjiajie.cn

wc -l < a.txt
来源：http://wr.nszjky.cn

[R43] 按名字查找文件
来源：http://ri.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://pt.haigaiapp.cn

[R44] 按修改时间查找
来源：http://ap.521024.cn

find . -mtime -7 -type f
来源：http://az.yuntaijiaju.cn

[R45] 批量删除
来源：http://jd.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://au.hnjuh.cn

[R46] 递归替换文件内容
来源：http://cc.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://po.szsharing.cn

[R47] sed 单行替换
来源：http://we.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hw.szsharing.cn

[R48] awk 取指定列
来源：http://id.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://ef.shtwfgs.cn

[R49] awk 带条件
来源：http://md.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bz.chemitech.net.cn

[R50] awk 求和
来源：http://vh.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qc.bjjhwx.cn

[R51] 排序去重取前几
来源：http://mt.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pv.huanxung.cn

[R52] 统计行数
来源：http://fs.szxytkj.cn

wc -l a.txt
来源：http://gm.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://vh.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hs.nszjky.cn

[R54] 比较两个文件
来源：http://np.nicolike.cn

diff a.txt b.txt
来源：http://cv.szsharing.cn

[R55] 压缩与解压
来源：http://ql.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bh.bjjhwx.cn

[R56] 远程拷贝
来源：http://zt.521024.cn

scp file user@host:/path/
来源：http://zi.newstarts.cn

[R57] 远程执行命令
来源：http://bn.szsharing.cn

ssh user@host 'uptime'
来源：http://fi.colortex.cn

[R58] 下载文件
来源：http://ex.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lj.colortex.cn

[R59] 发 POST JSON
来源：http://pb.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tu.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://zv.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pc.9csxet.cn

[R61] 磁盘占用
来源：http://gy.newstarts.cn

df -h;  du -sh *
来源：http://yg.newstarts.cn

[R62] 找最占空间的文件
来源：http://md.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://pf.9csxet.cn

[R63] 内存与进程
来源：http://oh.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://of.wgjwhj.cn

[R64] 结束进程
来源：http://np.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://uh.yuexingan06.cn

[R65] 查看端口占用
来源：http://nx.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ji.huanxung.cn

[R66] 定时任务
来源：http://xq.shxzskj.cn

crontab -e;  crontab -l
来源：http://kx.hahajie.cn

[R67] 生成随机十六进制串
来源：http://uv.panjiajie.cn

openssl rand -hex 16
来源：http://qr.shtwfgs.cn

[R68] 计算文件校验值
来源：http://cb.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cc.9csxet.cn

[R69] 生成随机密码
来源：http://ih.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://rt.shtwfgs.cn

[R70] 时间戳与互转
来源：http://sm.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://hj.asd995.cn

[R71] 日期格式化
来源：http://oc.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bm.wgjwhj.cn

[R72] 等待端口就绪
来源：http://xq.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jv.haigaiapp.cn

[R73] 分割大日志
来源：http://ma.lnxyls.cn

split -l 1000 big.log part_
来源：http://xn.521024.cn

[R74] 批量重命名
来源：http://fr.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ve.lnxyls.cn

[R75] 导出环境变量
来源：http://qp.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://xl.huixiangedu.cn

[R76] 使用临时文件
来源：http://tw.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uh.panjiajie.cn

[R77] 读取用户输入
来源：http://fl.panjiajie.cn

read -rp "请输入: " ans
来源：http://jf.nszjky.cn

[R78] 交互式菜单
来源：http://lq.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vt.panjiajie.cn

[R79] 解析命令行选项
来源：http://cm.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rw.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://er.bookmarksfly.cn

time ./run.sh
来源：http://it.newstarts.cn

================================================================================
来源：http://kx.shtwfgs.cn

S. C / C++ 专题
来源：http://jk.newstarts.cn

================================================================================
来源：http://mv.huixiangedu.cn

[S01] C：Hello World
来源：http://eh.huixinmuqiang.cn

#include <stdio.h>
来源：http://bm.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kr.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://ce.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://ko.yuexingan06.cn

[S03] C：读入整数
来源：http://jg.huanxung.cn

int x; scanf("%d", &x);
来源：http://qz.panjiajie.cn

[S04] C：字符串复制
来源：http://yf.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zj.muxihuayi.cn

[S05] C：字符串长度
来源：http://ke.huixiangedu.cn

strlen(s)
来源：http://qn.gzmigu.cn

[S06] C：字符串比较
来源：http://bp.gzmigu.cn

strcmp(a, b) == 0
来源：http://rl.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://wp.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nd.asd995.cn

[S08] C：动态内存分配与释放
来源：http://ws.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qo.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://wz.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dq.shtwfgs.cn

[S10] C：指针与解引用
来源：http://qf.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://um.gzmigu.cn

[S11] C：逐行读文件
来源：http://hv.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://vv.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xr.jianghongdianzi.cn

fclose(f);
来源：http://yh.nszjky.cn

[S12] C：写文件
来源：http://sm.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sx.jctech888.com.cn

[S13] C：宏定义
来源：http://xw.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rv.shxzukj.cn

[S14] C：枚举
来源：http://sw.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://fo.jctech888.com.cn

[S15] C：类型转换
来源：http://au.jctech888.com.cn

(double) a / b
来源：http://en.9csxet.cn

[S16] C：位操作置位
来源：http://uh.bjjhwx.cn


<!-- 参考信息 -->