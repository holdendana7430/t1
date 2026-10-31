代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ya.nicolike.cn

[Q52] 删除指定行
来源：http://cx.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://us.yuexingan06.cn

[Q53] 按条件删除
来源：http://ki.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ac.chemitech.net.cn

[Q54] 清空表
来源：http://js.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://rq.hahajie.cn

[Q55] 排名（并列占位）
来源：http://bu.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vd.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://ba.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ri.nicolike.cn

[Q57] 行号
来源：http://un.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nx.shtwfgs.cn

[Q58] 累计求和
来源：http://gy.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tv.bookmarksfly.cn

[Q59] 分组内累计
来源：http://od.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://io.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://uc.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mw.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pq.lnxyls.cn

[Q61] 移动平均
来源：http://fv.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tc.asd995.cn

[Q62] 分组占比
来源：http://et.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fx.lnxyls.cn

[Q63] 开启事务
来源：http://vo.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zx.huanxung.cn

[Q64] 提交事务
来源：http://ah.szxytkj.cn

COMMIT;
来源：http://xo.newstarts.cn

[Q65] 回滚事务
来源：http://pg.shxzskj.cn

ROLLBACK;
来源：http://be.panjiajie.cn

[Q66] 行锁查询
来源：http://zf.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dq.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://ve.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://un.gzmigu.cn

[Q68] 保存点
来源：http://pr.jctech888.com.cn

SAVEPOINT sp1;
来源：http://sx.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://ma.wgjwhj.cn

[Q69] 查看执行计划
来源：http://tf.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cj.muxihuayi.cn

[Q70] 更新统计信息
来源：http://xo.huanxung.cn

ANALYZE TABLE users;
来源：http://jk.lnxyls.cn

[Q71] 查看建表语句
来源：http://hj.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qi.bjjhwx.cn

[Q72] 查看索引
来源：http://pf.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://sy.wgjwhj.cn

[Q73] 查看表状态
来源：http://qq.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ak.gzmigu.cn

[Q74] 强制使用索引
来源：http://cc.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zw.asd995.cn

[Q75] 日期格式化
来源：http://zj.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pj.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dw.asd995.cn

[Q76] 按天统计
来源：http://fy.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bo.yuexingan06.cn

[Q77] 时间加减
来源：http://uo.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://no.newstarts.cn

[Q78] 当前时间
来源：http://jn.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yj.newstarts.cn

[Q79] 字符串拼接
来源：http://ml.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://in.yuexingan06.cn

[Q80] 字符串截取
来源：http://ue.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ty.muxihuayi.cn

[Q81] 字符串替换
来源：http://gm.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zs.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://cn.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ut.yuexingan06.cn

[Q83] 大小写转换
来源：http://dj.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mp.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://bs.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://mf.hnjuh.cn

[Q85] 数值取整
来源：http://tv.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oh.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://hg.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xh.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://oo.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xc.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://kj.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hh.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rk.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://az.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ee.haigaiapp.cn

[Q90] 生成序号列
来源：http://du.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uw.colortex.cn

================================================================================
来源：http://db.hnjuh.cn

R. Bash 专题
来源：http://ly.szxytkj.cn

================================================================================
来源：http://ad.huanxung.cn

[R01] shebang 与严格模式
来源：http://wh.jctech888.com.cn

#!/usr/bin/env bash
来源：http://an.lnxyls.cn

set -euo pipefail
来源：http://xc.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://oc.9csxet.cn

name="Tom"; echo "$name"
来源：http://yt.yuexingan06.cn

[R03] 只读变量
来源：http://bh.jctech888.com.cn

readonly PI=3.14
来源：http://pv.shxzukj.cn

[R04] 位置参数
来源：http://dz.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ay.hahajie.cn

[R05] 参数默认值
来源：http://sy.huanxung.cn

name="${1:-default}"
来源：http://oz.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://qz.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://km.newstarts.cn

[R07] if 判断文件
来源：http://eu.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ga.bjjhwx.cn

[R08] 数值比较
来源：http://uw.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sc.chemitech.net.cn

[R09] 字符串比较
来源：http://gs.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hc.huanxung.cn

[R10] 正则匹配
来源：http://hf.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rt.colortex.cn

[R11] case 多分支
来源：http://bi.wgjwhj.cn

