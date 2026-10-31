代发 wailian999

[Q61] 移动平均
来源：http://vu.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zd.huixinmuqiang.cn

[Q62] 分组占比
来源：http://ob.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://go.gzmigu.cn

[Q63] 开启事务
来源：http://le.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zs.gzmigu.cn

[Q64] 提交事务
来源：http://yz.nicolike.cn

COMMIT;
来源：http://hg.colortex.cn

[Q65] 回滚事务
来源：http://bz.szsharing.cn

ROLLBACK;
来源：http://pq.shxzukj.cn

[Q66] 行锁查询
来源：http://hm.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jx.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://md.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iu.nszjky.cn

[Q68] 保存点
来源：http://hg.panjiajie.cn

SAVEPOINT sp1;
来源：http://pu.nszjky.cn

ROLLBACK TO sp1;
来源：http://kl.chemitech.net.cn

[Q69] 查看执行计划
来源：http://tm.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bk.huixiangedu.cn

[Q70] 更新统计信息
来源：http://mt.hnjuh.cn

ANALYZE TABLE users;
来源：http://fz.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://er.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rp.chemitech.net.cn

[Q72] 查看索引
来源：http://ig.szxytkj.cn

SHOW INDEX FROM users;
来源：http://km.bjjhwx.cn

[Q73] 查看表状态
来源：http://lu.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ja.asd995.cn

[Q74] 强制使用索引
来源：http://dc.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vq.muxihuayi.cn

[Q75] 日期格式化
来源：http://my.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ya.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gl.chemitech.net.cn

[Q76] 按天统计
来源：http://qz.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yc.szsharing.cn

[Q77] 时间加减
来源：http://on.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vv.yuexingan06.cn

[Q78] 当前时间
来源：http://zh.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://co.panjiajie.cn

[Q79] 字符串拼接
来源：http://th.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ac.panjiajie.cn

[Q80] 字符串截取
来源：http://wg.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ca.lnxyls.cn

[Q81] 字符串替换
来源：http://hu.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wh.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://vc.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wx.jctech888.com.cn

[Q83] 大小写转换
来源：http://pq.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zd.panjiajie.cn

[Q84] 去除首尾空格
来源：http://ks.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://ek.asd995.cn

[Q85] 数值取整
来源：http://dk.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pu.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://lq.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bk.szsharing.cn

[Q87] JSON 字段做条件
来源：http://ox.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xx.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://pi.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zq.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://by.521024.cn

[Q89] 判断表是否存在
来源：http://no.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jy.bjjhwx.cn

[Q90] 生成序号列
来源：http://ep.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qu.huixiangedu.cn

================================================================================
来源：http://vq.newstarts.cn

R. Bash 专题
来源：http://pj.lnxyls.cn

================================================================================
来源：http://oy.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://gu.hnjuh.cn

#!/usr/bin/env bash
来源：http://wu.shtwfgs.cn

set -euo pipefail
来源：http://db.szsharing.cn

[R02] 变量赋值与使用
来源：http://xh.hnjuh.cn

name="Tom"; echo "$name"
来源：http://pt.haigaiapp.cn

[R03] 只读变量
来源：http://wj.yuexingan06.cn

readonly PI=3.14
来源：http://td.9csxet.cn

[R04] 位置参数
来源：http://nk.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://be.huanxung.cn

[R05] 参数默认值
来源：http://kj.chemitech.net.cn

name="${1:-default}"
来源：http://rs.nszjky.cn

[R06] 判断命令是否存在
来源：http://hy.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jj.haigaiapp.cn

[R07] if 判断文件
来源：http://zv.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xi.haigaiapp.cn

[R08] 数值比较
来源：http://qk.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cp.shxzskj.cn

[R09] 字符串比较
来源：http://of.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hw.colortex.cn

[R10] 正则匹配
来源：http://ls.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pd.bjjhwx.cn

[R11] case 多分支
来源：http://qm.521024.cn

case "$1" in
来源：http://rr.nszjky.cn

start) echo "启动" ;;
来源：http://tw.szxytkj.cn

stop)  echo "停止" ;;
来源：http://nw.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://cb.9csxet.cn

esac
来源：http://di.gzmigu.cn

[R12] for 遍历文件
来源：http://ji.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://ks.jctech888.com.cn

[R13] for 计数循环
来源：http://zc.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://nz.newstarts.cn

[R14] C 风格 for
来源：http://gz.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jg.shtwfgs.cn

[R15] while 逐行读文件
来源：http://ms.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tx.bookmarksfly.cn

[R16] until 等待条件
来源：http://tw.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nd.szsharing.cn

[R17] 数组定义与取值
来源：http://kk.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vs.muxihuayi.cn

