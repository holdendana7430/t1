代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pm.jctech888.com.cn

[Q58] 累计求和
来源：http://sh.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qj.521024.cn

[Q59] 分组内累计
来源：http://tm.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://um.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://rq.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ky.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mb.lnxyls.cn

[Q61] 移动平均
来源：http://ac.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xn.bookmarksfly.cn

[Q62] 分组占比
来源：http://jk.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zx.yuntaijiaju.cn

[Q63] 开启事务
来源：http://zb.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fn.huixinmuqiang.cn

[Q64] 提交事务
来源：http://ig.chemitech.net.cn

COMMIT;
来源：http://bb.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://qb.yuntaijiaju.cn

ROLLBACK;
来源：http://gn.hnjuh.cn

[Q66] 行锁查询
来源：http://ca.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hy.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://qw.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ld.shtwfgs.cn

[Q68] 保存点
来源：http://px.colortex.cn

SAVEPOINT sp1;
来源：http://dw.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://oj.bjjhwx.cn

[Q69] 查看执行计划
来源：http://mf.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hg.shxzskj.cn

[Q70] 更新统计信息
来源：http://fn.chemitech.net.cn

ANALYZE TABLE users;
来源：http://sw.shtwfgs.cn

[Q71] 查看建表语句
来源：http://nm.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ue.wgjwhj.cn

[Q72] 查看索引
来源：http://vz.colortex.cn

SHOW INDEX FROM users;
来源：http://ql.nicolike.cn

[Q73] 查看表状态
来源：http://ig.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fu.newstarts.cn

[Q74] 强制使用索引
来源：http://gl.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ns.bjjhwx.cn

[Q75] 日期格式化
来源：http://qf.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mb.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qv.yuntaijiaju.cn

[Q76] 按天统计
来源：http://fk.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wk.panjiajie.cn

[Q77] 时间加减
来源：http://wh.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ln.9csxet.cn

[Q78] 当前时间
来源：http://fh.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gf.muxihuayi.cn

[Q79] 字符串拼接
来源：http://im.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dw.asd995.cn

[Q80] 字符串截取
来源：http://bv.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dm.jctech888.com.cn

[Q81] 字符串替换
来源：http://ds.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bs.521024.cn

[Q82] 字符长度与字节长度
来源：http://wj.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yo.huanxung.cn

[Q83] 大小写转换
来源：http://hh.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kq.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://aq.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://bg.bjjhwx.cn

[Q85] 数值取整
来源：http://yn.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://od.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://dj.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rf.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://as.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lv.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://nk.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://om.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ar.colortex.cn

[Q89] 判断表是否存在
来源：http://pc.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://km.bjjhwx.cn

[Q90] 生成序号列
来源：http://gt.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gu.nicolike.cn

================================================================================
来源：http://yi.huixiangedu.cn

R. Bash 专题
来源：http://lx.jianghongdianzi.cn

================================================================================
来源：http://kr.lnxyls.cn

[R01] shebang 与严格模式
来源：http://vw.wgjwhj.cn

#!/usr/bin/env bash
来源：http://xl.muxihuayi.cn

set -euo pipefail
来源：http://yk.newstarts.cn

[R02] 变量赋值与使用
来源：http://mi.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://uj.huixiangedu.cn

[R03] 只读变量
来源：http://kb.9csxet.cn

readonly PI=3.14
来源：http://vz.huixinmuqiang.cn

[R04] 位置参数
来源：http://xu.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ef.newstarts.cn

[R05] 参数默认值
来源：http://kl.shxzskj.cn

name="${1:-default}"
来源：http://qa.hahajie.cn

[R06] 判断命令是否存在
来源：http://kk.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sw.9csxet.cn

[R07] if 判断文件
来源：http://oi.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lb.nszjky.cn

[R08] 数值比较
来源：http://hq.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zb.colortex.cn

[R09] 字符串比较
来源：http://oi.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nn.yuntaijiaju.cn

[R10] 正则匹配
来源：http://cd.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ux.huanxung.cn

[R11] case 多分支
来源：http://pa.hahajie.cn

case "$1" in
来源：http://ji.shxzskj.cn

start) echo "启动" ;;
来源：http://ab.asd995.cn

stop)  echo "停止" ;;
来源：http://kq.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://jv.huixiangedu.cn

esac
来源：http://po.panjiajie.cn

[R12] for 遍历文件
来源：http://mi.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://zi.nicolike.cn

[R13] for 计数循环
来源：http://im.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://my.muxihuayi.cn

