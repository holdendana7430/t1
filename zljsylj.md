代发 wailian999

ANALYZE TABLE users;
来源：http://da.huanxung.cn

[Q71] 查看建表语句
来源：http://wo.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rz.bookmarksfly.cn

[Q72] 查看索引
来源：http://gg.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://fr.muxihuayi.cn

[Q73] 查看表状态
来源：http://vs.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pl.shxzskj.cn

[Q74] 强制使用索引
来源：http://iz.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xh.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://hk.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://be.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yl.huixiangedu.cn

[Q76] 按天统计
来源：http://qd.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fm.shxzukj.cn

[Q77] 时间加减
来源：http://kn.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://py.muxihuayi.cn

[Q78] 当前时间
来源：http://kr.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oi.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://vp.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uw.jctech888.com.cn

[Q80] 字符串截取
来源：http://ag.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zx.wgjwhj.cn

[Q81] 字符串替换
来源：http://kc.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sa.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://ff.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gc.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://co.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yu.shxzskj.cn

[Q84] 去除首尾空格
来源：http://yn.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://ps.yuexingan06.cn

[Q85] 数值取整
来源：http://zs.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zm.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://ba.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xu.521024.cn

[Q87] JSON 字段做条件
来源：http://ya.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hb.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://td.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nk.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ct.asd995.cn

[Q89] 判断表是否存在
来源：http://lb.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ni.yuexingan06.cn

[Q90] 生成序号列
来源：http://zs.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cc.huanxung.cn

================================================================================
来源：http://xp.szsharing.cn

R. Bash 专题
来源：http://yh.521024.cn

================================================================================
来源：http://cd.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://iy.szxytkj.cn

#!/usr/bin/env bash
来源：http://cw.szsharing.cn

set -euo pipefail
来源：http://uu.521024.cn

[R02] 变量赋值与使用
来源：http://kg.lnxyls.cn

name="Tom"; echo "$name"
来源：http://np.gzmigu.cn

[R03] 只读变量
来源：http://bs.yuexingan06.cn

readonly PI=3.14
来源：http://ot.muxihuayi.cn

[R04] 位置参数
来源：http://fh.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://np.hnjuh.cn

[R05] 参数默认值
来源：http://zo.szsharing.cn

name="${1:-default}"
来源：http://cg.lnxyls.cn

[R06] 判断命令是否存在
来源：http://ne.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tc.asd995.cn

[R07] if 判断文件
来源：http://js.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://im.jctech888.com.cn

[R08] 数值比较
来源：http://mh.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mu.9csxet.cn

[R09] 字符串比较
来源：http://uq.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ze.huixinmuqiang.cn

[R10] 正则匹配
来源：http://tx.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vk.panjiajie.cn

[R11] case 多分支
来源：http://pb.hahajie.cn

case "$1" in
来源：http://ld.shxzukj.cn

start) echo "启动" ;;
来源：http://os.panjiajie.cn

stop)  echo "停止" ;;
来源：http://rw.szsharing.cn

*)     echo "未知命令" ;;
来源：http://ar.gzmigu.cn

esac
来源：http://qw.muxihuayi.cn

[R12] for 遍历文件
来源：http://es.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://aq.szsharing.cn

[R13] for 计数循环
来源：http://qg.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://hy.nszjky.cn

[R14] C 风格 for
来源：http://ni.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yx.hahajie.cn

[R15] while 逐行读文件
来源：http://ys.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gi.huixiangedu.cn

[R16] until 等待条件
来源：http://hj.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qp.szsharing.cn

[R17] 数组定义与取值
来源：http://ji.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zf.nicolike.cn

[R18] 遍历数组
来源：http://tz.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nx.nszjky.cn

[R19] 数组长度
来源：http://zd.nicolike.cn

echo "${#arr[@]}"
来源：http://il.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://vy.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aa.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ho.bookmarksfly.cn

echo "${#s}"
来源：http://qr.wgjwhj.cn

[R22] 截取子串
来源：http://ip.huanxung.cn

echo "${s:0:5}"
来源：http://pb.521024.cn

[R23] 字符串替换
来源：http://xh.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qx.panjiajie.cn

[R24] 大小写转换
来源：http://jt.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ta.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://zk.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ky.huixiangedu.cn

[R26] 命令替换
来源：http://rt.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://lp.yuntaijiaju.cn

[R27] 算术展开
来源：http://gu.9csxet.cn

