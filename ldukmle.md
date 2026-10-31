代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gy.haigaiapp.cn

[Q58] 累计求和
来源：http://hc.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nf.haigaiapp.cn

[Q59] 分组内累计
来源：http://xx.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sj.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://sm.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rg.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://of.bookmarksfly.cn

[Q61] 移动平均
来源：http://gg.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jz.colortex.cn

[Q62] 分组占比
来源：http://lg.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hn.huixinmuqiang.cn

[Q63] 开启事务
来源：http://lq.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ib.nszjky.cn

[Q64] 提交事务
来源：http://cl.9csxet.cn

COMMIT;
来源：http://xq.bjjhwx.cn

[Q65] 回滚事务
来源：http://qj.jianghongdianzi.cn

ROLLBACK;
来源：http://tw.huanxung.cn

[Q66] 行锁查询
来源：http://km.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pi.nicolike.cn

[Q67] 设置隔离级别
来源：http://vx.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fe.haigaiapp.cn

[Q68] 保存点
来源：http://am.nicolike.cn

SAVEPOINT sp1;
来源：http://ms.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://bi.huanxung.cn

[Q69] 查看执行计划
来源：http://hz.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gz.521024.cn

[Q70] 更新统计信息
来源：http://iv.muxihuayi.cn

ANALYZE TABLE users;
来源：http://kr.colortex.cn

[Q71] 查看建表语句
来源：http://bx.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dx.nicolike.cn

[Q72] 查看索引
来源：http://kf.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://zo.shxzskj.cn

[Q73] 查看表状态
来源：http://vs.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tz.hahajie.cn

[Q74] 强制使用索引
来源：http://mf.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hu.bjjhwx.cn

[Q75] 日期格式化
来源：http://fe.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zn.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gc.szxytkj.cn

[Q76] 按天统计
来源：http://ao.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dj.jctech888.com.cn

[Q77] 时间加减
来源：http://us.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://he.huixinmuqiang.cn

[Q78] 当前时间
来源：http://gh.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jn.shtwfgs.cn

[Q79] 字符串拼接
来源：http://zz.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yb.szsharing.cn

[Q80] 字符串截取
来源：http://og.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ho.asd995.cn

[Q81] 字符串替换
来源：http://el.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ek.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://ye.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rq.hahajie.cn

[Q83] 大小写转换
来源：http://cj.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://or.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://an.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://ib.haigaiapp.cn

[Q85] 数值取整
来源：http://rc.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qt.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://au.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bi.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://no.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wv.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://zl.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vl.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mk.shxzskj.cn

[Q89] 判断表是否存在
来源：http://by.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aa.nszjky.cn

[Q90] 生成序号列
来源：http://gj.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vy.panjiajie.cn

================================================================================
来源：http://pg.hahajie.cn

R. Bash 专题
来源：http://ud.yuexingan06.cn

================================================================================
来源：http://ni.9csxet.cn

[R01] shebang 与严格模式
来源：http://qm.huixiangedu.cn

#!/usr/bin/env bash
来源：http://ps.szxytkj.cn

set -euo pipefail
来源：http://la.panjiajie.cn

[R02] 变量赋值与使用
来源：http://zx.shxzskj.cn

name="Tom"; echo "$name"
来源：http://lj.haigaiapp.cn

[R03] 只读变量
来源：http://mk.lnxyls.cn

readonly PI=3.14
来源：http://he.haigaiapp.cn

[R04] 位置参数
来源：http://ct.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hd.hnjuh.cn

[R05] 参数默认值
来源：http://vo.wgjwhj.cn

name="${1:-default}"
来源：http://fo.huanxung.cn

[R06] 判断命令是否存在
来源：http://yw.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vf.asd995.cn

[R07] if 判断文件
来源：http://od.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hn.szsharing.cn

[R08] 数值比较
来源：http://yc.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ap.shxzskj.cn

[R09] 字符串比较
来源：http://lh.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yq.521024.cn

[R10] 正则匹配
来源：http://fl.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xt.panjiajie.cn

[R11] case 多分支
来源：http://tv.huixiangedu.cn

case "$1" in
来源：http://ed.nicolike.cn

start) echo "启动" ;;
来源：http://my.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://qe.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://xv.huixinmuqiang.cn

esac
来源：http://bl.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://zs.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://nm.bookmarksfly.cn

[R13] for 计数循环
来源：http://uj.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://mn.chemitech.net.cn

