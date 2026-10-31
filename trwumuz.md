代发 wailian999

SHOW INDEX FROM users;
来源：http://or.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://ij.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ps.muxihuayi.cn

[Q74] 强制使用索引
来源：http://nu.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xr.gzmigu.cn

[Q75] 日期格式化
来源：http://nk.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wn.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qt.asd995.cn

[Q76] 按天统计
来源：http://yv.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ig.yuntaijiaju.cn

[Q77] 时间加减
来源：http://hd.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uv.shtwfgs.cn

[Q78] 当前时间
来源：http://in.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uz.shtwfgs.cn

[Q79] 字符串拼接
来源：http://on.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cf.newstarts.cn

[Q80] 字符串截取
来源：http://xu.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lq.newstarts.cn

[Q81] 字符串替换
来源：http://jc.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cl.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://em.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lx.huixiangedu.cn

[Q83] 大小写转换
来源：http://fa.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bk.szsharing.cn

[Q84] 去除首尾空格
来源：http://na.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://ir.haigaiapp.cn

[Q85] 数值取整
来源：http://pi.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sg.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://lh.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kk.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://tp.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wu.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://mg.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tr.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vs.hnjuh.cn

[Q89] 判断表是否存在
来源：http://vr.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yk.huanxung.cn

[Q90] 生成序号列
来源：http://xj.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://my.521024.cn

================================================================================
来源：http://ix.yuntaijiaju.cn

R. Bash 专题
来源：http://fi.huanxung.cn

================================================================================
来源：http://mn.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://wn.shxzskj.cn

#!/usr/bin/env bash
来源：http://dm.shxzskj.cn

set -euo pipefail
来源：http://by.nszjky.cn

[R02] 变量赋值与使用
来源：http://qp.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://ho.521024.cn

[R03] 只读变量
来源：http://ov.chemitech.net.cn

readonly PI=3.14
来源：http://jc.shtwfgs.cn

[R04] 位置参数
来源：http://qh.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cb.bookmarksfly.cn

[R05] 参数默认值
来源：http://do.wgjwhj.cn

name="${1:-default}"
来源：http://ll.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://ea.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dy.panjiajie.cn

[R07] if 判断文件
来源：http://on.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iw.panjiajie.cn

[R08] 数值比较
来源：http://mo.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vt.colortex.cn

[R09] 字符串比较
来源：http://me.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dl.wgjwhj.cn

[R10] 正则匹配
来源：http://bi.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ye.hahajie.cn

[R11] case 多分支
来源：http://ww.wgjwhj.cn

case "$1" in
来源：http://hr.shxzukj.cn

start) echo "启动" ;;
来源：http://ls.huanxung.cn

stop)  echo "停止" ;;
来源：http://po.521024.cn

*)     echo "未知命令" ;;
来源：http://ds.yuexingan06.cn

esac
来源：http://zz.9csxet.cn

[R12] for 遍历文件
来源：http://zr.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://hu.jctech888.com.cn

[R13] for 计数循环
来源：http://jb.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://yy.521024.cn

[R14] C 风格 for
来源：http://pn.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mf.szsharing.cn

[R15] while 逐行读文件
来源：http://ly.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fo.szsharing.cn

[R16] until 等待条件
来源：http://ct.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ts.9csxet.cn

[R17] 数组定义与取值
来源：http://ar.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://la.bjjhwx.cn

[R18] 遍历数组
来源：http://le.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://op.lnxyls.cn

[R19] 数组长度
来源：http://vb.muxihuayi.cn

echo "${#arr[@]}"
来源：http://ml.panjiajie.cn

[R20] 关联数组（字典）
来源：http://xx.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lp.gzmigu.cn

[R21] 字符串长度
来源：http://de.shxzukj.cn

echo "${#s}"
来源：http://dd.yuexingan06.cn

[R22] 截取子串
来源：http://vk.nszjky.cn

echo "${s:0:5}"
来源：http://pp.szsharing.cn

[R23] 字符串替换
来源：http://tn.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://us.hahajie.cn

[R24] 大小写转换
来源：http://sp.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hr.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://vh.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ls.521024.cn

[R26] 命令替换
来源：http://yl.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://he.chemitech.net.cn

[R27] 算术展开
来源：http://hx.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://yp.shtwfgs.cn

[R28] 浮点运算
来源：http://iw.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://ni.521024.cn

