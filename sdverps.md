代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oa.colortex.cn

[Q75] 日期格式化
来源：http://yf.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kv.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ew.521024.cn

[Q76] 按天统计
来源：http://ek.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sr.nicolike.cn

[Q77] 时间加减
来源：http://sd.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mr.bookmarksfly.cn

[Q78] 当前时间
来源：http://vs.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gd.asd995.cn

[Q79] 字符串拼接
来源：http://ia.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qd.muxihuayi.cn

[Q80] 字符串截取
来源：http://ls.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pe.asd995.cn

[Q81] 字符串替换
来源：http://tj.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hj.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://bm.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gz.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://fj.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zf.shxzukj.cn

[Q84] 去除首尾空格
来源：http://qh.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://hp.nicolike.cn

[Q85] 数值取整
来源：http://nw.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aq.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://eb.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ro.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://qz.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ck.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://pt.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wf.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aa.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://uy.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eu.bookmarksfly.cn

[Q90] 生成序号列
来源：http://mi.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qe.chemitech.net.cn

================================================================================
来源：http://fo.521024.cn

R. Bash 专题
来源：http://th.lnxyls.cn

================================================================================
来源：http://nm.lnxyls.cn

[R01] shebang 与严格模式
来源：http://su.szxytkj.cn

#!/usr/bin/env bash
来源：http://tb.huixiangedu.cn

set -euo pipefail
来源：http://te.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://gp.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://ql.muxihuayi.cn

[R03] 只读变量
来源：http://tx.wgjwhj.cn

readonly PI=3.14
来源：http://pi.jianghongdianzi.cn

[R04] 位置参数
来源：http://ri.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hh.9csxet.cn

[R05] 参数默认值
来源：http://zu.shxzukj.cn

name="${1:-default}"
来源：http://sm.nicolike.cn

[R06] 判断命令是否存在
来源：http://dy.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yq.shtwfgs.cn

[R07] if 判断文件
来源：http://rn.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ap.asd995.cn

[R08] 数值比较
来源：http://lo.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qj.bjjhwx.cn

[R09] 字符串比较
来源：http://qx.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pn.yuntaijiaju.cn

[R10] 正则匹配
来源：http://pl.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hq.nicolike.cn

[R11] case 多分支
来源：http://mt.hnjuh.cn

case "$1" in
来源：http://kj.nszjky.cn

start) echo "启动" ;;
来源：http://nq.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://kk.huanxung.cn

*)     echo "未知命令" ;;
来源：http://gw.nszjky.cn

esac
来源：http://im.nszjky.cn

[R12] for 遍历文件
来源：http://en.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://bx.szxytkj.cn

[R13] for 计数循环
来源：http://lw.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://tw.panjiajie.cn

[R14] C 风格 for
来源：http://tf.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ys.hnjuh.cn

[R15] while 逐行读文件
来源：http://py.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jo.jctech888.com.cn

[R16] until 等待条件
来源：http://gk.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oe.huixiangedu.cn

[R17] 数组定义与取值
来源：http://yg.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vf.haigaiapp.cn

[R18] 遍历数组
来源：http://ab.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vf.gzmigu.cn

[R19] 数组长度
来源：http://vm.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://tg.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://si.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qk.nicolike.cn

[R21] 字符串长度
来源：http://op.panjiajie.cn

echo "${#s}"
来源：http://vj.nicolike.cn

[R22] 截取子串
来源：http://qc.szsharing.cn

echo "${s:0:5}"
来源：http://bq.bookmarksfly.cn

[R23] 字符串替换
来源：http://xu.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wx.shtwfgs.cn

[R24] 大小写转换
来源：http://hi.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hm.521024.cn

[R25] 去后缀 / 去前缀
来源：http://ak.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bt.panjiajie.cn

[R26] 命令替换
来源：http://ui.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://uz.521024.cn

[R27] 算术展开
来源：http://ol.colortex.cn

echo $((1 + 2 * 3))
来源：http://hs.yuexingan06.cn

[R28] 浮点运算
来源：http://jl.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://va.muxihuayi.cn

[R29] 定义函数
来源：http://sa.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://po.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://wq.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://lo.bjjhwx.cn

[R31] 局部变量
来源：http://pk.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://ht.gzmigu.cn

[R32] 参数个数校验
来源：http://eh.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bg.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://ff.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yz.shxzukj.cn

[R34] 退出时清理
来源：http://vq.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vy.szsharing.cn

