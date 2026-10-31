代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sy.colortex.cn

[Q52] 删除指定行
来源：http://ar.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://kf.asd995.cn

[Q53] 按条件删除
来源：http://kb.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vu.lnxyls.cn

[Q54] 清空表
来源：http://yl.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://vj.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://ne.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nm.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://zj.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ge.bjjhwx.cn

[Q57] 行号
来源：http://tp.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cm.gzmigu.cn

[Q58] 累计求和
来源：http://tk.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nx.muxihuayi.cn

[Q59] 分组内累计
来源：http://kh.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bc.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://lj.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qu.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dr.nicolike.cn

[Q61] 移动平均
来源：http://md.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zg.nszjky.cn

[Q62] 分组占比
来源：http://es.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pe.newstarts.cn

[Q63] 开启事务
来源：http://xl.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zs.gzmigu.cn

[Q64] 提交事务
来源：http://wa.huixiangedu.cn

COMMIT;
来源：http://wo.bjjhwx.cn

[Q65] 回滚事务
来源：http://vu.haigaiapp.cn

ROLLBACK;
来源：http://up.9csxet.cn

[Q66] 行锁查询
来源：http://sn.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cd.newstarts.cn

[Q67] 设置隔离级别
来源：http://ml.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vf.shxzskj.cn

[Q68] 保存点
来源：http://ab.521024.cn

SAVEPOINT sp1;
来源：http://mw.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://pi.huixiangedu.cn

[Q69] 查看执行计划
来源：http://vf.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ck.nszjky.cn

[Q70] 更新统计信息
来源：http://yy.shxzukj.cn

ANALYZE TABLE users;
来源：http://hy.521024.cn

[Q71] 查看建表语句
来源：http://ud.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hf.asd995.cn

[Q72] 查看索引
来源：http://bc.newstarts.cn

SHOW INDEX FROM users;
来源：http://fs.521024.cn

[Q73] 查看表状态
来源：http://tt.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sg.9csxet.cn

[Q74] 强制使用索引
来源：http://vz.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lh.shxzukj.cn

[Q75] 日期格式化
来源：http://ba.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vl.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hd.lnxyls.cn

[Q76] 按天统计
来源：http://bb.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yk.shxzskj.cn

[Q77] 时间加减
来源：http://wz.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ty.szxytkj.cn

[Q78] 当前时间
来源：http://dh.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tl.hnjuh.cn

[Q79] 字符串拼接
来源：http://ok.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nc.szsharing.cn

[Q80] 字符串截取
来源：http://fz.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qi.szsharing.cn

[Q81] 字符串替换
来源：http://om.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bn.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://yk.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fw.9csxet.cn

[Q83] 大小写转换
来源：http://rb.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ba.newstarts.cn

[Q84] 去除首尾空格
来源：http://mv.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://uj.hnjuh.cn

[Q85] 数值取整
来源：http://ig.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://co.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://ck.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ik.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://un.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://py.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://wf.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://he.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zt.9csxet.cn

[Q89] 判断表是否存在
来源：http://rl.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ey.9csxet.cn

[Q90] 生成序号列
来源：http://av.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zw.colortex.cn

================================================================================
来源：http://ey.bjjhwx.cn

R. Bash 专题
来源：http://jg.bookmarksfly.cn

================================================================================
来源：http://wd.newstarts.cn

[R01] shebang 与严格模式
来源：http://ib.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://fi.gzmigu.cn

set -euo pipefail
来源：http://eu.521024.cn

[R02] 变量赋值与使用
来源：http://bd.hnjuh.cn

name="Tom"; echo "$name"
来源：http://gw.shxzskj.cn

[R03] 只读变量
来源：http://py.hahajie.cn

readonly PI=3.14
来源：http://jq.huixinmuqiang.cn

[R04] 位置参数
来源：http://wp.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://co.szsharing.cn

[R05] 参数默认值
来源：http://xp.huixiangedu.cn

name="${1:-default}"
来源：http://zm.lnxyls.cn

[R06] 判断命令是否存在
来源：http://uc.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xh.jianghongdianzi.cn

[R07] if 判断文件
来源：http://cj.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wj.yuntaijiaju.cn

[R08] 数值比较
来源：http://ch.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zh.shxzukj.cn

[R09] 字符串比较
来源：http://dy.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sk.panjiajie.cn

[R10] 正则匹配
来源：http://ae.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qs.colortex.cn

