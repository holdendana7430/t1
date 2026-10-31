代发 wailian999

[Q63] 开启事务
来源：http://qg.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nm.asd995.cn

[Q64] 提交事务
来源：http://hu.lnxyls.cn

COMMIT;
来源：http://fx.muxihuayi.cn

[Q65] 回滚事务
来源：http://vx.huixinmuqiang.cn

ROLLBACK;
来源：http://uc.bjjhwx.cn

[Q66] 行锁查询
来源：http://vo.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.asd995.cn

[Q67] 设置隔离级别
来源：http://jf.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://se.shtwfgs.cn

[Q68] 保存点
来源：http://tv.huixiangedu.cn

SAVEPOINT sp1;
来源：http://qj.521024.cn

ROLLBACK TO sp1;
来源：http://xd.colortex.cn

[Q69] 查看执行计划
来源：http://ii.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wx.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://xe.9csxet.cn

ANALYZE TABLE users;
来源：http://bg.panjiajie.cn

[Q71] 查看建表语句
来源：http://mp.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://re.huanxung.cn

[Q72] 查看索引
来源：http://qd.nszjky.cn

SHOW INDEX FROM users;
来源：http://dt.shxzskj.cn

[Q73] 查看表状态
来源：http://mb.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ph.haigaiapp.cn

[Q74] 强制使用索引
来源：http://ao.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hf.lnxyls.cn

[Q75] 日期格式化
来源：http://ku.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kt.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lp.chemitech.net.cn

[Q76] 按天统计
来源：http://lv.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gd.gzmigu.cn

[Q77] 时间加减
来源：http://su.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sm.asd995.cn

[Q78] 当前时间
来源：http://lw.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qs.jctech888.com.cn

[Q79] 字符串拼接
来源：http://zd.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ja.newstarts.cn

[Q80] 字符串截取
来源：http://cr.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://np.jctech888.com.cn

[Q81] 字符串替换
来源：http://uu.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hq.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://mh.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jo.bjjhwx.cn

[Q83] 大小写转换
来源：http://dp.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ok.hahajie.cn

[Q84] 去除首尾空格
来源：http://gv.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://wh.gzmigu.cn

[Q85] 数值取整
来源：http://df.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gc.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://sg.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fd.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://wh.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ns.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://xh.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cc.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xw.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://aj.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ot.szxytkj.cn

[Q90] 生成序号列
来源：http://st.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sj.szxytkj.cn

================================================================================
来源：http://ow.hnjuh.cn

R. Bash 专题
来源：http://mc.hahajie.cn

================================================================================
来源：http://yo.huanxung.cn

[R01] shebang 与严格模式
来源：http://yo.asd995.cn

#!/usr/bin/env bash
来源：http://ux.huanxung.cn

set -euo pipefail
来源：http://hb.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://rf.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://be.bookmarksfly.cn

[R03] 只读变量
来源：http://du.muxihuayi.cn

readonly PI=3.14
来源：http://hz.huanxung.cn

[R04] 位置参数
来源：http://hr.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pr.hahajie.cn

[R05] 参数默认值
来源：http://rc.shxzukj.cn

name="${1:-default}"
来源：http://qe.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://ds.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bk.shxzskj.cn

[R07] if 判断文件
来源：http://qc.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wc.9csxet.cn

[R08] 数值比较
来源：http://db.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://si.hahajie.cn

[R09] 字符串比较
来源：http://vi.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ea.muxihuayi.cn

[R10] 正则匹配
来源：http://sw.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mc.asd995.cn

[R11] case 多分支
来源：http://ro.chemitech.net.cn

case "$1" in
来源：http://zt.panjiajie.cn

start) echo "启动" ;;
来源：http://ua.gzmigu.cn

stop)  echo "停止" ;;
来源：http://gm.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://tm.asd995.cn

esac
来源：http://qw.haigaiapp.cn

[R12] for 遍历文件
来源：http://qw.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://fi.hnjuh.cn

[R13] for 计数循环
来源：http://zn.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://au.asd995.cn

[R14] C 风格 for
来源：http://he.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sz.wgjwhj.cn

[R15] while 逐行读文件
来源：http://xj.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gk.jctech888.com.cn

[R16] until 等待条件
来源：http://mg.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://si.jctech888.com.cn

[R17] 数组定义与取值
来源：http://cg.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lv.haigaiapp.cn

[R18] 遍历数组
来源：http://cn.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rc.haigaiapp.cn

[R19] 数组长度
来源：http://qr.nicolike.cn