[R14] C 风格 for
来源：http://ll.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xt.szsharing.cn

[R15] while 逐行读文件
来源：http://nn.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wn.jianghongdianzi.cn

[R16] until 等待条件
来源：http://qr.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hk.shxzukj.cn

[R17] 数组定义与取值
来源：http://lq.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cz.szxytkj.cn

[R18] 遍历数组
来源：http://qr.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xo.colortex.cn

[R19] 数组长度
来源：http://vr.gzmigu.cn

echo "${#arr[@]}"
来源：http://fy.shxzskj.cn

[R20] 关联数组（字典）
来源：http://cg.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://st.bookmarksfly.cn

[R21] 字符串长度
来源：http://hf.huixinmuqiang.cn

echo "${#s}"
来源：http://zz.nszjky.cn

[R22] 截取子串
来源：http://so.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://bj.nicolike.cn

[R23] 字符串替换
来源：http://vm.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ho.9csxet.cn

[R24] 大小写转换
来源：http://nt.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qq.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://oz.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pw.haigaiapp.cn

[R26] 命令替换
来源：http://fl.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://gu.muxihuayi.cn

[R27] 算术展开
来源：http://ce.huanxung.cn

echo $((1 + 2 * 3))
来源：http://sx.shtwfgs.cn

[R28] 浮点运算
来源：http://yj.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://nb.wgjwhj.cn

[R29] 定义函数
来源：http://cg.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zr.muxihuayi.cn

[R30] 函数返回状态码
来源：http://qd.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://yd.szxytkj.cn

[R31] 局部变量
来源：http://xu.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://fz.9csxet.cn

[R32] 参数个数校验
来源：http://gs.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ak.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://hb.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jj.lnxyls.cn

[R34] 退出时清理
来源：http://zf.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ri.hnjuh.cn

[R35] 后台执行并等待
来源：http://kh.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ls.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://ys.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://th.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://xl.hahajie.cn

files=$(ls -1)
来源：http://ng.nicolike.cn

[R38] 管道串联
来源：http://li.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://jj.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://kk.newstarts.cn

cmd > out.log 2>&1
来源：http://oe.huixinmuqiang.cn

[R40] 追加写日志
来源：http://bu.szxytkj.cn

echo "log" >> out.log
来源：http://vz.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://sq.huanxung.cn

cmd >/dev/null 2>&1
来源：http://te.nszjky.cn

[R42] 输入重定向
来源：http://fh.jctech888.com.cn

wc -l < a.txt
来源：http://xf.521024.cn

[R43] 按名字查找文件
来源：http://zk.nicolike.cn

find . -name "*.log" -type f
来源：http://cb.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://rw.yuexingan06.cn

find . -mtime -7 -type f
来源：http://mf.huanxung.cn

[R45] 批量删除
来源：http://qg.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://td.gzmigu.cn

[R46] 递归替换文件内容
来源：http://wz.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fi.hahajie.cn

[R47] sed 单行替换
来源：http://pl.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jq.newstarts.cn

[R48] awk 取指定列
来源：http://cr.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://ap.szxytkj.cn

[R49] awk 带条件
来源：http://fw.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zi.shxzukj.cn

[R50] awk 求和
来源：http://pd.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jo.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://mp.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dl.yuntaijiaju.cn

[R52] 统计行数
来源：http://ys.nszjky.cn

wc -l a.txt
来源：http://nk.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://vx.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kh.huixiangedu.cn

[R54] 比较两个文件
来源：http://de.colortex.cn

diff a.txt b.txt
来源：http://qt.lnxyls.cn

[R55] 压缩与解压
来源：http://gi.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://to.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://db.9csxet.cn

scp file user@host:/path/
来源：http://wk.9csxet.cn

[R57] 远程执行命令
来源：http://wz.bjjhwx.cn

ssh user@host 'uptime'
来源：http://zv.newstarts.cn

[R58] 下载文件
来源：http://np.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gh.jctech888.com.cn

[R59] 发 POST JSON
来源：http://op.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ci.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://xb.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qw.nszjky.cn

[R61] 磁盘占用
来源：http://rt.wgjwhj.cn

df -h;  du -sh *
来源：http://rq.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://bd.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://vk.lnxyls.cn

[R63] 内存与进程
来源：http://ee.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://hi.yuexingan06.cn

[R64] 结束进程
来源：http://ul.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://lx.huixiangedu.cn

