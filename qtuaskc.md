代发 wailian999

[Q76] 按天统计
来源：http://dd.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wc.szsharing.cn

[Q77] 时间加减
来源：http://mb.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mt.asd995.cn

[Q78] 当前时间
来源：http://xf.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ek.shtwfgs.cn

[Q79] 字符串拼接
来源：http://fv.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hn.panjiajie.cn

[Q80] 字符串截取
来源：http://fk.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://va.newstarts.cn

[Q81] 字符串替换
来源：http://cl.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uk.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://sy.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xt.bookmarksfly.cn

[Q83] 大小写转换
来源：http://le.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://it.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://zf.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://qw.szsharing.cn

[Q85] 数值取整
来源：http://yp.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pf.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://jg.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rn.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://ms.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vu.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://tr.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zu.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jg.hnjuh.cn

[Q89] 判断表是否存在
来源：http://yj.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.bjjhwx.cn

[Q90] 生成序号列
来源：http://zp.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xb.asd995.cn

================================================================================
来源：http://ns.huixinmuqiang.cn

R. Bash 专题
来源：http://iv.newstarts.cn

================================================================================
来源：http://ky.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://nl.chemitech.net.cn

#!/usr/bin/env bash
来源：http://bc.colortex.cn

set -euo pipefail
来源：http://ld.szsharing.cn

[R02] 变量赋值与使用
来源：http://ry.hnjuh.cn

name="Tom"; echo "$name"
来源：http://ho.gzmigu.cn

[R03] 只读变量
来源：http://oc.hnjuh.cn

readonly PI=3.14
来源：http://lj.szsharing.cn

[R04] 位置参数
来源：http://xo.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fe.haigaiapp.cn

[R05] 参数默认值
来源：http://vx.gzmigu.cn

name="${1:-default}"
来源：http://dt.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://sw.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://es.bjjhwx.cn

[R07] if 判断文件
来源：http://ey.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://su.asd995.cn

[R08] 数值比较
来源：http://xu.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ud.hahajie.cn

[R09] 字符串比较
来源：http://cb.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dj.wgjwhj.cn

[R10] 正则匹配
来源：http://oc.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wv.newstarts.cn

[R11] case 多分支
来源：http://hf.asd995.cn

case "$1" in
来源：http://lg.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://tn.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://qv.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://ze.shxzskj.cn

esac
来源：http://vi.bjjhwx.cn

[R12] for 遍历文件
来源：http://wr.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://ue.yuexingan06.cn

[R13] for 计数循环
来源：http://fr.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://ek.shxzukj.cn

[R14] C 风格 for
来源：http://ue.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yz.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://cw.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jm.bjjhwx.cn

[R16] until 等待条件
来源：http://lo.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xw.haigaiapp.cn

[R17] 数组定义与取值
来源：http://we.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qn.hahajie.cn

[R18] 遍历数组
来源：http://xx.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oc.yuexingan06.cn

[R19] 数组长度
来源：http://sv.gzmigu.cn

echo "${#arr[@]}"
来源：http://ck.521024.cn

[R20] 关联数组（字典）
来源：http://ck.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nl.jianghongdianzi.cn

[R21] 字符串长度
来源：http://gd.jianghongdianzi.cn

echo "${#s}"
来源：http://la.szsharing.cn

[R22] 截取子串
来源：http://sq.newstarts.cn

echo "${s:0:5}"
来源：http://lz.jianghongdianzi.cn

[R23] 字符串替换
来源：http://px.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vu.colortex.cn

[R24] 大小写转换
来源：http://uk.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ea.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://rq.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://er.gzmigu.cn

[R26] 命令替换
来源：http://rr.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://jg.bookmarksfly.cn

[R27] 算术展开
来源：http://pd.newstarts.cn

echo $((1 + 2 * 3))
来源：http://af.shtwfgs.cn

[R28] 浮点运算
来源：http://ff.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://mv.jianghongdianzi.cn

[R29] 定义函数
来源：http://uf.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ex.newstarts.cn

[R30] 函数返回状态码
来源：http://tx.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://mf.huanxung.cn

[R31] 局部变量
来源：http://mh.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://an.nszjky.cn

[R32] 参数个数校验
来源：http://wq.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xr.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://wd.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sn.nicolike.cn

[R34] 退出时清理
来源：http://ib.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ml.asd995.cn

[R35] 后台执行并等待
来源：http://oo.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rg.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://fy.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gh.9csxet.cn