[R11] case 多分支
来源：http://lg.wgjwhj.cn

case "$1" in
来源：http://mf.lnxyls.cn

start) echo "启动" ;;
来源：http://bz.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://bt.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://py.lnxyls.cn

esac
来源：http://gj.haigaiapp.cn

[R12] for 遍历文件
来源：http://me.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://bq.colortex.cn

[R13] for 计数循环
来源：http://ms.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://od.gzmigu.cn

[R14] C 风格 for
来源：http://lt.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gw.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://ca.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ap.521024.cn

[R16] until 等待条件
来源：http://fe.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tj.shxzukj.cn

[R17] 数组定义与取值
来源：http://vv.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://am.jctech888.com.cn

[R18] 遍历数组
来源：http://ze.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gi.bookmarksfly.cn

[R19] 数组长度
来源：http://oz.wgjwhj.cn

echo "${#arr[@]}"
来源：http://ey.9csxet.cn

[R20] 关联数组（字典）
来源：http://yp.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hl.gzmigu.cn

[R21] 字符串长度
来源：http://jh.panjiajie.cn

echo "${#s}"
来源：http://ok.shxzukj.cn

[R22] 截取子串
来源：http://kw.lnxyls.cn

echo "${s:0:5}"
来源：http://dz.bookmarksfly.cn

[R23] 字符串替换
来源：http://nt.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vt.huixiangedu.cn

[R24] 大小写转换
来源：http://nl.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fp.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://mb.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oo.chemitech.net.cn

[R26] 命令替换
来源：http://yt.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://ce.huixinmuqiang.cn

[R27] 算术展开
来源：http://vu.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://sl.9csxet.cn

[R28] 浮点运算
来源：http://lf.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://ei.yuntaijiaju.cn

[R29] 定义函数
来源：http://ws.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zx.lnxyls.cn

[R30] 函数返回状态码
来源：http://ow.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://bw.shtwfgs.cn

[R31] 局部变量
来源：http://sd.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://xo.shxzskj.cn

[R32] 参数个数校验
来源：http://ya.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://av.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://rf.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://st.hnjuh.cn

[R34] 退出时清理
来源：http://vj.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aw.huanxung.cn

[R35] 后台执行并等待
来源：http://kc.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kd.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://by.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vf.nszjky.cn

[R37] 把输出赋给变量
来源：http://da.panjiajie.cn

files=$(ls -1)
来源：http://na.yuntaijiaju.cn

[R38] 管道串联
来源：http://cf.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://gk.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://qi.asd995.cn

cmd > out.log 2>&1
来源：http://tf.panjiajie.cn

[R40] 追加写日志
来源：http://yu.9csxet.cn

echo "log" >> out.log
来源：http://wq.hnjuh.cn

[R41] 丢弃输出
来源：http://qs.521024.cn

cmd >/dev/null 2>&1
来源：http://ic.newstarts.cn

[R42] 输入重定向
来源：http://iy.nicolike.cn

wc -l < a.txt
来源：http://cj.huixiangedu.cn

[R43] 按名字查找文件
来源：http://wm.haigaiapp.cn

find . -name "*.log" -type f
来源：http://nl.szsharing.cn

[R44] 按修改时间查找
来源：http://an.bjjhwx.cn

find . -mtime -7 -type f
来源：http://jb.yuexingan06.cn

[R45] 批量删除
来源：http://wb.newstarts.cn

find . -name "*.tmp" -delete
来源：http://dk.huanxung.cn

[R46] 递归替换文件内容
来源：http://zs.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pt.hnjuh.cn

[R47] sed 单行替换
来源：http://dp.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kx.hahajie.cn

[R48] awk 取指定列
来源：http://wu.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://by.521024.cn

[R49] awk 带条件
来源：http://qh.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://du.wgjwhj.cn

[R50] awk 求和
来源：http://zq.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cn.huixiangedu.cn

[R51] 排序去重取前几
来源：http://rk.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://if.shtwfgs.cn

[R52] 统计行数
来源：http://hg.hahajie.cn

wc -l a.txt
来源：http://zz.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://ip.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://it.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://cv.9csxet.cn

diff a.txt b.txt
来源：http://ug.panjiajie.cn

[R55] 压缩与解压
来源：http://qr.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ne.hnjuh.cn

[R56] 远程拷贝
来源：http://en.9csxet.cn

scp file user@host:/path/
来源：http://ja.shxzskj.cn