[R35] 后台执行并等待
来源：http://fc.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mx.colortex.cn

[R36] 并发执行多个任务
来源：http://wz.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://js.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://kp.chemitech.net.cn

files=$(ls -1)
来源：http://oi.jianghongdianzi.cn

[R38] 管道串联
来源：http://mz.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://xc.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://eg.9csxet.cn

cmd > out.log 2>&1
来源：http://yi.yuntaijiaju.cn

[R40] 追加写日志
来源：http://tb.wgjwhj.cn

echo "log" >> out.log
来源：http://go.yuexingan06.cn

[R41] 丢弃输出
来源：http://wx.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://bo.huixiangedu.cn

[R42] 输入重定向
来源：http://mo.hnjuh.cn

wc -l < a.txt
来源：http://lw.521024.cn

[R43] 按名字查找文件
来源：http://ds.nicolike.cn

find . -name "*.log" -type f
来源：http://wm.nicolike.cn

[R44] 按修改时间查找
来源：http://ta.szxytkj.cn

find . -mtime -7 -type f
来源：http://uq.szxytkj.cn

[R45] 批量删除
来源：http://un.nicolike.cn

find . -name "*.tmp" -delete
来源：http://xx.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://sq.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qf.asd995.cn

[R47] sed 单行替换
来源：http://ei.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ty.huixiangedu.cn

[R48] awk 取指定列
来源：http://op.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://nz.shxzukj.cn

[R49] awk 带条件
来源：http://qw.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jg.szsharing.cn

[R50] awk 求和
来源：http://bv.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hd.yuexingan06.cn

[R51] 排序去重取前几
来源：http://iu.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://we.shxzukj.cn

[R52] 统计行数
来源：http://oy.huixiangedu.cn

wc -l a.txt
来源：http://ih.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://wh.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sb.jctech888.com.cn

[R54] 比较两个文件
来源：http://pg.szsharing.cn

diff a.txt b.txt
来源：http://ow.newstarts.cn

[R55] 压缩与解压
来源：http://ag.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yk.chemitech.net.cn

[R56] 远程拷贝
来源：http://de.shtwfgs.cn

scp file user@host:/path/
来源：http://oi.colortex.cn

[R57] 远程执行命令
来源：http://ud.shxzukj.cn

ssh user@host 'uptime'
来源：http://zs.colortex.cn

[R58] 下载文件
来源：http://lp.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xr.lnxyls.cn

[R59] 发 POST JSON
来源：http://kg.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ng.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://jr.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fi.shtwfgs.cn

[R61] 磁盘占用
来源：http://mm.shtwfgs.cn

df -h;  du -sh *
来源：http://qf.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://kf.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://ea.521024.cn

[R63] 内存与进程
来源：http://fi.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://qr.nicolike.cn

[R64] 结束进程
来源：http://ou.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://fi.panjiajie.cn

[R65] 查看端口占用
来源：http://oz.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://di.haigaiapp.cn

[R66] 定时任务
来源：http://ah.colortex.cn

crontab -e;  crontab -l
来源：http://cq.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://on.panjiajie.cn

openssl rand -hex 16
来源：http://sq.szsharing.cn

[R68] 计算文件校验值
来源：http://ef.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://np.huanxung.cn

[R69] 生成随机密码
来源：http://bd.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://yz.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://nv.9csxet.cn

date +%s;  date -d @1700000000
来源：http://fs.haigaiapp.cn

[R71] 日期格式化
来源：http://mr.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bn.wgjwhj.cn

[R72] 等待端口就绪
来源：http://qv.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://am.huixinmuqiang.cn

[R73] 分割大日志
来源：http://qn.bjjhwx.cn

split -l 1000 big.log part_
来源：http://nb.nicolike.cn

[R74] 批量重命名
来源：http://aw.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bz.9csxet.cn

[R75] 导出环境变量
来源：http://cn.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://ty.huixiangedu.cn

[R76] 使用临时文件
来源：http://da.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ez.hahajie.cn

[R77] 读取用户输入
来源：http://ka.bjjhwx.cn

read -rp "请输入: " ans
来源：http://qj.huanxung.cn

[R78] 交互式菜单
来源：http://sm.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://df.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://zu.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lk.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://oj.shxzskj.cn

time ./run.sh
来源：http://dy.bjjhwx.cn

================================================================================
来源：http://jb.haigaiapp.cn

