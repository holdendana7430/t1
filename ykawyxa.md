代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fb.szsharing.cn

[Q58] 累计求和
来源：http://yd.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vf.newstarts.cn

[Q59] 分组内累计
来源：http://tr.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tu.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://xk.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vd.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ug.nszjky.cn

[Q61] 移动平均
来源：http://sm.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zg.wgjwhj.cn

[Q62] 分组占比
来源：http://jd.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mw.nicolike.cn

[Q63] 开启事务
来源：http://tq.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://if.wgjwhj.cn

[Q64] 提交事务
来源：http://yp.521024.cn

COMMIT;
来源：http://bx.wgjwhj.cn

[Q65] 回滚事务
来源：http://rn.colortex.cn

ROLLBACK;
来源：http://qs.hahajie.cn

[Q66] 行锁查询
来源：http://hv.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tb.szsharing.cn

[Q67] 设置隔离级别
来源：http://fe.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qg.colortex.cn

[Q68] 保存点
来源：http://yx.huanxung.cn

SAVEPOINT sp1;
来源：http://zc.szsharing.cn

ROLLBACK TO sp1;
来源：http://wo.huixiangedu.cn

[Q69] 查看执行计划
来源：http://pa.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wp.asd995.cn

[Q70] 更新统计信息
来源：http://vb.panjiajie.cn

ANALYZE TABLE users;
来源：http://ax.nszjky.cn

[Q71] 查看建表语句
来源：http://se.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wk.panjiajie.cn

[Q72] 查看索引
来源：http://oe.521024.cn

SHOW INDEX FROM users;
来源：http://cx.shtwfgs.cn

[Q73] 查看表状态
来源：http://kw.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://py.chemitech.net.cn

[Q74] 强制使用索引
来源：http://rc.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sk.asd995.cn

[Q75] 日期格式化
来源：http://zi.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ho.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zl.jianghongdianzi.cn

[Q76] 按天统计
来源：http://tf.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://le.wgjwhj.cn

[Q77] 时间加减
来源：http://mc.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tq.colortex.cn

[Q78] 当前时间
来源：http://dx.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oo.bjjhwx.cn

[Q79] 字符串拼接
来源：http://cr.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ue.szxytkj.cn

[Q80] 字符串截取
来源：http://cl.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://up.jctech888.com.cn

[Q81] 字符串替换
来源：http://uk.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oi.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://wl.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hu.lnxyls.cn

[Q83] 大小写转换
来源：http://yw.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zr.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://mi.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://mp.521024.cn

[Q85] 数值取整
来源：http://dm.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ro.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://qs.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ox.szsharing.cn

[Q87] JSON 字段做条件
来源：http://km.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xc.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://pc.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fl.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ve.shxzskj.cn

[Q89] 判断表是否存在
来源：http://ke.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jm.jctech888.com.cn

[Q90] 生成序号列
来源：http://kr.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nd.panjiajie.cn

================================================================================
来源：http://yj.bjjhwx.cn

R. Bash 专题
来源：http://fy.newstarts.cn

================================================================================
来源：http://qv.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://wl.9csxet.cn

#!/usr/bin/env bash
来源：http://yk.szsharing.cn

set -euo pipefail
来源：http://yf.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://pk.9csxet.cn

name="Tom"; echo "$name"
来源：http://tv.panjiajie.cn

[R03] 只读变量
来源：http://zm.panjiajie.cn

readonly PI=3.14
来源：http://kv.shtwfgs.cn

[R04] 位置参数
来源：http://ss.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ol.hnjuh.cn

[R05] 参数默认值
来源：http://wt.9csxet.cn

name="${1:-default}"
来源：http://uz.colortex.cn

[R06] 判断命令是否存在
来源：http://aq.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vq.9csxet.cn

[R07] if 判断文件
来源：http://dg.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eo.panjiajie.cn

[R08] 数值比较
来源：http://bp.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jw.shtwfgs.cn

[R09] 字符串比较
来源：http://uf.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fq.colortex.cn

[R10] 正则匹配
来源：http://tc.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wx.panjiajie.cn

[R11] case 多分支
来源：http://lz.bookmarksfly.cn

case "$1" in
来源：http://cu.shxzskj.cn

start) echo "启动" ;;
来源：http://hc.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://fg.colortex.cn

*)     echo "未知命令" ;;
来源：http://fe.szxytkj.cn

esac
来源：http://kr.jctech888.com.cn

[R12] for 遍历文件
来源：http://gm.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://dp.muxihuayi.cn

