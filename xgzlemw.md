代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aa.szxytkj.cn

[Q50] 批量更新
来源：http://np.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xw.huanxung.cn

[Q51] 用子查询更新
来源：http://tw.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nk.521024.cn

[Q52] 删除指定行
来源：http://zn.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://lx.bjjhwx.cn

[Q53] 按条件删除
来源：http://op.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ep.shtwfgs.cn

[Q54] 清空表
来源：http://ya.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://gn.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://el.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://py.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://us.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ui.shtwfgs.cn

[Q57] 行号
来源：http://wf.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hc.jianghongdianzi.cn

[Q58] 累计求和
来源：http://xy.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xj.jctech888.com.cn

[Q59] 分组内累计
来源：http://yc.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sm.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://yr.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gy.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zc.lnxyls.cn

[Q61] 移动平均
来源：http://jo.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xa.muxihuayi.cn

[Q62] 分组占比
来源：http://zc.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wn.yuexingan06.cn

[Q63] 开启事务
来源：http://qh.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tz.521024.cn

[Q64] 提交事务
来源：http://oi.jianghongdianzi.cn

COMMIT;
来源：http://zi.colortex.cn

[Q65] 回滚事务
来源：http://ax.jianghongdianzi.cn

ROLLBACK;
来源：http://jf.gzmigu.cn

[Q66] 行锁查询
来源：http://yf.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vj.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://nq.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://id.lnxyls.cn

[Q68] 保存点
来源：http://er.bjjhwx.cn

SAVEPOINT sp1;
来源：http://up.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://cz.muxihuayi.cn

[Q69] 查看执行计划
来源：http://gh.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ct.asd995.cn

[Q70] 更新统计信息
来源：http://sc.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://ts.521024.cn

[Q71] 查看建表语句
来源：http://zj.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rd.asd995.cn

[Q72] 查看索引
来源：http://oo.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://am.jctech888.com.cn

[Q73] 查看表状态
来源：http://xq.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hs.szxytkj.cn

[Q74] 强制使用索引
来源：http://sg.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lo.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://zb.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zf.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cs.colortex.cn

[Q76] 按天统计
来源：http://rm.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lt.jianghongdianzi.cn

[Q77] 时间加减
来源：http://rf.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dm.bjjhwx.cn

[Q78] 当前时间
来源：http://jm.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mf.colortex.cn

[Q79] 字符串拼接
来源：http://js.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://op.bjjhwx.cn

[Q80] 字符串截取
来源：http://xb.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://si.asd995.cn

[Q81] 字符串替换
来源：http://da.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gr.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://yw.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://km.521024.cn

[Q83] 大小写转换
来源：http://as.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qc.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://ov.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://zj.gzmigu.cn

[Q85] 数值取整
来源：http://aq.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ia.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://ee.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ij.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://it.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xh.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://ei.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bw.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nq.panjiajie.cn

[Q89] 判断表是否存在
来源：http://yc.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wa.wgjwhj.cn

[Q90] 生成序号列
来源：http://zj.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://um.wgjwhj.cn

================================================================================
来源：http://ql.szxytkj.cn

R. Bash 专题
来源：http://fa.szxytkj.cn

================================================================================
来源：http://wk.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://zb.bjjhwx.cn

#!/usr/bin/env bash
来源：http://kv.huixiangedu.cn

set -euo pipefail
来源：http://ff.newstarts.cn

[R02] 变量赋值与使用
来源：http://yg.9csxet.cn

name="Tom"; echo "$name"
来源：http://pz.szsharing.cn

[R03] 只读变量
来源：http://ct.bjjhwx.cn

readonly PI=3.14
来源：http://mw.521024.cn

[R04] 位置参数
来源：http://go.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tf.yuexingan06.cn

[R05] 参数默认值
来源：http://ju.shxzukj.cn

name="${1:-default}"
来源：http://dk.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://ar.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://py.muxihuayi.cn

[R07] if 判断文件
来源：http://uo.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hi.panjiajie.cn

[R08] 数值比较
来源：http://xb.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ns.wgjwhj.cn

[R09] 字符串比较
来源：http://ud.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ri.asd995.cn

[R10] 正则匹配
来源：http://kl.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tl.szsharing.cn

[R11] case 多分支
来源：http://fr.bjjhwx.cn

