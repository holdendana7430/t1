代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://to.wgjwhj.cn

[Q54] 清空表
来源：http://hi.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://bo.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://we.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eo.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://zw.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rp.shxzskj.cn

[Q57] 行号
来源：http://gm.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qw.bjjhwx.cn

[Q58] 累计求和
来源：http://xm.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jw.nszjky.cn

[Q59] 分组内累计
来源：http://sd.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vk.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://ao.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zm.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ij.yuntaijiaju.cn

[Q61] 移动平均
来源：http://tr.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dc.huixinmuqiang.cn

[Q62] 分组占比
来源：http://to.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hq.huixiangedu.cn

[Q63] 开启事务
来源：http://wm.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tj.nicolike.cn

[Q64] 提交事务
来源：http://oq.wgjwhj.cn

COMMIT;
来源：http://ws.chemitech.net.cn

[Q65] 回滚事务
来源：http://wy.szsharing.cn

ROLLBACK;
来源：http://kq.wgjwhj.cn

[Q66] 行锁查询
来源：http://cr.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qy.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://gy.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yl.shxzskj.cn

[Q68] 保存点
来源：http://te.jctech888.com.cn

SAVEPOINT sp1;
来源：http://op.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://lo.9csxet.cn

[Q69] 查看执行计划
来源：http://cj.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lk.huixiangedu.cn

[Q70] 更新统计信息
来源：http://dr.yuexingan06.cn

ANALYZE TABLE users;
来源：http://tr.colortex.cn

[Q71] 查看建表语句
来源：http://lj.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eg.wgjwhj.cn

[Q72] 查看索引
来源：http://fz.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://cy.asd995.cn

[Q73] 查看表状态
来源：http://ez.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://za.wgjwhj.cn

[Q74] 强制使用索引
来源：http://rs.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jf.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://bo.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zg.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mj.521024.cn

[Q76] 按天统计
来源：http://am.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gl.nicolike.cn

[Q77] 时间加减
来源：http://vu.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://is.newstarts.cn

[Q78] 当前时间
来源：http://jo.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wt.chemitech.net.cn

[Q79] 字符串拼接
来源：http://ft.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ih.jctech888.com.cn

[Q80] 字符串截取
来源：http://ll.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vw.bookmarksfly.cn

[Q81] 字符串替换
来源：http://nc.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qk.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://xa.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rr.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://hs.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://is.shxzukj.cn

[Q84] 去除首尾空格
来源：http://lv.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://dr.asd995.cn

[Q85] 数值取整
来源：http://ck.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dj.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://rd.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ok.newstarts.cn

[Q87] JSON 字段做条件
来源：http://fe.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fz.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://gy.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yd.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xl.szxytkj.cn

[Q89] 判断表是否存在
来源：http://jw.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bt.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://fk.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fv.shxzskj.cn

================================================================================
来源：http://xc.gzmigu.cn

R. Bash 专题
来源：http://ic.yuntaijiaju.cn

================================================================================
来源：http://cu.nszjky.cn

[R01] shebang 与严格模式
来源：http://do.haigaiapp.cn

#!/usr/bin/env bash
来源：http://na.shtwfgs.cn

set -euo pipefail
来源：http://ln.9csxet.cn

[R02] 变量赋值与使用
来源：http://sz.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://ik.szxytkj.cn

[R03] 只读变量
来源：http://di.huixinmuqiang.cn

readonly PI=3.14
来源：http://fk.hnjuh.cn

[R04] 位置参数
来源：http://or.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://if.9csxet.cn

[R05] 参数默认值
来源：http://le.yuexingan06.cn

name="${1:-default}"
来源：http://rm.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://hz.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xb.shxzukj.cn

[R07] if 判断文件
来源：http://ek.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ak.huanxung.cn

[R08] 数值比较
来源：http://xn.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qo.nszjky.cn

[R09] 字符串比较
来源：http://ct.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mx.jianghongdianzi.cn

[R10] 正则匹配
来源：http://bd.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gv.yuexingan06.cn

[R11] case 多分支
来源：http://zr.colortex.cn

case "$1" in
来源：http://pb.521024.cn

start) echo "启动" ;;
来源：http://ua.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://wo.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://kc.chemitech.net.cn

esac
来源：http://wz.colortex.cn