case "$1" in
来源：http://eu.shxzukj.cn

start) echo "启动" ;;
来源：http://ti.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://qp.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://tb.chemitech.net.cn

esac
来源：http://mv.huanxung.cn

[R12] for 遍历文件
来源：http://bv.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://fy.shtwfgs.cn

[R13] for 计数循环
来源：http://rt.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://qo.yuntaijiaju.cn

[R14] C 风格 for
来源：http://ai.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bl.hahajie.cn

[R15] while 逐行读文件
来源：http://sb.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bq.yuexingan06.cn

[R16] until 等待条件
来源：http://gb.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uw.hahajie.cn

[R17] 数组定义与取值
来源：http://yy.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jm.bookmarksfly.cn

[R18] 遍历数组
来源：http://mt.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oa.hahajie.cn

[R19] 数组长度
来源：http://sd.szsharing.cn

echo "${#arr[@]}"
来源：http://dy.9csxet.cn

[R20] 关联数组（字典）
来源：http://kl.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oj.haigaiapp.cn

[R21] 字符串长度
来源：http://ih.colortex.cn

echo "${#s}"
来源：http://ko.yuntaijiaju.cn

[R22] 截取子串
来源：http://yt.wgjwhj.cn

echo "${s:0:5}"
来源：http://iu.hnjuh.cn

[R23] 字符串替换
来源：http://za.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://da.nicolike.cn

[R24] 大小写转换
来源：http://iz.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://be.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://cs.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rn.chemitech.net.cn

[R26] 命令替换
来源：http://jb.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://io.shxzskj.cn

[R27] 算术展开
来源：http://ii.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://dg.bjjhwx.cn

[R28] 浮点运算
来源：http://zs.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://ul.bjjhwx.cn

[R29] 定义函数
来源：http://kh.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xr.huixiangedu.cn

[R30] 函数返回状态码
来源：http://sn.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://jy.chemitech.net.cn

[R31] 局部变量
来源：http://hr.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://ga.huixiangedu.cn

[R32] 参数个数校验
来源：http://tc.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ss.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://dv.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://im.nszjky.cn

[R34] 退出时清理
来源：http://xy.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ak.jctech888.com.cn

[R35] 后台执行并等待
来源：http://ma.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dw.panjiajie.cn

[R36] 并发执行多个任务
来源：http://nb.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wi.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://en.colortex.cn

files=$(ls -1)
来源：http://yb.nszjky.cn

[R38] 管道串联
来源：http://nm.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://sk.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://qf.yuexingan06.cn

cmd > out.log 2>&1
来源：http://hi.nicolike.cn

[R40] 追加写日志
来源：http://da.gzmigu.cn

echo "log" >> out.log
来源：http://on.haigaiapp.cn

[R41] 丢弃输出
来源：http://lj.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://lf.nszjky.cn

[R42] 输入重定向
来源：http://bu.jianghongdianzi.cn

wc -l < a.txt
来源：http://jw.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://mr.asd995.cn

find . -name "*.log" -type f
来源：http://dw.gzmigu.cn

[R44] 按修改时间查找
来源：http://ri.wgjwhj.cn

find . -mtime -7 -type f
来源：http://tg.colortex.cn

[R45] 批量删除
来源：http://mh.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://fx.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://in.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ve.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://ga.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://er.panjiajie.cn

[R48] awk 取指定列
来源：http://kc.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://hk.wgjwhj.cn

[R49] awk 带条件
来源：http://cz.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://al.lnxyls.cn

[R50] awk 求和
来源：http://wk.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fy.lnxyls.cn

[R51] 排序去重取前几
来源：http://lg.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://la.huixinmuqiang.cn

[R52] 统计行数
来源：http://cf.jctech888.com.cn

wc -l a.txt
来源：http://cd.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://ic.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ns.muxihuayi.cn

[R54] 比较两个文件
来源：http://lr.shxzukj.cn

diff a.txt b.txt
来源：http://zd.panjiajie.cn

[R55] 压缩与解压
来源：http://bm.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ij.lnxyls.cn

[R56] 远程拷贝
来源：http://wy.jianghongdianzi.cn

scp file user@host:/path/
来源：http://tl.jctech888.com.cn

[R57] 远程执行命令
来源：http://yl.shtwfgs.cn

ssh user@host 'uptime'
来源：http://fe.hahajie.cn