[R18] 遍历数组
来源：http://ri.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://id.haigaiapp.cn

[R19] 数组长度
来源：http://ju.bjjhwx.cn

echo "${#arr[@]}"
来源：http://nj.lnxyls.cn

[R20] 关联数组（字典）
来源：http://yn.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bv.chemitech.net.cn

[R21] 字符串长度
来源：http://nh.nszjky.cn

echo "${#s}"
来源：http://ca.shxzskj.cn

[R22] 截取子串
来源：http://wl.szsharing.cn

echo "${s:0:5}"
来源：http://ab.colortex.cn

[R23] 字符串替换
来源：http://fr.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vx.bjjhwx.cn

[R24] 大小写转换
来源：http://ax.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://if.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://wx.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bj.yuexingan06.cn

[R26] 命令替换
来源：http://oz.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://ph.bjjhwx.cn

[R27] 算术展开
来源：http://ha.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://mu.newstarts.cn

[R28] 浮点运算
来源：http://qi.521024.cn

echo "scale=2; 10/3" | bc
来源：http://ja.hnjuh.cn

[R29] 定义函数
来源：http://tv.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://er.muxihuayi.cn

[R30] 函数返回状态码
来源：http://vj.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://qg.jctech888.com.cn

[R31] 局部变量
来源：http://wu.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://vx.521024.cn

[R32] 参数个数校验
来源：http://oe.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jk.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://qe.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zb.wgjwhj.cn

[R34] 退出时清理
来源：http://yk.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nx.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://xl.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lc.lnxyls.cn

[R36] 并发执行多个任务
来源：http://qt.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ch.lnxyls.cn

[R37] 把输出赋给变量
来源：http://tv.shtwfgs.cn

files=$(ls -1)
来源：http://eu.nszjky.cn

[R38] 管道串联
来源：http://rf.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://jt.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://dy.shxzskj.cn

cmd > out.log 2>&1
来源：http://mo.521024.cn

[R40] 追加写日志
来源：http://rp.shxzskj.cn

echo "log" >> out.log
来源：http://tz.panjiajie.cn

[R41] 丢弃输出
来源：http://gj.nicolike.cn

cmd >/dev/null 2>&1
来源：http://lo.nszjky.cn

[R42] 输入重定向
来源：http://by.asd995.cn

wc -l < a.txt
来源：http://tl.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://hq.newstarts.cn

find . -name "*.log" -type f
来源：http://mz.jctech888.com.cn

[R44] 按修改时间查找
来源：http://jz.yuexingan06.cn

find . -mtime -7 -type f
来源：http://tq.lnxyls.cn

[R45] 批量删除
来源：http://ff.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://to.shxzskj.cn

[R46] 递归替换文件内容
来源：http://gl.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rq.panjiajie.cn

[R47] sed 单行替换
来源：http://xh.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hf.chemitech.net.cn

[R48] awk 取指定列
来源：http://ei.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://hr.lnxyls.cn

[R49] awk 带条件
来源：http://iw.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wd.shtwfgs.cn

[R50] awk 求和
来源：http://uk.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://od.jctech888.com.cn

[R51] 排序去重取前几
来源：http://ie.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ug.shxzukj.cn

[R52] 统计行数
来源：http://nv.huixiangedu.cn

wc -l a.txt
来源：http://ls.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://fl.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ua.huanxung.cn

[R54] 比较两个文件
来源：http://gn.huixiangedu.cn

diff a.txt b.txt
来源：http://ut.asd995.cn

[R55] 压缩与解压
来源：http://tn.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://je.shxzskj.cn

[R56] 远程拷贝
来源：http://tc.newstarts.cn

scp file user@host:/path/
来源：http://lh.chemitech.net.cn

[R57] 远程执行命令
来源：http://gs.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://ko.wgjwhj.cn

[R58] 下载文件
来源：http://pd.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fv.newstarts.cn

[R59] 发 POST JSON
来源：http://gv.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dm.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://lz.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://po.szsharing.cn

[R61] 磁盘占用
来源：http://xb.9csxet.cn

df -h;  du -sh *
来源：http://zp.lnxyls.cn

[R62] 找最占空间的文件
来源：http://au.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://pz.jctech888.com.cn

[R63] 内存与进程
来源：http://to.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://iq.shxzukj.cn

[R64] 结束进程
来源：http://yv.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://if.newstarts.cn

[R65] 查看端口占用
来源：http://gt.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sc.haigaiapp.cn

[R66] 定时任务
来源：http://pa.gzmigu.cn

crontab -e;  crontab -l
来源：http://uq.nszjky.cn

[R67] 生成随机十六进制串
来源：http://iw.newstarts.cn

openssl rand -hex 16
来源：http://gj.colortex.cn