echo "${#arr[@]}"
来源：http://ii.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://kp.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://un.hnjuh.cn

[R21] 字符串长度
来源：http://up.jctech888.com.cn

echo "${#s}"
来源：http://vz.shxzukj.cn

[R22] 截取子串
来源：http://ie.colortex.cn

echo "${s:0:5}"
来源：http://so.gzmigu.cn

[R23] 字符串替换
来源：http://bc.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tl.asd995.cn

[R24] 大小写转换
来源：http://hj.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cb.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://bs.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gh.haigaiapp.cn

[R26] 命令替换
来源：http://tp.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://nc.521024.cn

[R27] 算术展开
来源：http://pv.huanxung.cn

echo $((1 + 2 * 3))
来源：http://gm.asd995.cn

[R28] 浮点运算
来源：http://ke.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://sp.szxytkj.cn

[R29] 定义函数
来源：http://nd.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qi.colortex.cn

[R30] 函数返回状态码
来源：http://fe.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ts.szsharing.cn

[R31] 局部变量
来源：http://dx.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://km.bjjhwx.cn

[R32] 参数个数校验
来源：http://hx.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xz.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://oe.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bf.9csxet.cn

[R34] 退出时清理
来源：http://ec.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wl.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://zw.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gf.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://ox.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dv.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://gj.szxytkj.cn

files=$(ls -1)
来源：http://ev.colortex.cn

[R38] 管道串联
来源：http://nz.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://dn.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://eg.shxzukj.cn

cmd > out.log 2>&1
来源：http://ym.jianghongdianzi.cn

[R40] 追加写日志
来源：http://jr.newstarts.cn

echo "log" >> out.log
来源：http://yi.panjiajie.cn

[R41] 丢弃输出
来源：http://lp.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://pc.gzmigu.cn

[R42] 输入重定向
来源：http://ly.huanxung.cn

wc -l < a.txt
来源：http://cd.shtwfgs.cn

[R43] 按名字查找文件
来源：http://je.jctech888.com.cn

find . -name "*.log" -type f
来源：http://kb.521024.cn

[R44] 按修改时间查找
来源：http://iw.szxytkj.cn

find . -mtime -7 -type f
来源：http://cc.jctech888.com.cn

[R45] 批量删除
来源：http://ac.newstarts.cn

find . -name "*.tmp" -delete
来源：http://jj.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://gx.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vx.gzmigu.cn

[R47] sed 单行替换
来源：http://hq.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://px.szsharing.cn

[R48] awk 取指定列
来源：http://vu.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://ah.chemitech.net.cn

[R49] awk 带条件
来源：http://cx.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nm.yuntaijiaju.cn

[R50] awk 求和
来源：http://me.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zj.muxihuayi.cn

[R51] 排序去重取前几
来源：http://ee.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wd.huixiangedu.cn

[R52] 统计行数
来源：http://ig.colortex.cn

wc -l a.txt
来源：http://gy.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://ym.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bc.bjjhwx.cn

[R54] 比较两个文件
来源：http://dw.wgjwhj.cn

diff a.txt b.txt
来源：http://py.yuexingan06.cn

[R55] 压缩与解压
来源：http://gs.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vp.bjjhwx.cn

[R56] 远程拷贝
来源：http://ux.huanxung.cn

scp file user@host:/path/
来源：http://np.521024.cn

[R57] 远程执行命令
来源：http://mn.jctech888.com.cn

ssh user@host 'uptime'
来源：http://av.muxihuayi.cn

[R58] 下载文件
来源：http://cp.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nd.huixiangedu.cn

[R59] 发 POST JSON
来源：http://ds.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nn.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://wn.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sl.shxzukj.cn

[R61] 磁盘占用
来源：http://bd.shtwfgs.cn

df -h;  du -sh *
来源：http://pt.nicolike.cn

[R62] 找最占空间的文件
来源：http://kc.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://ma.yuexingan06.cn

[R63] 内存与进程
来源：http://nn.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://wr.yuntaijiaju.cn

[R64] 结束进程
来源：http://jr.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://ap.jctech888.com.cn

[R65] 查看端口占用
来源：http://wi.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mq.lnxyls.cn

[R66] 定时任务
来源：http://vu.haigaiapp.cn

crontab -e;  crontab -l
来源：http://ci.colortex.cn

[R67] 生成随机十六进制串
来源：http://er.bjjhwx.cn

openssl rand -hex 16
来源：http://bi.bjjhwx.cn