echo $((1 + 2 * 3))
来源：http://sb.yuntaijiaju.cn

[R28] 浮点运算
来源：http://tm.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://gr.haigaiapp.cn

[R29] 定义函数
来源：http://dm.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cz.szxytkj.cn

[R30] 函数返回状态码
来源：http://gd.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://ro.wgjwhj.cn

[R31] 局部变量
来源：http://pt.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://sj.bookmarksfly.cn

[R32] 参数个数校验
来源：http://fw.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ap.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://qx.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://le.gzmigu.cn

[R34] 退出时清理
来源：http://fo.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://do.9csxet.cn

[R35] 后台执行并等待
来源：http://ok.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ty.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://dq.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pq.gzmigu.cn

[R37] 把输出赋给变量
来源：http://gg.colortex.cn

files=$(ls -1)
来源：http://gf.szsharing.cn

[R38] 管道串联
来源：http://vc.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://kz.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://fc.szxytkj.cn

cmd > out.log 2>&1
来源：http://aw.9csxet.cn

[R40] 追加写日志
来源：http://sx.szsharing.cn

echo "log" >> out.log
来源：http://ji.huanxung.cn

[R41] 丢弃输出
来源：http://lq.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://gh.shxzukj.cn

[R42] 输入重定向
来源：http://xt.wgjwhj.cn

wc -l < a.txt
来源：http://ll.nicolike.cn

[R43] 按名字查找文件
来源：http://ix.huanxung.cn

find . -name "*.log" -type f
来源：http://wx.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://no.szxytkj.cn

find . -mtime -7 -type f
来源：http://be.jctech888.com.cn

[R45] 批量删除
来源：http://iq.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://zw.newstarts.cn

[R46] 递归替换文件内容
来源：http://zi.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pt.huanxung.cn

[R47] sed 单行替换
来源：http://qn.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cj.nszjky.cn

[R48] awk 取指定列
来源：http://yq.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://mq.shxzukj.cn

[R49] awk 带条件
来源：http://ny.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wi.lnxyls.cn

[R50] awk 求和
来源：http://fy.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uh.bjjhwx.cn

[R51] 排序去重取前几
来源：http://ne.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wgjwhj.cn

[R52] 统计行数
来源：http://oy.yuexingan06.cn

wc -l a.txt
来源：http://tk.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://jm.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://my.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://dg.muxihuayi.cn

diff a.txt b.txt
来源：http://ky.shxzskj.cn

[R55] 压缩与解压
来源：http://ii.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yl.muxihuayi.cn

[R56] 远程拷贝
来源：http://eg.newstarts.cn

scp file user@host:/path/
来源：http://tz.huanxung.cn

[R57] 远程执行命令
来源：http://yu.szsharing.cn

ssh user@host 'uptime'
来源：http://ry.yuntaijiaju.cn

[R58] 下载文件
来源：http://lk.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ae.jctech888.com.cn

[R59] 发 POST JSON
来源：http://rn.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qw.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://gr.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://it.jctech888.com.cn

[R61] 磁盘占用
来源：http://xl.panjiajie.cn

df -h;  du -sh *
来源：http://zf.lnxyls.cn

[R62] 找最占空间的文件
来源：http://kq.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://lc.panjiajie.cn

[R63] 内存与进程
来源：http://hx.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://nd.asd995.cn

[R64] 结束进程
来源：http://pm.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://uq.hahajie.cn

[R65] 查看端口占用
来源：http://bl.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kp.shtwfgs.cn

[R66] 定时任务
来源：http://zs.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://vt.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://zn.panjiajie.cn

openssl rand -hex 16
来源：http://sd.hnjuh.cn

[R68] 计算文件校验值
来源：http://vs.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sj.hnjuh.cn

[R69] 生成随机密码
来源：http://kh.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://pd.newstarts.cn

[R70] 时间戳与互转
来源：http://nq.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://vy.9csxet.cn

[R71] 日期格式化
来源：http://fv.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qu.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://st.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jj.jianghongdianzi.cn

[R73] 分割大日志
来源：http://sz.chemitech.net.cn

split -l 1000 big.log part_
来源：http://mf.muxihuayi.cn

[R74] 批量重命名
来源：http://vb.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ck.panjiajie.cn

[R75] 导出环境变量
来源：http://ik.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://xm.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://qr.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ee.nszjky.cn

[R77] 读取用户输入
来源：http://ra.colortex.cn