[R58] 下载文件
来源：http://fz.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xr.newstarts.cn

[R59] 发 POST JSON
来源：http://aa.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ch.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://ie.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eu.hahajie.cn

[R61] 磁盘占用
来源：http://we.asd995.cn

df -h;  du -sh *
来源：http://qt.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://mn.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://le.nszjky.cn

[R63] 内存与进程
来源：http://ke.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://kr.jianghongdianzi.cn

[R64] 结束进程
来源：http://np.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://nr.nicolike.cn

[R65] 查看端口占用
来源：http://nh.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yb.szxytkj.cn

[R66] 定时任务
来源：http://xs.panjiajie.cn

crontab -e;  crontab -l
来源：http://mc.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://xu.hnjuh.cn

openssl rand -hex 16
来源：http://jj.9csxet.cn

[R68] 计算文件校验值
来源：http://sw.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kr.szsharing.cn

[R69] 生成随机密码
来源：http://wb.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://rj.521024.cn

[R70] 时间戳与互转
来源：http://ng.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://zc.shxzukj.cn

[R71] 日期格式化
来源：http://qg.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ov.asd995.cn

[R72] 等待端口就绪
来源：http://fh.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fy.colortex.cn

[R73] 分割大日志
来源：http://ou.lnxyls.cn

split -l 1000 big.log part_
来源：http://jy.jianghongdianzi.cn

[R74] 批量重命名
来源：http://di.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sk.bookmarksfly.cn

[R75] 导出环境变量
来源：http://so.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://mi.nszjky.cn

[R76] 使用临时文件
来源：http://pb.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gh.nszjky.cn

[R77] 读取用户输入
来源：http://lw.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://tr.hnjuh.cn

[R78] 交互式菜单
来源：http://rn.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ca.bjjhwx.cn

[R79] 解析命令行选项
来源：http://gd.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cw.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://mu.szsharing.cn

time ./run.sh
来源：http://dy.wgjwhj.cn

================================================================================
来源：http://ft.521024.cn

S. C / C++ 专题
来源：http://zk.huixinmuqiang.cn

================================================================================
来源：http://se.panjiajie.cn

[S01] C：Hello World
来源：http://pn.9csxet.cn

#include <stdio.h>
来源：http://re.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nf.9csxet.cn

[S02] C：变量与格式化输出
来源：http://gp.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://sv.hahajie.cn

[S03] C：读入整数
来源：http://eh.newstarts.cn

int x; scanf("%d", &x);
来源：http://bl.shxzukj.cn

[S04] C：字符串复制
来源：http://et.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uo.newstarts.cn

[S05] C：字符串长度
来源：http://cw.huanxung.cn

strlen(s)
来源：http://ks.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://qo.colortex.cn

strcmp(a, b) == 0
来源：http://il.colortex.cn

[S07] C：数组遍历求和
来源：http://hu.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jm.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://qq.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kw.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://iw.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yb.muxihuayi.cn

[S10] C：指针与解引用
来源：http://vx.szsharing.cn

int *p = &a;  *p = 5;
来源：http://bz.shxzukj.cn

[S11] C：逐行读文件
来源：http://sy.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://qt.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xi.jctech888.com.cn

fclose(f);
来源：http://wv.panjiajie.cn

[S12] C：写文件
来源：http://ir.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cl.521024.cn

[S13] C：宏定义
来源：http://an.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qz.gzmigu.cn

[S14] C：枚举
来源：http://gu.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://wy.jianghongdianzi.cn

[S15] C：类型转换
来源：http://tb.shxzukj.cn

(double) a / b
来源：http://wd.panjiajie.cn

[S16] C：位操作置位
来源：http://lg.jctech888.com.cn

x |= (1 << 3);
来源：http://uu.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://kw.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tg.szsharing.cn

[S18] C：命令行参数
来源：http://rl.huixiangedu.cn

int main(int argc, char **argv)
来源：http://ao.chemitech.net.cn

[S19] C：快速排序
来源：http://mq.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vm.huixiangedu.cn

[S20] C：二分查找
来源：http://hu.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zn.asd995.cn

[S21] C：字符类别判断
来源：http://yy.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nn.shtwfgs.cn

[S22] C：字符串转数字
来源：http://na.huixinmuqiang.cn


<!-- 参考信息 -->