case "$1" in
来源：http://mm.panjiajie.cn

start) echo "启动" ;;
来源：http://pq.hnjuh.cn

stop)  echo "停止" ;;
来源：http://sg.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://qq.521024.cn

esac
来源：http://td.newstarts.cn

[R12] for 遍历文件
来源：http://fe.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://bn.haigaiapp.cn

[R13] for 计数循环
来源：http://fb.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://xw.shxzukj.cn

[R14] C 风格 for
来源：http://hu.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ao.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://zw.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pi.asd995.cn

[R16] until 等待条件
来源：http://hp.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fe.gzmigu.cn

[R17] 数组定义与取值
来源：http://xf.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yg.hnjuh.cn

[R18] 遍历数组
来源：http://dp.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pd.lnxyls.cn

[R19] 数组长度
来源：http://jz.521024.cn

echo "${#arr[@]}"
来源：http://fq.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://nr.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ag.huixinmuqiang.cn

[R21] 字符串长度
来源：http://or.huanxung.cn

echo "${#s}"
来源：http://pf.szxytkj.cn

[R22] 截取子串
来源：http://sf.chemitech.net.cn

echo "${s:0:5}"
来源：http://lh.lnxyls.cn

[R23] 字符串替换
来源：http://fq.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ij.yuntaijiaju.cn

[R24] 大小写转换
来源：http://oy.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bs.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://dy.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bt.shxzukj.cn

[R26] 命令替换
来源：http://ba.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://rk.shtwfgs.cn

[R27] 算术展开
来源：http://gi.asd995.cn

echo $((1 + 2 * 3))
来源：http://sy.bjjhwx.cn

[R28] 浮点运算
来源：http://lb.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://ok.yuntaijiaju.cn

[R29] 定义函数
来源：http://qg.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yg.colortex.cn

[R30] 函数返回状态码
来源：http://zr.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://yo.hnjuh.cn

[R31] 局部变量
来源：http://ec.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://uf.shtwfgs.cn

[R32] 参数个数校验
来源：http://pp.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vd.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://pe.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ao.szsharing.cn

[R34] 退出时清理
来源：http://qo.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cg.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://gn.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jb.huanxung.cn

[R36] 并发执行多个任务
来源：http://mh.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ri.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://qz.huixinmuqiang.cn

files=$(ls -1)
来源：http://ja.newstarts.cn

[R38] 管道串联
来源：http://oq.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://jr.asd995.cn

[R39] 重定向标准输出与错误
来源：http://lv.bjjhwx.cn

cmd > out.log 2>&1
来源：http://jp.jianghongdianzi.cn

[R40] 追加写日志
来源：http://qa.521024.cn

echo "log" >> out.log
来源：http://nh.hnjuh.cn

[R41] 丢弃输出
来源：http://xo.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://fn.huanxung.cn

[R42] 输入重定向
来源：http://cn.hahajie.cn

wc -l < a.txt
来源：http://ck.yuexingan06.cn

[R43] 按名字查找文件
来源：http://jj.yuexingan06.cn

find . -name "*.log" -type f
来源：http://bf.nszjky.cn

[R44] 按修改时间查找
来源：http://wk.521024.cn

find . -mtime -7 -type f
来源：http://ev.lnxyls.cn

[R45] 批量删除
来源：http://tq.huanxung.cn

find . -name "*.tmp" -delete
来源：http://qn.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://vb.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lz.asd995.cn

[R47] sed 单行替换
来源：http://wh.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bb.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://uu.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://da.nszjky.cn

[R49] awk 带条件
来源：http://nj.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mw.huanxung.cn

[R50] awk 求和
来源：http://yd.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://an.bjjhwx.cn

[R51] 排序去重取前几
来源：http://hz.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xv.asd995.cn

[R52] 统计行数
来源：http://ep.szsharing.cn

wc -l a.txt
来源：http://ly.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://kx.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xv.chemitech.net.cn

[R54] 比较两个文件
来源：http://wt.szsharing.cn

diff a.txt b.txt
来源：http://mn.szxytkj.cn

[R55] 压缩与解压
来源：http://pu.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mk.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://tg.yuexingan06.cn

scp file user@host:/path/
来源：http://po.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://hi.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://ma.huixiangedu.cn