[R68] 计算文件校验值
来源：http://ai.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wk.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://tv.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://ki.haigaiapp.cn

[R70] 时间戳与互转
来源：http://ve.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://pt.chemitech.net.cn

[R71] 日期格式化
来源：http://wk.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bv.nicolike.cn

[R72] 等待端口就绪
来源：http://gx.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://of.newstarts.cn

[R73] 分割大日志
来源：http://hg.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://bn.asd995.cn

[R74] 批量重命名
来源：http://xl.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jc.bjjhwx.cn

[R75] 导出环境变量
来源：http://tm.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://sj.huixiangedu.cn

[R76] 使用临时文件
来源：http://uv.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ly.9csxet.cn

[R77] 读取用户输入
来源：http://hi.wgjwhj.cn

read -rp "请输入: " ans
来源：http://ib.jctech888.com.cn

[R78] 交互式菜单
来源：http://qg.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dt.lnxyls.cn

[R79] 解析命令行选项
来源：http://sv.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xu.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://ni.wgjwhj.cn

time ./run.sh
来源：http://qo.bjjhwx.cn

================================================================================
来源：http://jw.yuexingan06.cn

S. C / C++ 专题
来源：http://al.huixinmuqiang.cn

================================================================================
来源：http://od.nszjky.cn

[S01] C：Hello World
来源：http://tc.bookmarksfly.cn

#include <stdio.h>
来源：http://ww.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dp.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://qs.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://dm.panjiajie.cn

[S03] C：读入整数
来源：http://sh.panjiajie.cn

int x; scanf("%d", &x);
来源：http://mj.shxzskj.cn

[S04] C：字符串复制
来源：http://zi.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ex.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://nw.gzmigu.cn

strlen(s)
来源：http://ma.colortex.cn

[S06] C：字符串比较
来源：http://ou.shxzskj.cn

strcmp(a, b) == 0
来源：http://ps.panjiajie.cn

[S07] C：数组遍历求和
来源：http://br.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mv.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://zr.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bw.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://dd.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fd.shtwfgs.cn

[S10] C：指针与解引用
来源：http://at.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://nc.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://xz.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://mz.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://op.shxzukj.cn

fclose(f);
来源：http://sk.hahajie.cn

[S12] C：写文件
来源：http://ms.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://th.521024.cn

[S13] C：宏定义
来源：http://dq.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lg.521024.cn

[S14] C：枚举
来源：http://vk.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://mj.yuntaijiaju.cn

[S15] C：类型转换
来源：http://ab.haigaiapp.cn

(double) a / b
来源：http://ng.9csxet.cn

[S16] C：位操作置位
来源：http://ew.haigaiapp.cn

x |= (1 << 3);
来源：http://bq.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://aj.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bf.nszjky.cn

[S18] C：命令行参数
来源：http://cu.yuexingan06.cn

int main(int argc, char **argv)
来源：http://my.panjiajie.cn

[S19] C：快速排序
来源：http://cj.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dk.newstarts.cn

[S20] C：二分查找
来源：http://zh.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yo.shxzskj.cn

[S21] C：字符类别判断
来源：http://wk.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://am.nszjky.cn

[S22] C：字符串转数字
来源：http://ni.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nu.huixinmuqiang.cn

[S23] C：随机数
来源：http://ui.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vw.asd995.cn

[S24] C：获取本地时间
来源：http://np.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zo.huixiangedu.cn

[S25] C：内存拷贝
来源：http://lv.szxytkj.cn

memcpy(dst, src, n);
来源：http://ef.521024.cn

[S26] C：内存清零
来源：http://ve.nszjky.cn

memset(a, 0, sizeof a);
来源：http://ht.huanxung.cn

[S27] C：定义常量
来源：http://qx.nicolike.cn

const double PI = 3.14159;
来源：http://qg.yuntaijiaju.cn

[S28] C：静态变量
来源：http://nb.newstarts.cn

static int counter = 0;
来源：http://xm.shxzukj.cn

[S29] C：变参函数
来源：http://zy.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bt.shxzskj.cn

[S30] C：头文件保护
来源：http://fh.colortex.cn

#ifndef X_H
来源：http://zp.shtwfgs.cn

#define X_H
来源：http://wm.panjiajie.cn

#endif
来源：http://go.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://kv.szxytkj.cn

#include <iostream>
来源：http://ab.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://at.nszjky.cn

[S32] C++：字符串
来源：http://hb.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://ew.panjiajie.cn


<!-- 参考信息 -->