S. C / C++ 专题
来源：http://kt.hnjuh.cn

================================================================================
来源：http://bj.hnjuh.cn

[S01] C：Hello World
来源：http://ec.shxzukj.cn

#include <stdio.h>
来源：http://yj.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bl.newstarts.cn

[S02] C：变量与格式化输出
来源：http://zc.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://dj.haigaiapp.cn

[S03] C：读入整数
来源：http://fv.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://kx.colortex.cn

[S04] C：字符串复制
来源：http://xv.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zq.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://mi.gzmigu.cn

strlen(s)
来源：http://rt.szxytkj.cn

[S06] C：字符串比较
来源：http://do.haigaiapp.cn

strcmp(a, b) == 0
来源：http://ny.newstarts.cn

[S07] C：数组遍历求和
来源：http://xt.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ss.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://ka.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ly.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://fg.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zd.shxzukj.cn

[S10] C：指针与解引用
来源：http://om.nszjky.cn

int *p = &a;  *p = 5;
来源：http://ui.asd995.cn

[S11] C：逐行读文件
来源：http://cy.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://xl.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yb.gzmigu.cn

fclose(f);
来源：http://fv.asd995.cn

[S12] C：写文件
来源：http://uu.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tn.bjjhwx.cn

[S13] C：宏定义
来源：http://jy.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sm.hnjuh.cn

[S14] C：枚举
来源：http://jt.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://qa.shxzukj.cn

[S15] C：类型转换
来源：http://yf.yuntaijiaju.cn

(double) a / b
来源：http://zx.yuexingan06.cn

[S16] C：位操作置位
来源：http://yl.chemitech.net.cn

x |= (1 << 3);
来源：http://dr.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://aj.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://if.wgjwhj.cn

[S18] C：命令行参数
来源：http://id.newstarts.cn

int main(int argc, char **argv)
来源：http://pw.bjjhwx.cn

[S19] C：快速排序
来源：http://gp.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dl.shtwfgs.cn

[S20] C：二分查找
来源：http://fr.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ft.szsharing.cn

[S21] C：字符类别判断
来源：http://ex.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rl.9csxet.cn

[S22] C：字符串转数字
来源：http://iy.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://la.szxytkj.cn

[S23] C：随机数
来源：http://md.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wb.hnjuh.cn

[S24] C：获取本地时间
来源：http://rd.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://az.shtwfgs.cn

[S25] C：内存拷贝
来源：http://jt.wgjwhj.cn

memcpy(dst, src, n);
来源：http://oq.bookmarksfly.cn

[S26] C：内存清零
来源：http://ke.colortex.cn

memset(a, 0, sizeof a);
来源：http://yr.bjjhwx.cn

[S27] C：定义常量
来源：http://rt.shxzskj.cn

const double PI = 3.14159;
来源：http://gf.shxzukj.cn

[S28] C：静态变量
来源：http://ii.shxzskj.cn

static int counter = 0;
来源：http://ty.nicolike.cn

[S29] C：变参函数
来源：http://jd.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://en.gzmigu.cn

[S30] C：头文件保护
来源：http://wi.jianghongdianzi.cn

#ifndef X_H
来源：http://gu.gzmigu.cn

#define X_H
来源：http://tx.hnjuh.cn

#endif
来源：http://rl.yuexingan06.cn

[S31] C++：Hello World
来源：http://sm.haigaiapp.cn

#include <iostream>
来源：http://hh.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://qp.huixiangedu.cn

[S32] C++：字符串
来源：http://ca.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://sv.gzmigu.cn

[S33] C++：vector 增删
来源：http://ai.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kg.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://vc.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://le.lnxyls.cn

[S35] C++：map
来源：http://ca.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xa.huanxung.cn

[S36] C++：unordered_map
来源：http://pg.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ud.shxzskj.cn

[S37] C++：set
来源：http://yh.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vh.yuexingan06.cn

[S38] C++：排序
来源：http://mq.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://zz.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://vm.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dg.panjiajie.cn

[S40] C++：查找元素
来源：http://nd.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mw.szsharing.cn

[S41] C++：类与构造函数
来源：http://vx.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nk.huanxung.cn

[S42] C++：继承与虚函数
来源：http://tp.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://ui.szsharing.cn

[S43] C++：智能指针
来源：http://th.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://pn.wgjwhj.cn

[S44] C++：引用传参
来源：http://nc.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://wp.nszjky.cn


<!-- 参考信息 -->