[R37] 把输出赋给变量
来源：http://zy.wgjwhj.cn

files=$(ls -1)
来源：http://re.521024.cn

[R38] 管道串联
来源：http://gj.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://qv.521024.cn

[R39] 重定向标准输出与错误
来源：http://bq.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://tk.bjjhwx.cn

[R40] 追加写日志
来源：http://ij.521024.cn

echo "log" >> out.log
来源：http://tl.newstarts.cn

[R41] 丢弃输出
来源：http://ul.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://fj.szsharing.cn

[R42] 输入重定向
来源：http://so.asd995.cn

wc -l < a.txt
来源：http://jh.wgjwhj.cn

[R43] 按名字查找文件
来源：http://ab.lnxyls.cn

find . -name "*.log" -type f
来源：http://fb.asd995.cn

[R44] 按修改时间查找
来源：http://ak.panjiajie.cn

find . -mtime -7 -type f
来源：http://rr.haigaiapp.cn

[R45] 批量删除
来源：http://fk.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://oz.lnxyls.cn

[R46] 递归替换文件内容
来源：http://di.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ih.szxytkj.cn

[R47] sed 单行替换
来源：http://da.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hh.muxihuayi.cn

[R48] awk 取指定列
来源：http://ak.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://ue.gzmigu.cn

[R49] awk 带条件
来源：http://kz.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sp.muxihuayi.cn

[R50] awk 求和
来源：http://oq.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ed.nszjky.cn

[R51] 排序去重取前几
来源：http://go.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kx.chemitech.net.cn

[R52] 统计行数
来源：http://eb.jctech888.com.cn

wc -l a.txt
来源：http://vy.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://yp.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ly.muxihuayi.cn

[R54] 比较两个文件
来源：http://pr.szxytkj.cn

diff a.txt b.txt
来源：http://mi.hahajie.cn

[R55] 压缩与解压
来源：http://vh.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fz.shtwfgs.cn

[R56] 远程拷贝
来源：http://vx.bjjhwx.cn

scp file user@host:/path/
来源：http://dm.szsharing.cn

[R57] 远程执行命令
来源：http://ui.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://kr.szsharing.cn

[R58] 下载文件
来源：http://cp.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pv.yuexingan06.cn

[R59] 发 POST JSON
来源：http://fv.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ku.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://dj.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fk.szsharing.cn

[R61] 磁盘占用
来源：http://gu.huanxung.cn

df -h;  du -sh *
来源：http://tl.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://eg.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://jx.gzmigu.cn

[R63] 内存与进程
来源：http://zy.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://ps.hahajie.cn

[R64] 结束进程
来源：http://wn.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://ly.bookmarksfly.cn

[R65] 查看端口占用
来源：http://ez.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jy.shxzskj.cn

[R66] 定时任务
来源：http://bo.shxzukj.cn

crontab -e;  crontab -l
来源：http://sk.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://oe.yuntaijiaju.cn

openssl rand -hex 16
来源：http://no.shxzukj.cn

[R68] 计算文件校验值
来源：http://kz.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hh.huixiangedu.cn

[R69] 生成随机密码
来源：http://jk.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://xw.panjiajie.cn

[R70] 时间戳与互转
来源：http://qo.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://ne.hnjuh.cn

[R71] 日期格式化
来源：http://ju.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rh.hnjuh.cn

[R72] 等待端口就绪
来源：http://iu.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ws.wgjwhj.cn

[R73] 分割大日志
来源：http://mg.jctech888.com.cn

split -l 1000 big.log part_
来源：http://sz.hahajie.cn

[R74] 批量重命名
来源：http://ev.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xb.szsharing.cn

[R75] 导出环境变量
来源：http://vz.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://if.521024.cn

[R76] 使用临时文件
来源：http://ve.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cg.521024.cn

[R77] 读取用户输入
来源：http://nb.muxihuayi.cn

read -rp "请输入: " ans
来源：http://ps.bookmarksfly.cn

[R78] 交互式菜单
来源：http://ou.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://es.shxzukj.cn

[R79] 解析命令行选项
来源：http://nh.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zk.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://md.shtwfgs.cn

time ./run.sh
来源：http://ln.nicolike.cn

================================================================================
来源：http://ea.muxihuayi.cn

S. C / C++ 专题
来源：http://xk.huixiangedu.cn

================================================================================
来源：http://fz.huixinmuqiang.cn

[S01] C：Hello World
来源：http://hi.nicolike.cn

