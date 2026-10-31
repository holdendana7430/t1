代发 wailian999

[Q76] 按天统计
来源：http://sp.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ep.muxihuayi.cn

[Q77] 时间加减
来源：http://ox.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ru.gzmigu.cn

[Q78] 当前时间
来源：http://sx.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jn.huixiangedu.cn

[Q79] 字符串拼接
来源：http://bl.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ij.9csxet.cn

[Q80] 字符串截取
来源：http://ql.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uj.asd995.cn

[Q81] 字符串替换
来源：http://st.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xy.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://xq.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dh.muxihuayi.cn

[Q83] 大小写转换
来源：http://vm.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gc.newstarts.cn

[Q84] 去除首尾空格
来源：http://wg.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://jm.asd995.cn

[Q85] 数值取整
来源：http://ne.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ed.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://og.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xw.asd995.cn

[Q87] JSON 字段做条件
来源：http://qz.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zy.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://cg.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cz.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ji.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://np.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://na.hnjuh.cn

[Q90] 生成序号列
来源：http://kv.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zb.yuexingan06.cn

================================================================================
来源：http://ln.wgjwhj.cn

R. Bash 专题
来源：http://io.huixinmuqiang.cn

================================================================================
来源：http://xk.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://cw.shxzukj.cn

#!/usr/bin/env bash
来源：http://po.jianghongdianzi.cn

set -euo pipefail
来源：http://ea.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://jv.szsharing.cn

name="Tom"; echo "$name"
来源：http://uc.gzmigu.cn

[R03] 只读变量
来源：http://ck.hahajie.cn

readonly PI=3.14
来源：http://fi.nszjky.cn

[R04] 位置参数
来源：http://el.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kk.9csxet.cn

[R05] 参数默认值
来源：http://jj.hahajie.cn

name="${1:-default}"
来源：http://rt.9csxet.cn

[R06] 判断命令是否存在
来源：http://je.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tz.yuexingan06.cn

[R07] if 判断文件
来源：http://rb.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yy.asd995.cn

[R08] 数值比较
来源：http://mx.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cm.jctech888.com.cn

[R09] 字符串比较
来源：http://ig.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lk.shxzskj.cn

[R10] 正则匹配
来源：http://en.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ti.shtwfgs.cn

[R11] case 多分支
来源：http://qm.colortex.cn

case "$1" in
来源：http://jb.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://gk.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://lu.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://hx.9csxet.cn

esac
来源：http://nb.szsharing.cn

[R12] for 遍历文件
来源：http://lg.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://sd.huanxung.cn

[R13] for 计数循环
来源：http://au.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://cr.szxytkj.cn

[R14] C 风格 for
来源：http://si.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xu.huixiangedu.cn

[R15] while 逐行读文件
来源：http://et.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wr.hahajie.cn

[R16] until 等待条件
来源：http://cx.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bz.colortex.cn

[R17] 数组定义与取值
来源：http://kj.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qu.jianghongdianzi.cn

[R18] 遍历数组
来源：http://bj.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ir.panjiajie.cn

[R19] 数组长度
来源：http://jk.colortex.cn

echo "${#arr[@]}"
来源：http://qz.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://uu.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gq.asd995.cn

[R21] 字符串长度
来源：http://mn.haigaiapp.cn

echo "${#s}"
来源：http://zg.haigaiapp.cn

[R22] 截取子串
来源：http://uh.newstarts.cn

echo "${s:0:5}"
来源：http://wa.jianghongdianzi.cn

[R23] 字符串替换
来源：http://an.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uk.bjjhwx.cn

[R24] 大小写转换
来源：http://hg.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ar.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://yz.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wn.lnxyls.cn

[R26] 命令替换
来源：http://gl.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://pz.yuexingan06.cn

[R27] 算术展开
来源：http://wb.nicolike.cn

echo $((1 + 2 * 3))
来源：http://nd.chemitech.net.cn

[R28] 浮点运算
来源：http://sz.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://zy.shtwfgs.cn

[R29] 定义函数
来源：http://bg.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lt.huanxung.cn

[R30] 函数返回状态码
来源：http://lw.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://yg.jianghongdianzi.cn

[R31] 局部变量
来源：http://ka.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://ng.yuexingan06.cn

[R32] 参数个数校验
来源：http://gh.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eo.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://ii.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mx.bookmarksfly.cn

