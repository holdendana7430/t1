代发 wailian999

SHOW INDEX FROM users;
来源：http://rn.szsharing.cn

[Q73] 查看表状态
来源：http://mr.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xh.panjiajie.cn

[Q74] 强制使用索引
来源：http://sg.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ub.huixiangedu.cn

[Q75] 日期格式化
来源：http://vr.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ot.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://li.huixinmuqiang.cn

[Q76] 按天统计
来源：http://jm.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ah.haigaiapp.cn

[Q77] 时间加减
来源：http://kj.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yv.asd995.cn

[Q78] 当前时间
来源：http://xa.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mf.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://de.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kj.jctech888.com.cn

[Q80] 字符串截取
来源：http://dz.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ny.jctech888.com.cn

[Q81] 字符串替换
来源：http://ly.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yb.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://fo.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fa.nszjky.cn

[Q83] 大小写转换
来源：http://fn.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dc.panjiajie.cn

[Q84] 去除首尾空格
来源：http://ma.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://ok.9csxet.cn

[Q85] 数值取整
来源：http://gb.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vs.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://gf.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ko.hahajie.cn

[Q87] JSON 字段做条件
来源：http://ox.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tb.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://qd.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ii.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vn.panjiajie.cn

[Q89] 判断表是否存在
来源：http://vg.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vy.nicolike.cn

[Q90] 生成序号列
来源：http://qe.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zz.lnxyls.cn

================================================================================
来源：http://qz.huixiangedu.cn

R. Bash 专题
来源：http://kz.nicolike.cn

================================================================================
来源：http://vd.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://hn.muxihuayi.cn

#!/usr/bin/env bash
来源：http://bp.nszjky.cn

set -euo pipefail
来源：http://ab.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://bd.panjiajie.cn

name="Tom"; echo "$name"
来源：http://tg.shxzukj.cn

[R03] 只读变量
来源：http://hn.lnxyls.cn

readonly PI=3.14
来源：http://dr.521024.cn

[R04] 位置参数
来源：http://az.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gn.muxihuayi.cn

[R05] 参数默认值
来源：http://gw.huixiangedu.cn

name="${1:-default}"
来源：http://fn.colortex.cn

[R06] 判断命令是否存在
来源：http://eg.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ai.haigaiapp.cn

[R07] if 判断文件
来源：http://qa.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rx.jianghongdianzi.cn

[R08] 数值比较
来源：http://hp.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ak.hahajie.cn

[R09] 字符串比较
来源：http://za.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yv.lnxyls.cn

[R10] 正则匹配
来源：http://nu.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lp.nicolike.cn

[R11] case 多分支
来源：http://uq.colortex.cn

case "$1" in
来源：http://lf.hahajie.cn

start) echo "启动" ;;
来源：http://ak.shxzukj.cn

stop)  echo "停止" ;;
来源：http://sk.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://vy.szsharing.cn

esac
来源：http://nt.lnxyls.cn

[R12] for 遍历文件
来源：http://ft.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://qj.wgjwhj.cn

[R13] for 计数循环
来源：http://vg.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://nj.shtwfgs.cn

[R14] C 风格 for
来源：http://jj.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://si.shxzskj.cn

[R15] while 逐行读文件
来源：http://ot.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zo.jianghongdianzi.cn

[R16] until 等待条件
来源：http://fv.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tb.wgjwhj.cn

[R17] 数组定义与取值
来源：http://cz.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rs.shxzskj.cn

[R18] 遍历数组
来源：http://vs.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eg.muxihuayi.cn

[R19] 数组长度
来源：http://kl.szsharing.cn

echo "${#arr[@]}"
来源：http://yy.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://ab.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tt.bjjhwx.cn

[R21] 字符串长度
来源：http://ka.huanxung.cn

echo "${#s}"
来源：http://qg.jctech888.com.cn

[R22] 截取子串
来源：http://bf.lnxyls.cn

echo "${s:0:5}"
来源：http://ru.shxzskj.cn

[R23] 字符串替换
来源：http://ph.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bc.colortex.cn

[R24] 大小写转换
来源：http://cm.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oo.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://bw.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jm.haigaiapp.cn

[R26] 命令替换
来源：http://ag.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://us.shxzukj.cn

[R27] 算术展开
来源：http://yx.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://yx.yuntaijiaju.cn

[R28] 浮点运算
来源：http://md.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://ki.haigaiapp.cn

[R29] 定义函数
来源：http://ej.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mu.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://ie.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://at.jianghongdianzi.cn

[R31] 局部变量
来源：http://wk.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://qx.wgjwhj.cn

[R32] 参数个数校验
来源：http://gw.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vg.colortex.cn