[R13] for 计数循环
来源：http://zx.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://rn.huixinmuqiang.cn

[R14] C 风格 for
来源：http://tl.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mk.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://pw.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://af.521024.cn

[R16] until 等待条件
来源：http://bc.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wd.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://bw.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ov.hahajie.cn

[R18] 遍历数组
来源：http://sa.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oz.bjjhwx.cn

[R19] 数组长度
来源：http://ym.newstarts.cn

echo "${#arr[@]}"
来源：http://uh.9csxet.cn

[R20] 关联数组（字典）
来源：http://gr.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xl.shxzukj.cn

[R21] 字符串长度
来源：http://kp.nicolike.cn

echo "${#s}"
来源：http://oj.chemitech.net.cn

[R22] 截取子串
来源：http://es.newstarts.cn

echo "${s:0:5}"
来源：http://tp.9csxet.cn

[R23] 字符串替换
来源：http://do.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eq.yuntaijiaju.cn

[R24] 大小写转换
来源：http://ob.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yx.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://il.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hi.nszjky.cn

[R26] 命令替换
来源：http://zy.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://er.szsharing.cn

[R27] 算术展开
来源：http://bp.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://dc.9csxet.cn

[R28] 浮点运算
来源：http://pb.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://yq.521024.cn

[R29] 定义函数
来源：http://ob.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nt.muxihuayi.cn

[R30] 函数返回状态码
来源：http://xv.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://jt.huixiangedu.cn

[R31] 局部变量
来源：http://bn.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://eh.colortex.cn

[R32] 参数个数校验
来源：http://ns.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uu.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://rt.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jf.shxzskj.cn

[R34] 退出时清理
来源：http://ka.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gx.lnxyls.cn

[R35] 后台执行并等待
来源：http://tv.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xe.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://dc.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xh.asd995.cn

[R37] 把输出赋给变量
来源：http://en.hnjuh.cn

files=$(ls -1)
来源：http://bo.shtwfgs.cn

[R38] 管道串联
来源：http://ax.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://fd.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://sm.lnxyls.cn

cmd > out.log 2>&1
来源：http://ui.wgjwhj.cn

[R40] 追加写日志
来源：http://qr.yuexingan06.cn

echo "log" >> out.log
来源：http://dl.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://by.nszjky.cn

cmd >/dev/null 2>&1
来源：http://pa.shtwfgs.cn

[R42] 输入重定向
来源：http://ll.haigaiapp.cn

wc -l < a.txt
来源：http://pa.huixiangedu.cn

[R43] 按名字查找文件
来源：http://wf.shxzukj.cn

find . -name "*.log" -type f
来源：http://rl.521024.cn

[R44] 按修改时间查找
来源：http://yz.panjiajie.cn

find . -mtime -7 -type f
来源：http://we.hahajie.cn

[R45] 批量删除
来源：http://xs.huanxung.cn

find . -name "*.tmp" -delete
来源：http://kf.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://nb.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lj.chemitech.net.cn

[R47] sed 单行替换
来源：http://vq.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ex.9csxet.cn

[R48] awk 取指定列
来源：http://ng.521024.cn

awk '{print $1, $3}' a.txt
来源：http://fb.nicolike.cn

[R49] awk 带条件
来源：http://hb.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ej.asd995.cn

[R50] awk 求和
来源：http://sg.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cf.huixiangedu.cn

[R51] 排序去重取前几
来源：http://wi.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gl.yuexingan06.cn

[R52] 统计行数
来源：http://xb.jianghongdianzi.cn

wc -l a.txt
来源：http://fs.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://zl.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://np.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://rb.chemitech.net.cn

diff a.txt b.txt
来源：http://ei.muxihuayi.cn

[R55] 压缩与解压
来源：http://cm.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://of.jctech888.com.cn

[R56] 远程拷贝
来源：http://gk.muxihuayi.cn

scp file user@host:/path/
来源：http://js.szxytkj.cn

[R57] 远程执行命令
来源：http://qs.wgjwhj.cn

ssh user@host 'uptime'
来源：http://tk.newstarts.cn

[R58] 下载文件
来源：http://ic.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cd.haigaiapp.cn

[R59] 发 POST JSON
来源：http://kv.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yz.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://vm.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wd.colortex.cn

[R61] 磁盘占用
来源：http://hd.chemitech.net.cn

df -h;  du -sh *
来源：http://dv.gzmigu.cn

[R62] 找最占空间的文件
来源：http://ye.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://rc.521024.cn