[R34] 退出时清理
来源：http://qg.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fh.muxihuayi.cn

[R35] 后台执行并等待
来源：http://wn.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vb.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://eg.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://or.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://dw.yuntaijiaju.cn

files=$(ls -1)
来源：http://la.lnxyls.cn

[R38] 管道串联
来源：http://dv.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://rz.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://om.newstarts.cn

cmd > out.log 2>&1
来源：http://xc.9csxet.cn

[R40] 追加写日志
来源：http://jg.panjiajie.cn

echo "log" >> out.log
来源：http://wj.nszjky.cn

[R41] 丢弃输出
来源：http://fa.521024.cn

cmd >/dev/null 2>&1
来源：http://wh.521024.cn

[R42] 输入重定向
来源：http://zq.yuexingan06.cn

wc -l < a.txt
来源：http://fv.gzmigu.cn

[R43] 按名字查找文件
来源：http://ca.huixiangedu.cn

find . -name "*.log" -type f
来源：http://rp.szxytkj.cn

[R44] 按修改时间查找
来源：http://tm.asd995.cn

find . -mtime -7 -type f
来源：http://ux.jctech888.com.cn

[R45] 批量删除
来源：http://wk.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://hg.hnjuh.cn

[R46] 递归替换文件内容
来源：http://sk.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yb.hnjuh.cn

[R47] sed 单行替换
来源：http://mb.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fy.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://gi.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://ww.yuntaijiaju.cn

[R49] awk 带条件
来源：http://kc.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fc.haigaiapp.cn

[R50] awk 求和
来源：http://qn.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lo.yuexingan06.cn

[R51] 排序去重取前几
来源：http://fo.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gm.jctech888.com.cn

[R52] 统计行数
来源：http://zl.newstarts.cn

wc -l a.txt
来源：http://ls.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://hx.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pq.bookmarksfly.cn

[R54] 比较两个文件
来源：http://sf.huanxung.cn

diff a.txt b.txt
来源：http://qc.bjjhwx.cn

[R55] 压缩与解压
来源：http://ub.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dh.yuexingan06.cn

[R56] 远程拷贝
来源：http://zr.asd995.cn

scp file user@host:/path/
来源：http://xi.nicolike.cn

[R57] 远程执行命令
来源：http://zv.shxzukj.cn

ssh user@host 'uptime'
来源：http://ao.hahajie.cn

[R58] 下载文件
来源：http://dw.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nr.lnxyls.cn

[R59] 发 POST JSON
来源：http://re.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uk.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://zl.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gg.szxytkj.cn

[R61] 磁盘占用
来源：http://lr.nicolike.cn

df -h;  du -sh *
来源：http://pz.521024.cn

[R62] 找最占空间的文件
来源：http://ij.colortex.cn

du -ah . | sort -rh | head -10
来源：http://fq.wgjwhj.cn

[R63] 内存与进程
来源：http://yx.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://yt.chemitech.net.cn

[R64] 结束进程
来源：http://yu.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://gm.newstarts.cn

[R65] 查看端口占用
来源：http://hb.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pi.shtwfgs.cn

[R66] 定时任务
来源：http://ts.colortex.cn

crontab -e;  crontab -l
来源：http://zg.huanxung.cn

[R67] 生成随机十六进制串
来源：http://xq.shxzukj.cn

openssl rand -hex 16
来源：http://su.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://yl.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vo.9csxet.cn

[R69] 生成随机密码
来源：http://ep.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://dl.huixiangedu.cn

[R70] 时间戳与互转
来源：http://ao.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://kf.gzmigu.cn

[R71] 日期格式化
来源：http://vl.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mk.hahajie.cn

[R72] 等待端口就绪
来源：http://lu.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zp.shtwfgs.cn

[R73] 分割大日志
来源：http://ax.nszjky.cn

split -l 1000 big.log part_
来源：http://pr.nszjky.cn

[R74] 批量重命名
来源：http://tz.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ch.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://kv.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://en.lnxyls.cn

[R76] 使用临时文件
来源：http://ye.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bc.9csxet.cn

[R77] 读取用户输入
来源：http://bt.muxihuayi.cn

read -rp "请输入: " ans
来源：http://us.hnjuh.cn

[R78] 交互式菜单
来源：http://dn.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uc.lnxyls.cn

[R79] 解析命令行选项
来源：http://mg.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://by.asd995.cn