[R12] for 遍历文件
来源：http://nl.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://ne.shtwfgs.cn

[R13] for 计数循环
来源：http://in.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://dn.panjiajie.cn

[R14] C 风格 for
来源：http://hi.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fj.szxytkj.cn

[R15] while 逐行读文件
来源：http://cl.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ql.shxzskj.cn

[R16] until 等待条件
来源：http://bv.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xg.szxytkj.cn

[R17] 数组定义与取值
来源：http://im.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://en.newstarts.cn

[R18] 遍历数组
来源：http://zj.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wl.jctech888.com.cn

[R19] 数组长度
来源：http://lo.nszjky.cn

echo "${#arr[@]}"
来源：http://vv.szxytkj.cn

[R20] 关联数组（字典）
来源：http://sl.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://py.szxytkj.cn

[R21] 字符串长度
来源：http://iy.asd995.cn

echo "${#s}"
来源：http://xz.shxzukj.cn

[R22] 截取子串
来源：http://mh.asd995.cn

echo "${s:0:5}"
来源：http://wq.gzmigu.cn

[R23] 字符串替换
来源：http://bo.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mj.gzmigu.cn

[R24] 大小写转换
来源：http://qe.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wz.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://tp.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zw.bjjhwx.cn

[R26] 命令替换
来源：http://bl.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://cx.szsharing.cn

[R27] 算术展开
来源：http://zp.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://pz.jianghongdianzi.cn

[R28] 浮点运算
来源：http://bg.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://gz.jctech888.com.cn

[R29] 定义函数
来源：http://pw.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lp.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://qs.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://hu.nicolike.cn

[R31] 局部变量
来源：http://hb.521024.cn

f() { local x=1; echo "$x"; }
来源：http://ql.gzmigu.cn

[R32] 参数个数校验
来源：http://ai.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rc.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://nh.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://br.wgjwhj.cn

[R34] 退出时清理
来源：http://wq.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kb.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://zq.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yz.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://xf.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pf.hnjuh.cn

[R37] 把输出赋给变量
来源：http://nw.hnjuh.cn

files=$(ls -1)
来源：http://uf.jianghongdianzi.cn

[R38] 管道串联
来源：http://aa.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://dj.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://ug.521024.cn

cmd > out.log 2>&1
来源：http://eu.shxzukj.cn

[R40] 追加写日志
来源：http://ti.colortex.cn

echo "log" >> out.log
来源：http://dc.newstarts.cn

[R41] 丢弃输出
来源：http://vn.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://lh.jianghongdianzi.cn

[R42] 输入重定向
来源：http://rt.huixiangedu.cn

wc -l < a.txt
来源：http://ij.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://xs.hnjuh.cn

find . -name "*.log" -type f
来源：http://rj.nszjky.cn

[R44] 按修改时间查找
来源：http://ud.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://jn.szxytkj.cn

[R45] 批量删除
来源：http://et.nicolike.cn

find . -name "*.tmp" -delete
来源：http://ib.nicolike.cn

[R46] 递归替换文件内容
来源：http://rp.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://el.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://yg.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dh.szsharing.cn

[R48] awk 取指定列
来源：http://nd.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://tt.gzmigu.cn

[R49] awk 带条件
来源：http://nt.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wo.huixiangedu.cn

[R50] awk 求和
来源：http://po.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ak.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://ml.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xn.hahajie.cn

[R52] 统计行数
来源：http://xw.szsharing.cn

wc -l a.txt
来源：http://tw.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ls.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lj.9csxet.cn

[R54] 比较两个文件
来源：http://oc.huixiangedu.cn

diff a.txt b.txt
来源：http://oj.gzmigu.cn

[R55] 压缩与解压
来源：http://ht.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ot.bookmarksfly.cn

[R56] 远程拷贝
来源：http://ae.yuntaijiaju.cn

scp file user@host:/path/
来源：http://xn.newstarts.cn

[R57] 远程执行命令
来源：http://kh.szsharing.cn

ssh user@host 'uptime'
来源：http://iw.panjiajie.cn

[R58] 下载文件
来源：http://qd.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wv.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://gq.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://od.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://ua.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ga.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://ec.yuexingan06.cn

df -h;  du -sh *
来源：http://tv.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://ly.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://xf.szsharing.cn