[R63] 内存与进程
来源：http://vv.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://kh.haigaiapp.cn

[R64] 结束进程
来源：http://ta.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://im.yuexingan06.cn

[R65] 查看端口占用
来源：http://lj.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rl.lnxyls.cn

[R66] 定时任务
来源：http://tl.shxzukj.cn

crontab -e;  crontab -l
来源：http://ab.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://jm.nicolike.cn

openssl rand -hex 16
来源：http://xw.wgjwhj.cn

[R68] 计算文件校验值
来源：http://zq.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uh.asd995.cn

[R69] 生成随机密码
来源：http://lb.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://pu.shxzskj.cn

[R70] 时间戳与互转
来源：http://mo.nszjky.cn

date +%s;  date -d @1700000000
来源：http://zm.newstarts.cn

[R71] 日期格式化
来源：http://nd.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rf.szsharing.cn

[R72] 等待端口就绪
来源：http://bp.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mg.shxzukj.cn

[R73] 分割大日志
来源：http://ke.asd995.cn

split -l 1000 big.log part_
来源：http://jv.gzmigu.cn

[R74] 批量重命名
来源：http://nt.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://us.nicolike.cn

[R75] 导出环境变量
来源：http://xh.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://mr.bookmarksfly.cn

[R76] 使用临时文件
来源：http://vn.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yu.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://dp.shtwfgs.cn

read -rp "请输入: " ans
来源：http://jb.nszjky.cn

[R78] 交互式菜单
来源：http://fv.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ls.yuexingan06.cn

[R79] 解析命令行选项
来源：http://wb.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hm.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://af.shxzskj.cn

time ./run.sh
来源：http://fr.chemitech.net.cn

================================================================================
来源：http://yk.wgjwhj.cn

S. C / C++ 专题
来源：http://ig.521024.cn

================================================================================
来源：http://eo.huanxung.cn

[S01] C：Hello World
来源：http://rz.nicolike.cn

#include <stdio.h>
来源：http://uv.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nj.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://hd.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://po.szsharing.cn

[S03] C：读入整数
来源：http://vn.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://gc.lnxyls.cn

[S04] C：字符串复制
来源：http://is.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pu.newstarts.cn

[S05] C：字符串长度
来源：http://nq.huixinmuqiang.cn

strlen(s)
来源：http://yc.huanxung.cn

[S06] C：字符串比较
来源：http://ht.jctech888.com.cn

strcmp(a, b) == 0
来源：http://ym.newstarts.cn

[S07] C：数组遍历求和
来源：http://xk.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wu.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://pr.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ec.521024.cn

[S09] C：结构体定义与初始化
来源：http://xp.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zu.chemitech.net.cn

[S10] C：指针与解引用
来源：http://vp.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://vo.szsharing.cn

[S11] C：逐行读文件
来源：http://kf.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://ea.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ka.jianghongdianzi.cn

fclose(f);
来源：http://uz.hnjuh.cn

[S12] C：写文件
来源：http://xx.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ph.haigaiapp.cn

[S13] C：宏定义
来源：http://dq.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ll.asd995.cn

[S14] C：枚举
来源：http://fy.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://th.yuntaijiaju.cn

[S15] C：类型转换
来源：http://qc.huanxung.cn

(double) a / b
来源：http://tl.wgjwhj.cn

[S16] C：位操作置位
来源：http://vi.hahajie.cn

x |= (1 << 3);
来源：http://bb.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://hk.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sh.bjjhwx.cn

[S18] C：命令行参数
来源：http://jg.521024.cn

int main(int argc, char **argv)
来源：http://qo.nszjky.cn

[S19] C：快速排序
来源：http://vz.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zl.colortex.cn

[S20] C：二分查找
来源：http://dm.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hm.panjiajie.cn

[S21] C：字符类别判断
来源：http://va.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dy.chemitech.net.cn

[S22] C：字符串转数字
来源：http://kw.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rh.yuntaijiaju.cn

[S23] C：随机数
来源：http://bo.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ny.521024.cn

[S24] C：获取本地时间
来源：http://im.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ky.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://nr.nszjky.cn

memcpy(dst, src, n);
来源：http://fy.bookmarksfly.cn

[S26] C：内存清零
来源：http://fq.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://dy.jianghongdianzi.cn

[S27] C：定义常量
来源：http://yh.hahajie.cn

const double PI = 3.14159;
来源：http://cv.colortex.cn

[S28] C：静态变量
来源：http://dg.lnxyls.cn


<!-- 参考信息 -->