[R57] 远程执行命令
来源：http://ql.shxzukj.cn

ssh user@host 'uptime'
来源：http://mg.haigaiapp.cn

[R58] 下载文件
来源：http://tg.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kl.shxzukj.cn

[R59] 发 POST JSON
来源：http://pk.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jp.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://nl.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dl.shtwfgs.cn

[R61] 磁盘占用
来源：http://gy.wgjwhj.cn

df -h;  du -sh *
来源：http://me.hnjuh.cn

[R62] 找最占空间的文件
来源：http://pw.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://uo.hahajie.cn

[R63] 内存与进程
来源：http://tc.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://tu.bjjhwx.cn

[R64] 结束进程
来源：http://cd.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://ug.shxzskj.cn

[R65] 查看端口占用
来源：http://cs.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ms.panjiajie.cn

[R66] 定时任务
来源：http://uk.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://pd.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://ln.bookmarksfly.cn

openssl rand -hex 16
来源：http://dt.chemitech.net.cn

[R68] 计算文件校验值
来源：http://rc.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ap.521024.cn

[R69] 生成随机密码
来源：http://ur.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://sa.gzmigu.cn

[R70] 时间戳与互转
来源：http://cw.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://ye.wgjwhj.cn

[R71] 日期格式化
来源：http://zp.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gd.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://gk.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iq.shxzskj.cn

[R73] 分割大日志
来源：http://hk.asd995.cn

split -l 1000 big.log part_
来源：http://nd.huixiangedu.cn

[R74] 批量重命名
来源：http://wm.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fg.wgjwhj.cn

[R75] 导出环境变量
来源：http://ui.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://jq.9csxet.cn

[R76] 使用临时文件
来源：http://hp.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://im.shxzukj.cn

[R77] 读取用户输入
来源：http://sx.shtwfgs.cn

read -rp "请输入: " ans
来源：http://ve.asd995.cn

[R78] 交互式菜单
来源：http://tf.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gh.gzmigu.cn

[R79] 解析命令行选项
来源：http://wx.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ra.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://li.panjiajie.cn

time ./run.sh
来源：http://yy.9csxet.cn

================================================================================
来源：http://sj.9csxet.cn

S. C / C++ 专题
来源：http://vi.jianghongdianzi.cn

================================================================================
来源：http://zs.wgjwhj.cn

[S01] C：Hello World
来源：http://zg.shxzukj.cn

#include <stdio.h>
来源：http://kl.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://de.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://jl.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://sf.shxzskj.cn

[S03] C：读入整数
来源：http://rk.szxytkj.cn

int x; scanf("%d", &x);
来源：http://fu.bjjhwx.cn

[S04] C：字符串复制
来源：http://dz.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://va.szsharing.cn

[S05] C：字符串长度
来源：http://oh.wgjwhj.cn

strlen(s)
来源：http://kq.szsharing.cn

[S06] C：字符串比较
来源：http://wm.wgjwhj.cn

strcmp(a, b) == 0
来源：http://ya.9csxet.cn

[S07] C：数组遍历求和
来源：http://me.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dz.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://mu.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fa.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://kf.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ya.nicolike.cn

[S10] C：指针与解引用
来源：http://az.asd995.cn

int *p = &a;  *p = 5;
来源：http://jo.shtwfgs.cn

[S11] C：逐行读文件
来源：http://rb.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://px.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://si.gzmigu.cn

fclose(f);
来源：http://uf.panjiajie.cn

[S12] C：写文件
来源：http://xo.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qd.shtwfgs.cn

[S13] C：宏定义
来源：http://ni.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bb.nicolike.cn

[S14] C：枚举
来源：http://yt.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://kx.bookmarksfly.cn

[S15] C：类型转换
来源：http://pu.huixiangedu.cn

(double) a / b
来源：http://ar.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://iv.muxihuayi.cn

x |= (1 << 3);
来源：http://uq.nszjky.cn

[S17] C：安全拼接字符串
来源：http://pt.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dn.yuexingan06.cn

[S18] C：命令行参数
来源：http://od.shtwfgs.cn

int main(int argc, char **argv)
来源：http://mc.yuexingan06.cn

[S19] C：快速排序
来源：http://rk.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cu.wgjwhj.cn

[S20] C：二分查找
来源：http://zy.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://td.yuexingan06.cn

[S21] C：字符类别判断
来源：http://op.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jw.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://im.panjiajie.cn


<!-- 参考信息 -->