[R29] 定义函数
来源：http://iz.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cw.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://bj.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ld.shtwfgs.cn

[R31] 局部变量
来源：http://np.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://ky.szxytkj.cn

[R32] 参数个数校验
来源：http://hm.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vd.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://sl.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fc.jianghongdianzi.cn

[R34] 退出时清理
来源：http://gt.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yw.huanxung.cn

[R35] 后台执行并等待
来源：http://hx.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://op.nszjky.cn

[R36] 并发执行多个任务
来源：http://ad.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ki.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://tu.jianghongdianzi.cn

files=$(ls -1)
来源：http://pg.9csxet.cn

[R38] 管道串联
来源：http://nr.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://qf.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://kr.muxihuayi.cn

cmd > out.log 2>&1
来源：http://mu.huixiangedu.cn

[R40] 追加写日志
来源：http://kq.521024.cn

echo "log" >> out.log
来源：http://il.521024.cn

[R41] 丢弃输出
来源：http://ag.9csxet.cn

cmd >/dev/null 2>&1
来源：http://pm.muxihuayi.cn

[R42] 输入重定向
来源：http://vs.huixiangedu.cn

wc -l < a.txt
来源：http://rc.shtwfgs.cn

[R43] 按名字查找文件
来源：http://wp.chemitech.net.cn

find . -name "*.log" -type f
来源：http://ph.szsharing.cn

[R44] 按修改时间查找
来源：http://tu.shxzskj.cn

find . -mtime -7 -type f
来源：http://fl.yuntaijiaju.cn

[R45] 批量删除
来源：http://zl.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://us.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://cu.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rs.gzmigu.cn

[R47] sed 单行替换
来源：http://gt.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iz.colortex.cn

[R48] awk 取指定列
来源：http://jl.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://cm.newstarts.cn

[R49] awk 带条件
来源：http://zd.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ym.9csxet.cn

[R50] awk 求和
来源：http://tc.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ls.asd995.cn

[R51] 排序去重取前几
来源：http://nf.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ys.chemitech.net.cn

[R52] 统计行数
来源：http://ey.newstarts.cn

wc -l a.txt
来源：http://ft.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://hh.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ka.haigaiapp.cn

[R54] 比较两个文件
来源：http://fh.huixiangedu.cn

diff a.txt b.txt
来源：http://si.jctech888.com.cn

[R55] 压缩与解压
来源：http://gy.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bq.hahajie.cn

[R56] 远程拷贝
来源：http://un.panjiajie.cn

scp file user@host:/path/
来源：http://yf.9csxet.cn

[R57] 远程执行命令
来源：http://bx.yuexingan06.cn

ssh user@host 'uptime'
来源：http://jt.colortex.cn

[R58] 下载文件
来源：http://bx.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hj.shxzskj.cn

[R59] 发 POST JSON
来源：http://lb.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yx.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://ag.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iz.shtwfgs.cn

[R61] 磁盘占用
来源：http://lx.haigaiapp.cn

df -h;  du -sh *
来源：http://cx.huanxung.cn

[R62] 找最占空间的文件
来源：http://te.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://fk.gzmigu.cn

[R63] 内存与进程
来源：http://og.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://yj.shxzukj.cn

[R64] 结束进程
来源：http://uk.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://fs.huanxung.cn

[R65] 查看端口占用
来源：http://jg.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tf.9csxet.cn

[R66] 定时任务
来源：http://fa.newstarts.cn

crontab -e;  crontab -l
来源：http://ot.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://oe.bjjhwx.cn

openssl rand -hex 16
来源：http://er.newstarts.cn

[R68] 计算文件校验值
来源：http://su.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mp.lnxyls.cn

[R69] 生成随机密码
来源：http://oe.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://nn.chemitech.net.cn

[R70] 时间戳与互转
来源：http://lq.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://qu.bookmarksfly.cn

[R71] 日期格式化
来源：http://vd.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fc.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://mz.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ks.asd995.cn

[R73] 分割大日志
来源：http://lt.shtwfgs.cn

split -l 1000 big.log part_
来源：http://ag.gzmigu.cn

[R74] 批量重命名
来源：http://el.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oq.521024.cn

[R75] 导出环境变量
来源：http://sh.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://tl.muxihuayi.cn

[R76] 使用临时文件
来源：http://pu.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rq.huixiangedu.cn