[R58] 下载文件
来源：http://nh.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vv.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://di.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fv.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://fh.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ah.newstarts.cn

[R61] 磁盘占用
来源：http://my.szxytkj.cn

df -h;  du -sh *
来源：http://nt.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://ac.asd995.cn

du -ah . | sort -rh | head -10
来源：http://qt.shxzukj.cn

[R63] 内存与进程
来源：http://xy.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://wt.asd995.cn

[R64] 结束进程
来源：http://qt.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://kn.bjjhwx.cn

[R65] 查看端口占用
来源：http://nt.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lp.colortex.cn

[R66] 定时任务
来源：http://tx.haigaiapp.cn

crontab -e;  crontab -l
来源：http://te.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://sw.shtwfgs.cn

openssl rand -hex 16
来源：http://tn.521024.cn

[R68] 计算文件校验值
来源：http://ac.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ha.colortex.cn

[R69] 生成随机密码
来源：http://od.521024.cn

head -c 16 /dev/urandom | base64
来源：http://es.asd995.cn

[R70] 时间戳与互转
来源：http://kk.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://mv.huixiangedu.cn

[R71] 日期格式化
来源：http://zf.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oq.hnjuh.cn

[R72] 等待端口就绪
来源：http://wz.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dt.hnjuh.cn

[R73] 分割大日志
来源：http://jf.chemitech.net.cn

split -l 1000 big.log part_
来源：http://fj.gzmigu.cn

[R74] 批量重命名
来源：http://zo.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xl.bjjhwx.cn

[R75] 导出环境变量
来源：http://og.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://ar.lnxyls.cn

[R76] 使用临时文件
来源：http://vq.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zg.yuexingan06.cn

[R77] 读取用户输入
来源：http://qn.yuexingan06.cn

read -rp "请输入: " ans
来源：http://wl.shxzskj.cn

[R78] 交互式菜单
来源：http://sr.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yg.bjjhwx.cn

[R79] 解析命令行选项
来源：http://zq.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yb.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://wk.panjiajie.cn

time ./run.sh
来源：http://xu.jctech888.com.cn

================================================================================
来源：http://uz.yuntaijiaju.cn

S. C / C++ 专题
来源：http://md.lnxyls.cn

================================================================================
来源：http://op.muxihuayi.cn

[S01] C：Hello World
来源：http://uf.jianghongdianzi.cn

#include <stdio.h>
来源：http://mm.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ue.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://gl.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://gz.nszjky.cn

[S03] C：读入整数
来源：http://jp.szxytkj.cn

int x; scanf("%d", &x);
来源：http://vq.chemitech.net.cn

[S04] C：字符串复制
来源：http://fk.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xl.bjjhwx.cn

[S05] C：字符串长度
来源：http://ie.huixinmuqiang.cn

strlen(s)
来源：http://iy.shxzukj.cn

[S06] C：字符串比较
来源：http://xe.asd995.cn

strcmp(a, b) == 0
来源：http://we.shxzskj.cn

[S07] C：数组遍历求和
来源：http://bm.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gd.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://zg.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iv.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://vi.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cw.huanxung.cn

[S10] C：指针与解引用
来源：http://ew.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://it.panjiajie.cn

[S11] C：逐行读文件
来源：http://jt.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://zz.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fz.szsharing.cn

fclose(f);
来源：http://tl.lnxyls.cn

[S12] C：写文件
来源：http://mm.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://im.shxzukj.cn

[S13] C：宏定义
来源：http://ve.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aw.huanxung.cn

[S14] C：枚举
来源：http://sx.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://go.yuntaijiaju.cn

[S15] C：类型转换
来源：http://qb.hnjuh.cn

(double) a / b
来源：http://yb.jctech888.com.cn

[S16] C：位操作置位
来源：http://jj.haigaiapp.cn

x |= (1 << 3);
来源：http://cy.521024.cn

[S17] C：安全拼接字符串
来源：http://te.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gx.colortex.cn

[S18] C：命令行参数
来源：http://kr.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://hg.yuntaijiaju.cn

[S19] C：快速排序
来源：http://tm.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fd.shxzukj.cn

[S20] C：二分查找
来源：http://bp.jianghongdianzi.cn


<!-- 参考信息 -->