[R65] 查看端口占用
来源：http://pr.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ac.bjjhwx.cn

[R66] 定时任务
来源：http://zg.bjjhwx.cn

crontab -e;  crontab -l
来源：http://vb.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://vc.lnxyls.cn

openssl rand -hex 16
来源：http://mv.szxytkj.cn

[R68] 计算文件校验值
来源：http://qy.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tx.jctech888.com.cn

[R69] 生成随机密码
来源：http://kg.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://hn.colortex.cn

[R70] 时间戳与互转
来源：http://yw.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://ma.huixiangedu.cn

[R71] 日期格式化
来源：http://lq.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wf.hahajie.cn

[R72] 等待端口就绪
来源：http://oa.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nh.huixiangedu.cn

[R73] 分割大日志
来源：http://so.huixiangedu.cn

split -l 1000 big.log part_
来源：http://dr.yuntaijiaju.cn

[R74] 批量重命名
来源：http://pa.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xy.gzmigu.cn

[R75] 导出环境变量
来源：http://fo.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://xx.szxytkj.cn

[R76] 使用临时文件
来源：http://ql.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ud.haigaiapp.cn

[R77] 读取用户输入
来源：http://qm.huixiangedu.cn

read -rp "请输入: " ans
来源：http://fs.yuexingan06.cn

[R78] 交互式菜单
来源：http://vm.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kl.panjiajie.cn

[R79] 解析命令行选项
来源：http://ml.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kt.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://ip.bookmarksfly.cn

time ./run.sh
来源：http://ov.jianghongdianzi.cn

================================================================================
来源：http://lc.panjiajie.cn

S. C / C++ 专题
来源：http://sy.jianghongdianzi.cn

================================================================================
来源：http://hw.521024.cn

[S01] C：Hello World
来源：http://xz.9csxet.cn

#include <stdio.h>
来源：http://by.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bo.nicolike.cn

[S02] C：变量与格式化输出
来源：http://jk.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://nk.huanxung.cn

[S03] C：读入整数
来源：http://hh.asd995.cn

int x; scanf("%d", &x);
来源：http://tg.gzmigu.cn

[S04] C：字符串复制
来源：http://yz.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nl.nicolike.cn

[S05] C：字符串长度
来源：http://gv.bookmarksfly.cn

strlen(s)
来源：http://at.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://gd.szsharing.cn

strcmp(a, b) == 0
来源：http://eh.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://wf.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qp.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://vh.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rb.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://fm.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tb.nszjky.cn

[S10] C：指针与解引用
来源：http://un.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://jp.haigaiapp.cn

[S11] C：逐行读文件
来源：http://gk.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://jz.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yp.521024.cn

fclose(f);
来源：http://nj.chemitech.net.cn

[S12] C：写文件
来源：http://iz.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qz.bjjhwx.cn

[S13] C：宏定义
来源：http://ov.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ho.huanxung.cn

[S14] C：枚举
来源：http://vu.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://df.szxytkj.cn

[S15] C：类型转换
来源：http://no.huanxung.cn

(double) a / b
来源：http://in.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://no.521024.cn

x |= (1 << 3);
来源：http://yg.521024.cn

[S17] C：安全拼接字符串
来源：http://ol.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hg.yuexingan06.cn

[S18] C：命令行参数
来源：http://od.szxytkj.cn

int main(int argc, char **argv)
来源：http://gr.jianghongdianzi.cn

[S19] C：快速排序
来源：http://ei.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vc.shxzskj.cn

[S20] C：二分查找
来源：http://pa.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://va.panjiajie.cn

[S21] C：字符类别判断
来源：http://jw.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oh.huixiangedu.cn

[S22] C：字符串转数字
来源：http://gq.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nm.nicolike.cn

[S23] C：随机数
来源：http://sp.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pp.shtwfgs.cn

[S24] C：获取本地时间
来源：http://rd.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://js.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://lv.hahajie.cn

memcpy(dst, src, n);
来源：http://mu.lnxyls.cn

[S26] C：内存清零
来源：http://ns.hahajie.cn

memset(a, 0, sizeof a);
来源：http://cq.haigaiapp.cn

[S27] C：定义常量
来源：http://bt.chemitech.net.cn

const double PI = 3.14159;
来源：http://yh.gzmigu.cn

[S28] C：静态变量
来源：http://bu.chemitech.net.cn


<!-- 参考信息 -->