[R14] C 风格 for
来源：http://rk.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iw.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://lq.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pv.521024.cn

[R16] until 等待条件
来源：http://vu.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ns.szxytkj.cn

[R17] 数组定义与取值
来源：http://lh.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ej.yuexingan06.cn

[R18] 遍历数组
来源：http://lp.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cu.jctech888.com.cn

[R19] 数组长度
来源：http://nw.haigaiapp.cn

echo "${#arr[@]}"
来源：http://dr.szsharing.cn

[R20] 关联数组（字典）
来源：http://wc.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wf.szsharing.cn

[R21] 字符串长度
来源：http://pi.asd995.cn

echo "${#s}"
来源：http://ym.lnxyls.cn

[R22] 截取子串
来源：http://vm.jctech888.com.cn

echo "${s:0:5}"
来源：http://la.szxytkj.cn

[R23] 字符串替换
来源：http://xw.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pf.9csxet.cn

[R24] 大小写转换
来源：http://jv.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nx.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://hk.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ra.haigaiapp.cn

[R26] 命令替换
来源：http://xu.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://wx.haigaiapp.cn

[R27] 算术展开
来源：http://fi.hahajie.cn

echo $((1 + 2 * 3))
来源：http://rv.shtwfgs.cn

[R28] 浮点运算
来源：http://kr.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://de.hahajie.cn

[R29] 定义函数
来源：http://pl.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://al.shxzukj.cn

[R30] 函数返回状态码
来源：http://kj.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://wz.gzmigu.cn

[R31] 局部变量
来源：http://dc.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://th.9csxet.cn

[R32] 参数个数校验
来源：http://eq.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ix.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://ck.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mx.chemitech.net.cn

[R34] 退出时清理
来源：http://sm.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ok.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://oo.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rd.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://rp.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ul.asd995.cn

[R37] 把输出赋给变量
来源：http://yf.szxytkj.cn

files=$(ls -1)
来源：http://sa.newstarts.cn

[R38] 管道串联
来源：http://gt.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://ef.colortex.cn

[R39] 重定向标准输出与错误
来源：http://vc.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://rj.haigaiapp.cn

[R40] 追加写日志
来源：http://lb.521024.cn

echo "log" >> out.log
来源：http://jo.chemitech.net.cn

[R41] 丢弃输出
来源：http://oz.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://xc.shxzskj.cn

[R42] 输入重定向
来源：http://cf.panjiajie.cn

wc -l < a.txt
来源：http://ji.shtwfgs.cn

[R43] 按名字查找文件
来源：http://hz.shxzukj.cn

find . -name "*.log" -type f
来源：http://rd.huanxung.cn

[R44] 按修改时间查找
来源：http://ly.colortex.cn

find . -mtime -7 -type f
来源：http://kv.newstarts.cn

[R45] 批量删除
来源：http://cm.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://bp.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://zf.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hx.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://iw.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yw.nszjky.cn

[R48] awk 取指定列
来源：http://ft.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://lr.haigaiapp.cn

[R49] awk 带条件
来源：http://ev.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gx.hahajie.cn

[R50] awk 求和
来源：http://kw.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sr.gzmigu.cn

[R51] 排序去重取前几
来源：http://ty.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qq.lnxyls.cn

[R52] 统计行数
来源：http://qr.szxytkj.cn

wc -l a.txt
来源：http://mp.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://fu.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qk.haigaiapp.cn

[R54] 比较两个文件
来源：http://iv.jctech888.com.cn

diff a.txt b.txt
来源：http://wx.jctech888.com.cn

[R55] 压缩与解压
来源：http://rt.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fw.haigaiapp.cn

[R56] 远程拷贝
来源：http://za.521024.cn

scp file user@host:/path/
来源：http://va.panjiajie.cn

[R57] 远程执行命令
来源：http://pn.nszjky.cn

ssh user@host 'uptime'
来源：http://kw.huixinmuqiang.cn

[R58] 下载文件
来源：http://fr.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bc.haigaiapp.cn

[R59] 发 POST JSON
来源：http://lj.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qn.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://rq.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ba.huanxung.cn

[R61] 磁盘占用
来源：http://hw.jctech888.com.cn

df -h;  du -sh *
来源：http://lb.shxzskj.cn

[R62] 找最占空间的文件
来源：http://gr.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://re.huixiangedu.cn

[R63] 内存与进程
来源：http://bu.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://tt.lnxyls.cn