[R77] 读取用户输入
来源：http://hd.shxzskj.cn

read -rp "请输入: " ans
来源：http://gn.shxzskj.cn

[R78] 交互式菜单
来源：http://ze.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fu.gzmigu.cn

[R79] 解析命令行选项
来源：http://tc.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yq.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://mu.yuexingan06.cn

time ./run.sh
来源：http://nm.chemitech.net.cn

================================================================================
来源：http://qs.9csxet.cn

S. C / C++ 专题
来源：http://zt.shxzukj.cn

================================================================================
来源：http://pe.shtwfgs.cn

[S01] C：Hello World
来源：http://wr.yuexingan06.cn

#include <stdio.h>
来源：http://dp.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gs.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://yi.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://jv.szxytkj.cn

[S03] C：读入整数
来源：http://li.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://rf.huanxung.cn

[S04] C：字符串复制
来源：http://bz.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cl.szxytkj.cn

[S05] C：字符串长度
来源：http://lg.bookmarksfly.cn

strlen(s)
来源：http://he.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://cm.newstarts.cn

strcmp(a, b) == 0
来源：http://vx.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://ku.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rq.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://bj.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tw.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://bp.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gl.jctech888.com.cn

[S10] C：指针与解引用
来源：http://wr.nicolike.cn

int *p = &a;  *p = 5;
来源：http://zi.szxytkj.cn

[S11] C：逐行读文件
来源：http://ai.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://gz.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wi.9csxet.cn

fclose(f);
来源：http://fb.shxzskj.cn

[S12] C：写文件
来源：http://be.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://me.gzmigu.cn

[S13] C：宏定义
来源：http://xm.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tg.asd995.cn

[S14] C：枚举
来源：http://cn.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://di.asd995.cn

[S15] C：类型转换
来源：http://yz.huixinmuqiang.cn

(double) a / b
来源：http://yo.huixiangedu.cn

[S16] C：位操作置位
来源：http://ae.colortex.cn

x |= (1 << 3);
来源：http://mw.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://zs.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zy.shxzskj.cn

[S18] C：命令行参数
来源：http://uv.lnxyls.cn

int main(int argc, char **argv)
来源：http://ip.nszjky.cn

[S19] C：快速排序
来源：http://rm.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jk.jianghongdianzi.cn

[S20] C：二分查找
来源：http://jg.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bc.panjiajie.cn

[S21] C：字符类别判断
来源：http://qy.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bv.521024.cn

[S22] C：字符串转数字
来源：http://ik.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zy.gzmigu.cn

[S23] C：随机数
来源：http://fu.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wu.chemitech.net.cn

[S24] C：获取本地时间
来源：http://ae.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yt.newstarts.cn

[S25] C：内存拷贝
来源：http://oe.haigaiapp.cn

memcpy(dst, src, n);
来源：http://xr.nszjky.cn

[S26] C：内存清零
来源：http://si.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://pf.huixinmuqiang.cn

[S27] C：定义常量
来源：http://kj.521024.cn

const double PI = 3.14159;
来源：http://fv.newstarts.cn

[S28] C：静态变量
来源：http://wc.szxytkj.cn

static int counter = 0;
来源：http://dq.bjjhwx.cn

[S29] C：变参函数
来源：http://yv.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iu.muxihuayi.cn

[S30] C：头文件保护
来源：http://dw.huixiangedu.cn

#ifndef X_H
来源：http://vb.muxihuayi.cn

#define X_H
来源：http://ai.asd995.cn

#endif
来源：http://np.lnxyls.cn

[S31] C++：Hello World
来源：http://mb.huixiangedu.cn

#include <iostream>
来源：http://tl.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://bs.jctech888.com.cn

[S32] C++：字符串
来源：http://ub.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://bp.hnjuh.cn

[S33] C++：vector 增删
来源：http://wq.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eu.nszjky.cn

[S34] C++：遍历 vector
来源：http://gw.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://zr.panjiajie.cn

[S35] C++：map
来源：http://vv.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yp.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://ol.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zm.shtwfgs.cn

[S37] C++：set
来源：http://fm.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ky.521024.cn

[S38] C++：排序
来源：http://nf.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://xp.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://gc.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xy.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://px.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uk.huanxung.cn

[S41] C++：类与构造函数
来源：http://au.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://no.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://fm.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://ee.asd995.cn


<!-- 参考信息 -->