read -rp "请输入: " ans
来源：http://cr.colortex.cn

[R78] 交互式菜单
来源：http://lg.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oo.9csxet.cn

[R79] 解析命令行选项
来源：http://wi.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tp.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://hl.hahajie.cn

time ./run.sh
来源：http://ji.yuexingan06.cn

================================================================================
来源：http://kr.shxzskj.cn

S. C / C++ 专题
来源：http://bl.huixinmuqiang.cn

================================================================================
来源：http://an.gzmigu.cn

[S01] C：Hello World
来源：http://dn.nszjky.cn

#include <stdio.h>
来源：http://kc.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jf.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://wd.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://kp.jianghongdianzi.cn

[S03] C：读入整数
来源：http://pn.lnxyls.cn

int x; scanf("%d", &x);
来源：http://yj.bjjhwx.cn

[S04] C：字符串复制
来源：http://il.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jv.newstarts.cn

[S05] C：字符串长度
来源：http://as.shxzukj.cn

strlen(s)
来源：http://sl.huanxung.cn

[S06] C：字符串比较
来源：http://iv.nicolike.cn

strcmp(a, b) == 0
来源：http://ht.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://br.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zr.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://gg.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://px.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://fq.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jg.shtwfgs.cn

[S10] C：指针与解引用
来源：http://th.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://dw.jctech888.com.cn

[S11] C：逐行读文件
来源：http://iz.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://js.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rx.newstarts.cn

fclose(f);
来源：http://or.bookmarksfly.cn

[S12] C：写文件
来源：http://xv.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pw.jctech888.com.cn

[S13] C：宏定义
来源：http://zo.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tu.shxzskj.cn

[S14] C：枚举
来源：http://el.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://zl.shtwfgs.cn

[S15] C：类型转换
来源：http://gv.nicolike.cn

(double) a / b
来源：http://jk.hahajie.cn

[S16] C：位操作置位
来源：http://cj.521024.cn

x |= (1 << 3);
来源：http://dd.9csxet.cn

[S17] C：安全拼接字符串
来源：http://zr.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pv.gzmigu.cn

[S18] C：命令行参数
来源：http://ww.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://in.gzmigu.cn

[S19] C：快速排序
来源：http://nx.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gf.newstarts.cn

[S20] C：二分查找
来源：http://uo.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dy.521024.cn

[S21] C：字符类别判断
来源：http://bi.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kj.bjjhwx.cn

[S22] C：字符串转数字
来源：http://do.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://co.huixiangedu.cn

[S23] C：随机数
来源：http://fz.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kn.newstarts.cn

[S24] C：获取本地时间
来源：http://pd.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vu.haigaiapp.cn

[S25] C：内存拷贝
来源：http://fd.yuexingan06.cn

memcpy(dst, src, n);
来源：http://qz.shtwfgs.cn

[S26] C：内存清零
来源：http://ql.nszjky.cn

memset(a, 0, sizeof a);
来源：http://td.huixiangedu.cn

[S27] C：定义常量
来源：http://yo.szxytkj.cn

const double PI = 3.14159;
来源：http://wm.jctech888.com.cn

[S28] C：静态变量
来源：http://ka.asd995.cn

static int counter = 0;
来源：http://ts.szxytkj.cn

[S29] C：变参函数
来源：http://cf.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ik.hnjuh.cn

[S30] C：头文件保护
来源：http://nm.jianghongdianzi.cn

#ifndef X_H
来源：http://jh.shxzukj.cn

#define X_H
来源：http://gq.9csxet.cn

#endif
来源：http://uf.jctech888.com.cn

[S31] C++：Hello World
来源：http://wj.chemitech.net.cn

#include <iostream>
来源：http://ai.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://aw.szxytkj.cn

[S32] C++：字符串
来源：http://qu.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://sz.panjiajie.cn

[S33] C++：vector 增删
来源：http://en.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vf.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://gk.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://mo.yuntaijiaju.cn

[S35] C++：map
来源：http://nh.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kw.chemitech.net.cn

[S36] C++：unordered_map
来源：http://ua.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lz.9csxet.cn

[S37] C++：set
来源：http://ea.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://an.shxzskj.cn

[S38] C++：排序
来源：http://qz.colortex.cn

std::sort(v.begin(), v.end());
来源：http://id.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://si.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nb.colortex.cn

[S40] C++：查找元素
来源：http://ox.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://by.hnjuh.cn


<!-- 参考信息 -->