[R63] 内存与进程
来源：http://ue.asd995.cn

free -h;  ps aux | grep nginx
来源：http://mv.huanxung.cn

[R64] 结束进程
来源：http://sg.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://nr.lnxyls.cn

[R65] 查看端口占用
来源：http://so.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bv.shxzskj.cn

[R66] 定时任务
来源：http://ef.huanxung.cn

crontab -e;  crontab -l
来源：http://zb.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://qt.huixiangedu.cn

openssl rand -hex 16
来源：http://tk.huixiangedu.cn

[R68] 计算文件校验值
来源：http://lu.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nw.jctech888.com.cn

[R69] 生成随机密码
来源：http://ml.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://fx.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://al.521024.cn

date +%s;  date -d @1700000000
来源：http://dq.chemitech.net.cn

[R71] 日期格式化
来源：http://pq.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cl.muxihuayi.cn

[R72] 等待端口就绪
来源：http://cc.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uu.colortex.cn

[R73] 分割大日志
来源：http://mg.colortex.cn

split -l 1000 big.log part_
来源：http://xh.colortex.cn

[R74] 批量重命名
来源：http://jl.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wz.hnjuh.cn

[R75] 导出环境变量
来源：http://st.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://wi.shtwfgs.cn

[R76] 使用临时文件
来源：http://ya.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kk.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://pr.hnjuh.cn

read -rp "请输入: " ans
来源：http://ic.hnjuh.cn

[R78] 交互式菜单
来源：http://vp.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ha.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://de.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ei.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://nm.yuntaijiaju.cn

time ./run.sh
来源：http://uo.yuexingan06.cn

================================================================================
来源：http://qq.wgjwhj.cn

S. C / C++ 专题
来源：http://jo.nszjky.cn

================================================================================
来源：http://qz.521024.cn

[S01] C：Hello World
来源：http://nz.huixiangedu.cn

#include <stdio.h>
来源：http://dv.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ki.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://yf.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://sy.huixinmuqiang.cn

[S03] C：读入整数
来源：http://uf.colortex.cn

int x; scanf("%d", &x);
来源：http://px.huixiangedu.cn

[S04] C：字符串复制
来源：http://wd.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jv.huixiangedu.cn

[S05] C：字符串长度
来源：http://hh.panjiajie.cn

strlen(s)
来源：http://cp.shxzukj.cn

[S06] C：字符串比较
来源：http://wq.huixiangedu.cn

strcmp(a, b) == 0
来源：http://pr.colortex.cn

[S07] C：数组遍历求和
来源：http://mj.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ep.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://fo.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zy.colortex.cn

[S09] C：结构体定义与初始化
来源：http://ih.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pj.shxzukj.cn

[S10] C：指针与解引用
来源：http://un.asd995.cn

int *p = &a;  *p = 5;
来源：http://bx.haigaiapp.cn

[S11] C：逐行读文件
来源：http://vo.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://xi.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://no.szsharing.cn

fclose(f);
来源：http://ou.huixinmuqiang.cn

[S12] C：写文件
来源：http://fh.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gq.shxzskj.cn

[S13] C：宏定义
来源：http://tl.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yu.haigaiapp.cn

[S14] C：枚举
来源：http://bd.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://ie.newstarts.cn

[S15] C：类型转换
来源：http://jc.hnjuh.cn

(double) a / b
来源：http://nv.chemitech.net.cn

[S16] C：位操作置位
来源：http://xr.jctech888.com.cn

x |= (1 << 3);
来源：http://nr.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://mu.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tn.nszjky.cn

[S18] C：命令行参数
来源：http://jg.9csxet.cn

int main(int argc, char **argv)
来源：http://qr.shxzskj.cn

[S19] C：快速排序
来源：http://rh.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dt.wgjwhj.cn

[S20] C：二分查找
来源：http://wb.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ht.hnjuh.cn

[S21] C：字符类别判断
来源：http://mt.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uc.bjjhwx.cn

[S22] C：字符串转数字
来源：http://mn.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xs.bookmarksfly.cn

[S23] C：随机数
来源：http://qx.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sp.521024.cn

[S24] C：获取本地时间
来源：http://gu.bookmarksfly.cn


<!-- 参考信息 -->