[R64] 结束进程
来源：http://jb.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://tc.bookmarksfly.cn

[R65] 查看端口占用
来源：http://kd.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://en.bookmarksfly.cn

[R66] 定时任务
来源：http://al.hahajie.cn

crontab -e;  crontab -l
来源：http://qp.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://dv.jianghongdianzi.cn

openssl rand -hex 16
来源：http://jy.chemitech.net.cn

[R68] 计算文件校验值
来源：http://hf.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ur.shxzukj.cn

[R69] 生成随机密码
来源：http://rq.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://zo.newstarts.cn

[R70] 时间戳与互转
来源：http://wr.nszjky.cn

date +%s;  date -d @1700000000
来源：http://cf.haigaiapp.cn

[R71] 日期格式化
来源：http://ln.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oo.haigaiapp.cn

[R72] 等待端口就绪
来源：http://ss.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rn.huixiangedu.cn

[R73] 分割大日志
来源：http://pt.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://sv.huixinmuqiang.cn

[R74] 批量重命名
来源：http://wg.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bz.chemitech.net.cn

[R75] 导出环境变量
来源：http://gm.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://cg.panjiajie.cn

[R76] 使用临时文件
来源：http://oh.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pt.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://wy.chemitech.net.cn

read -rp "请输入: " ans
来源：http://yt.lnxyls.cn

[R78] 交互式菜单
来源：http://rl.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sv.asd995.cn

[R79] 解析命令行选项
来源：http://qs.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mk.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://ua.shtwfgs.cn

time ./run.sh
来源：http://sz.hahajie.cn

================================================================================
来源：http://ta.yuntaijiaju.cn

S. C / C++ 专题
来源：http://ou.szxytkj.cn

================================================================================
来源：http://fc.bookmarksfly.cn

[S01] C：Hello World
来源：http://ak.nszjky.cn

#include <stdio.h>
来源：http://aj.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ki.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://aw.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://zd.521024.cn

[S03] C：读入整数
来源：http://ca.lnxyls.cn

int x; scanf("%d", &x);
来源：http://hp.bookmarksfly.cn

[S04] C：字符串复制
来源：http://wm.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qt.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://rr.hahajie.cn

strlen(s)
来源：http://ne.shxzukj.cn

[S06] C：字符串比较
来源：http://eq.shxzskj.cn

strcmp(a, b) == 0
来源：http://by.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://ox.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rx.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://to.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qk.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://rc.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pa.yuexingan06.cn

[S10] C：指针与解引用
来源：http://as.asd995.cn

int *p = &a;  *p = 5;
来源：http://ki.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://uc.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://mo.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lf.wgjwhj.cn

fclose(f);
来源：http://zw.nicolike.cn

[S12] C：写文件
来源：http://le.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ro.bjjhwx.cn

[S13] C：宏定义
来源：http://xb.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cz.szxytkj.cn

[S14] C：枚举
来源：http://xd.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://yf.jctech888.com.cn

[S15] C：类型转换
来源：http://yk.shtwfgs.cn

(double) a / b
来源：http://hg.szxytkj.cn

[S16] C：位操作置位
来源：http://dq.lnxyls.cn

x |= (1 << 3);
来源：http://ue.newstarts.cn

[S17] C：安全拼接字符串
来源：http://qc.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xf.wgjwhj.cn

[S18] C：命令行参数
来源：http://om.bjjhwx.cn

int main(int argc, char **argv)
来源：http://lp.szsharing.cn

[S19] C：快速排序
来源：http://on.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zl.bookmarksfly.cn

[S20] C：二分查找
来源：http://tl.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aw.chemitech.net.cn

[S21] C：字符类别判断
来源：http://ix.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jm.huixiangedu.cn

[S22] C：字符串转数字
来源：http://wz.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sd.hahajie.cn

[S23] C：随机数
来源：http://ln.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://to.shxzukj.cn

[S24] C：获取本地时间
来源：http://mm.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rk.chemitech.net.cn

[S25] C：内存拷贝
来源：http://yd.asd995.cn

memcpy(dst, src, n);
来源：http://mc.gzmigu.cn

[S26] C：内存清零
来源：http://ql.szsharing.cn

memset(a, 0, sizeof a);
来源：http://im.colortex.cn

[S27] C：定义常量
来源：http://vr.bjjhwx.cn

const double PI = 3.14159;
来源：http://mf.yuntaijiaju.cn

[S28] C：静态变量
来源：http://nz.huanxung.cn


<!-- 参考信息 -->