[R80] 查看脚本执行耗时
来源：http://qe.yuntaijiaju.cn

time ./run.sh
来源：http://bk.shxzskj.cn

================================================================================
来源：http://ze.szsharing.cn

S. C / C++ 专题
来源：http://mp.shxzskj.cn

================================================================================
来源：http://sq.gzmigu.cn

[S01] C：Hello World
来源：http://tw.colortex.cn

#include <stdio.h>
来源：http://xs.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xx.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://mj.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://oi.shxzskj.cn

[S03] C：读入整数
来源：http://sx.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://mh.panjiajie.cn

[S04] C：字符串复制
来源：http://pa.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oi.hnjuh.cn

[S05] C：字符串长度
来源：http://yj.hahajie.cn

strlen(s)
来源：http://pg.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://pt.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://ps.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://rp.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jw.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://pw.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ab.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://be.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ij.nszjky.cn

[S10] C：指针与解引用
来源：http://uy.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ms.9csxet.cn

[S11] C：逐行读文件
来源：http://lz.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://dq.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qc.newstarts.cn

fclose(f);
来源：http://yi.jctech888.com.cn

[S12] C：写文件
来源：http://yz.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://az.yuntaijiaju.cn

[S13] C：宏定义
来源：http://tu.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eq.huixiangedu.cn

[S14] C：枚举
来源：http://qq.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://qd.panjiajie.cn

[S15] C：类型转换
来源：http://pr.nszjky.cn

(double) a / b
来源：http://dk.szsharing.cn

[S16] C：位操作置位
来源：http://wj.gzmigu.cn

x |= (1 << 3);
来源：http://cf.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://jm.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ub.bjjhwx.cn

[S18] C：命令行参数
来源：http://hy.muxihuayi.cn

int main(int argc, char **argv)
来源：http://uv.hahajie.cn

[S19] C：快速排序
来源：http://er.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bo.haigaiapp.cn

[S20] C：二分查找
来源：http://zx.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gg.panjiajie.cn

[S21] C：字符类别判断
来源：http://bg.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kg.9csxet.cn

[S22] C：字符串转数字
来源：http://ue.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ao.wgjwhj.cn

[S23] C：随机数
来源：http://qx.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zs.asd995.cn

[S24] C：获取本地时间
来源：http://jx.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ec.hnjuh.cn

[S25] C：内存拷贝
来源：http://pw.gzmigu.cn

memcpy(dst, src, n);
来源：http://wk.muxihuayi.cn

[S26] C：内存清零
来源：http://rh.huanxung.cn

memset(a, 0, sizeof a);
来源：http://iq.szxytkj.cn

[S27] C：定义常量
来源：http://eu.newstarts.cn

const double PI = 3.14159;
来源：http://uz.9csxet.cn

[S28] C：静态变量
来源：http://mc.huanxung.cn

static int counter = 0;
来源：http://xn.jctech888.com.cn

[S29] C：变参函数
来源：http://ua.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jk.bookmarksfly.cn

[S30] C：头文件保护
来源：http://ug.huixiangedu.cn

#ifndef X_H
来源：http://qe.hahajie.cn

#define X_H
来源：http://ld.jianghongdianzi.cn

#endif
来源：http://ur.jctech888.com.cn

[S31] C++：Hello World
来源：http://ra.521024.cn

#include <iostream>
来源：http://oy.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://ua.szsharing.cn

[S32] C++：字符串
来源：http://uv.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://dx.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ir.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fb.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://md.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://tf.bjjhwx.cn

[S35] C++：map
来源：http://vt.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ij.yuexingan06.cn

[S36] C++：unordered_map
来源：http://kg.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wm.9csxet.cn

[S37] C++：set
来源：http://ma.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xl.asd995.cn

[S38] C++：排序
来源：http://ra.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://js.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://wg.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ba.nszjky.cn

[S40] C++：查找元素
来源：http://qh.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://as.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://bb.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zx.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://jy.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://zi.shtwfgs.cn

[S43] C++：智能指针
来源：http://zg.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://zj.huanxung.cn

[S44] C++：引用传参
来源：http://dk.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://tw.colortex.cn

[S45] C++：lambda
来源：http://vz.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xo.yuexingan06.cn

[S46] C++：函数模板
来源：http://kr.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://un.asd995.cn


<!-- 参考信息 -->