[R68] 计算文件校验值
来源：http://iu.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wl.chemitech.net.cn

[R69] 生成随机密码
来源：http://ad.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://vs.jctech888.com.cn

[R70] 时间戳与互转
来源：http://xi.szsharing.cn

date +%s;  date -d @1700000000
来源：http://gb.huixinmuqiang.cn

[R71] 日期格式化
来源：http://av.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://et.szxytkj.cn

[R72] 等待端口就绪
来源：http://xu.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aj.szsharing.cn

[R73] 分割大日志
来源：http://dc.asd995.cn

split -l 1000 big.log part_
来源：http://mr.panjiajie.cn

[R74] 批量重命名
来源：http://tl.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://js.yuexingan06.cn

[R75] 导出环境变量
来源：http://ih.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://ik.chemitech.net.cn

[R76] 使用临时文件
来源：http://ps.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wd.colortex.cn

[R77] 读取用户输入
来源：http://tn.nszjky.cn

read -rp "请输入: " ans
来源：http://ms.panjiajie.cn

[R78] 交互式菜单
来源：http://dt.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fd.jctech888.com.cn

[R79] 解析命令行选项
来源：http://nq.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bk.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://vm.bjjhwx.cn

time ./run.sh
来源：http://vi.chemitech.net.cn

================================================================================
来源：http://vp.haigaiapp.cn

S. C / C++ 专题
来源：http://qe.chemitech.net.cn

================================================================================
来源：http://ac.nicolike.cn

[S01] C：Hello World
来源：http://nm.jctech888.com.cn

#include <stdio.h>
来源：http://kc.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gz.asd995.cn

[S02] C：变量与格式化输出
来源：http://mq.521024.cn

int a = 10; printf("%d\n", a);
来源：http://hn.9csxet.cn

[S03] C：读入整数
来源：http://dp.newstarts.cn

int x; scanf("%d", &x);
来源：http://cl.huanxung.cn

[S04] C：字符串复制
来源：http://wn.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lg.muxihuayi.cn

[S05] C：字符串长度
来源：http://nm.huixiangedu.cn

strlen(s)
来源：http://gj.asd995.cn

[S06] C：字符串比较
来源：http://gx.huanxung.cn

strcmp(a, b) == 0
来源：http://bj.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://by.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jg.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://gi.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sf.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://vy.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nh.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://dt.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://zy.szxytkj.cn

[S11] C：逐行读文件
来源：http://ii.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://kv.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ia.yuntaijiaju.cn

fclose(f);
来源：http://zc.szxytkj.cn

[S12] C：写文件
来源：http://md.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cc.panjiajie.cn

[S13] C：宏定义
来源：http://rs.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lf.panjiajie.cn

[S14] C：枚举
来源：http://an.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://lq.shtwfgs.cn

[S15] C：类型转换
来源：http://vu.shxzskj.cn

(double) a / b
来源：http://lf.huanxung.cn

[S16] C：位操作置位
来源：http://mk.asd995.cn

x |= (1 << 3);
来源：http://yg.hahajie.cn

[S17] C：安全拼接字符串
来源：http://xl.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qu.shxzskj.cn

[S18] C：命令行参数
来源：http://ep.nicolike.cn

int main(int argc, char **argv)
来源：http://ec.lnxyls.cn

[S19] C：快速排序
来源：http://mv.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oy.hahajie.cn

[S20] C：二分查找
来源：http://sd.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cp.asd995.cn

[S21] C：字符类别判断
来源：http://xi.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uc.yuexingan06.cn

[S22] C：字符串转数字
来源：http://cz.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yv.9csxet.cn

[S23] C：随机数
来源：http://zu.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vd.gzmigu.cn

[S24] C：获取本地时间
来源：http://dl.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sc.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://sk.hahajie.cn

memcpy(dst, src, n);
来源：http://na.muxihuayi.cn

[S26] C：内存清零
来源：http://px.521024.cn

memset(a, 0, sizeof a);
来源：http://xh.yuntaijiaju.cn

[S27] C：定义常量
来源：http://qv.yuexingan06.cn

const double PI = 3.14159;
来源：http://ed.521024.cn

[S28] C：静态变量
来源：http://da.asd995.cn

static int counter = 0;
来源：http://hu.bookmarksfly.cn

[S29] C：变参函数
来源：http://ga.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bm.newstarts.cn

[S30] C：头文件保护
来源：http://lj.huanxung.cn

#ifndef X_H
来源：http://jp.muxihuayi.cn

#define X_H
来源：http://jp.lnxyls.cn

#endif
来源：http://hs.lnxyls.cn

[S31] C++：Hello World
来源：http://ll.nszjky.cn


<!-- 参考信息 -->