#include <stdio.h>
来源：http://td.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hq.colortex.cn

[S02] C：变量与格式化输出
来源：http://mf.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://ap.shxzskj.cn

[S03] C：读入整数
来源：http://ex.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://zb.521024.cn

[S04] C：字符串复制
来源：http://uf.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ii.hahajie.cn

[S05] C：字符串长度
来源：http://vx.szxytkj.cn

strlen(s)
来源：http://xg.huanxung.cn

[S06] C：字符串比较
来源：http://gb.yuexingan06.cn

strcmp(a, b) == 0
来源：http://wc.colortex.cn

[S07] C：数组遍历求和
来源：http://hb.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://en.colortex.cn

[S08] C：动态内存分配与释放
来源：http://df.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nm.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://ld.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uz.shxzskj.cn

[S10] C：指针与解引用
来源：http://kf.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://gk.bjjhwx.cn

[S11] C：逐行读文件
来源：http://wv.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://qi.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wu.muxihuayi.cn

fclose(f);
来源：http://lf.hahajie.cn

[S12] C：写文件
来源：http://ue.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wj.shxzukj.cn

[S13] C：宏定义
来源：http://vq.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hq.hnjuh.cn

[S14] C：枚举
来源：http://ll.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://nm.nszjky.cn

[S15] C：类型转换
来源：http://xn.newstarts.cn

(double) a / b
来源：http://us.szxytkj.cn

[S16] C：位操作置位
来源：http://ev.muxihuayi.cn

x |= (1 << 3);
来源：http://qk.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://yk.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qk.muxihuayi.cn

[S18] C：命令行参数
来源：http://yc.panjiajie.cn

int main(int argc, char **argv)
来源：http://rc.colortex.cn

[S19] C：快速排序
来源：http://fo.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oe.hahajie.cn

[S20] C：二分查找
来源：http://op.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qj.lnxyls.cn

[S21] C：字符类别判断
来源：http://vd.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ao.huanxung.cn

[S22] C：字符串转数字
来源：http://jx.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xz.hnjuh.cn

[S23] C：随机数
来源：http://yy.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qg.shtwfgs.cn

[S24] C：获取本地时间
来源：http://az.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cx.szxytkj.cn

[S25] C：内存拷贝
来源：http://hk.colortex.cn

memcpy(dst, src, n);
来源：http://ho.shxzukj.cn

[S26] C：内存清零
来源：http://km.9csxet.cn

memset(a, 0, sizeof a);
来源：http://kc.huixinmuqiang.cn

[S27] C：定义常量
来源：http://sx.yuexingan06.cn

const double PI = 3.14159;
来源：http://va.shxzskj.cn

[S28] C：静态变量
来源：http://cl.newstarts.cn

static int counter = 0;
来源：http://bp.hnjuh.cn

[S29] C：变参函数
来源：http://cu.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qb.huixiangedu.cn

[S30] C：头文件保护
来源：http://bl.shxzskj.cn

#ifndef X_H
来源：http://mo.521024.cn

#define X_H
来源：http://io.hnjuh.cn

#endif
来源：http://ol.huixiangedu.cn

[S31] C++：Hello World
来源：http://cz.lnxyls.cn

#include <iostream>
来源：http://ro.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://vg.haigaiapp.cn

[S32] C++：字符串
来源：http://eg.asd995.cn

std::string s = "hi";  s += "!";
来源：http://ea.asd995.cn

[S33] C++：vector 增删
来源：http://qt.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ph.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ll.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://kb.szxytkj.cn

[S35] C++：map
来源：http://uu.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ir.9csxet.cn

[S36] C++：unordered_map
来源：http://mt.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ov.nicolike.cn

[S37] C++：set
来源：http://gl.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uq.colortex.cn

[S38] C++：排序
来源：http://lf.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://yf.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://hs.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sm.nszjky.cn

[S40] C++：查找元素
来源：http://aw.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mx.panjiajie.cn

[S41] C++：类与构造函数
来源：http://ko.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zn.asd995.cn

[S42] C++：继承与虚函数
来源：http://ac.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://tu.wgjwhj.cn

[S43] C++：智能指针
来源：http://cb.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://oa.nszjky.cn

[S44] C++：引用传参
来源：http://nm.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://hw.huixiangedu.cn

[S45] C++：lambda
来源：http://xb.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pu.szxytkj.cn

[S46] C++：函数模板
来源：http://se.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bg.nszjky.cn


<!-- 参考信息 -->