[R33] 捕获错误并提示行号
来源：http://qx.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cs.huixinmuqiang.cn

[R34] 退出时清理
来源：http://vw.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ye.panjiajie.cn

[R35] 后台执行并等待
来源：http://vt.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nu.huanxung.cn

[R36] 并发执行多个任务
来源：http://jz.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ko.huanxung.cn

[R37] 把输出赋给变量
来源：http://im.wgjwhj.cn

files=$(ls -1)
来源：http://iw.chemitech.net.cn

[R38] 管道串联
来源：http://cf.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://pp.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://vp.colortex.cn

cmd > out.log 2>&1
来源：http://wo.huanxung.cn

[R40] 追加写日志
来源：http://mf.shxzskj.cn

echo "log" >> out.log
来源：http://ae.szsharing.cn

[R41] 丢弃输出
来源：http://on.huanxung.cn

cmd >/dev/null 2>&1
来源：http://rt.szxytkj.cn

[R42] 输入重定向
来源：http://sj.asd995.cn

wc -l < a.txt
来源：http://oe.yuexingan06.cn

[R43] 按名字查找文件
来源：http://bw.haigaiapp.cn

find . -name "*.log" -type f
来源：http://dr.gzmigu.cn

[R44] 按修改时间查找
来源：http://kn.huanxung.cn

find . -mtime -7 -type f
来源：http://dp.nicolike.cn

[R45] 批量删除
来源：http://ht.newstarts.cn

find . -name "*.tmp" -delete
来源：http://kk.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://wy.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ri.nszjky.cn

[R47] sed 单行替换
来源：http://da.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mw.colortex.cn

[R48] awk 取指定列
来源：http://de.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://px.hahajie.cn

[R49] awk 带条件
来源：http://vw.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sp.shtwfgs.cn

[R50] awk 求和
来源：http://dc.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lp.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://yp.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fv.jctech888.com.cn

[R52] 统计行数
来源：http://pn.521024.cn

wc -l a.txt
来源：http://bp.521024.cn

[R53] 查看文件头与实时尾
来源：http://mt.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mb.bookmarksfly.cn

[R54] 比较两个文件
来源：http://eq.huixiangedu.cn

diff a.txt b.txt
来源：http://hh.szxytkj.cn

[R55] 压缩与解压
来源：http://tc.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kd.haigaiapp.cn

[R56] 远程拷贝
来源：http://um.nszjky.cn

scp file user@host:/path/
来源：http://dm.gzmigu.cn

[R57] 远程执行命令
来源：http://hi.521024.cn

ssh user@host 'uptime'
来源：http://qw.wgjwhj.cn

[R58] 下载文件
来源：http://xc.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ax.huanxung.cn

[R59] 发 POST JSON
来源：http://hy.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vm.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://xz.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tk.nszjky.cn

[R61] 磁盘占用
来源：http://ba.haigaiapp.cn

df -h;  du -sh *
来源：http://ko.521024.cn

[R62] 找最占空间的文件
来源：http://sr.521024.cn

du -ah . | sort -rh | head -10
来源：http://ck.haigaiapp.cn

[R63] 内存与进程
来源：http://ct.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://yx.wgjwhj.cn

[R64] 结束进程
来源：http://ft.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://nv.asd995.cn

[R65] 查看端口占用
来源：http://mk.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jp.asd995.cn

[R66] 定时任务
来源：http://lz.shxzukj.cn

crontab -e;  crontab -l
来源：http://yr.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://na.bookmarksfly.cn

openssl rand -hex 16
来源：http://vo.huixiangedu.cn

[R68] 计算文件校验值
来源：http://il.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tt.nszjky.cn

[R69] 生成随机密码
来源：http://mc.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://ft.huixiangedu.cn

[R70] 时间戳与互转
来源：http://vx.9csxet.cn

date +%s;  date -d @1700000000
来源：http://ci.shtwfgs.cn

[R71] 日期格式化
来源：http://yc.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mi.gzmigu.cn

[R72] 等待端口就绪
来源：http://qy.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oo.muxihuayi.cn

[R73] 分割大日志
来源：http://zj.hnjuh.cn

split -l 1000 big.log part_
来源：http://ek.wgjwhj.cn

[R74] 批量重命名
来源：http://lv.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fb.szxytkj.cn

[R75] 导出环境变量
来源：http://rw.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://dm.muxihuayi.cn

[R76] 使用临时文件
来源：http://ur.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rj.colortex.cn

[R77] 读取用户输入
来源：http://oa.shxzskj.cn

read -rp "请输入: " ans
来源：http://qo.nicolike.cn

[R78] 交互式菜单
来源：http://xw.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oj.yuexingan06.cn

[R79] 解析命令行选项
来源：http://lp.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xv.asd995.cn

[R80] 查看脚本执行耗时
来源：http://mt.haigaiapp.cn

time ./run.sh
来源：http://pf.jctech888.com.cn

================================================================================
来源：http://oa.yuntaijiaju.cn

S. C / C++ 专题
来源：http://xe.bookmarksfly.cn

================================================================================
来源：http://gs.hahajie.cn

[S01] C：Hello World
来源：http://fb.asd995.cn

#include <stdio.h>
来源：http://ow.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yt.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://mt.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://jg.haigaiapp.cn

[S03] C：读入整数
来源：http://wp.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://sz.muxihuayi.cn

[S04] C：字符串复制
来源：http://xq.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cx.bjjhwx.cn

[S05] C：字符串长度
来源：http://cv.gzmigu.cn

strlen(s)
来源：http://tx.shxzukj.cn

[S06] C：字符串比较
来源：http://qv.jctech888.com.cn

strcmp(a, b) == 0
来源：http://jx.newstarts.cn

[S07] C：数组遍历求和
来源：http://wy.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cu.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://vi.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://db.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://lg.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ye.9csxet.cn

[S10] C：指针与解引用
来源：http://wz.asd995.cn

int *p = &a;  *p = 5;
来源：http://cg.bjjhwx.cn

[S11] C：逐行读文件
来源：http://pd.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://ai.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wb.szxytkj.cn

fclose(f);
来源：http://en.szsharing.cn

[S12] C：写文件
来源：http://br.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jr.nicolike.cn

[S13] C：宏定义
来源：http://gi.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ih.szxytkj.cn

[S14] C：枚举
来源：http://fx.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://sx.panjiajie.cn

[S15] C：类型转换
来源：http://uz.yuntaijiaju.cn

(double) a / b
来源：http://gl.bjjhwx.cn

[S16] C：位操作置位
来源：http://vx.yuexingan06.cn

x |= (1 << 3);
来源：http://id.521024.cn

[S17] C：安全拼接字符串
来源：http://zg.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dz.szxytkj.cn

[S18] C：命令行参数
来源：http://rr.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://gw.newstarts.cn

[S19] C：快速排序
来源：http://gq.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uw.newstarts.cn

[S20] C：二分查找
来源：http://ld.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rn.szxytkj.cn

[S21] C：字符类别判断
来源：http://es.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ma.gzmigu.cn

[S22] C：字符串转数字
来源：http://ji.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tw.huixiangedu.cn

[S23] C：随机数
来源：http://qy.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ng.chemitech.net.cn

[S24] C：获取本地时间
来源：http://mx.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hs.szxytkj.cn

[S25] C：内存拷贝
来源：http://yr.huanxung.cn

memcpy(dst, src, n);
来源：http://kg.yuntaijiaju.cn

[S26] C：内存清零
来源：http://rw.9csxet.cn

memset(a, 0, sizeof a);
来源：http://xc.bjjhwx.cn

[S27] C：定义常量
来源：http://qq.panjiajie.cn

const double PI = 3.14159;
来源：http://dm.huixiangedu.cn

[S28] C：静态变量
来源：http://le.colortex.cn

static int counter = 0;
来源：http://nx.bjjhwx.cn

[S29] C：变参函数
来源：http://kc.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mk.shxzukj.cn

[S30] C：头文件保护
来源：http://uf.wgjwhj.cn

#ifndef X_H
来源：http://qo.jianghongdianzi.cn

#define X_H
来源：http://ps.muxihuayi.cn

#endif
来源：http://ly.shtwfgs.cn

[S31] C++：Hello World
来源：http://zd.muxihuayi.cn

#include <iostream>
来源：http://ep.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://ds.jctech888.com.cn

[S32] C++：字符串
来源：http://ly.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://fl.bjjhwx.cn

[S33] C++：vector 增删
来源：http://iw.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fk.hahajie.cn

[S34] C++：遍历 vector
来源：http://yo.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://kh.bjjhwx.cn

[S35] C++：map
来源：http://ml.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yf.panjiajie.cn

[S36] C++：unordered_map
来源：http://ig.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ah.asd995.cn

[S37] C++：set
来源：http://qy.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yw.jctech888.com.cn

[S38] C++：排序
来源：http://no.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://nd.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://xv.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://df.shtwfgs.cn

[S40] C++：查找元素
来源：http://yl.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cp.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://bs.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zi.nszjky.cn

[S42] C++：继承与虚函数
来源：http://tw.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://ro.asd995.cn


<!-- 参考信息 -->