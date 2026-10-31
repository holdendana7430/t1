代发 wailian999

[Q76] 按天统计
来源：http://jz.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://el.szxytkj.cn

[Q77] 时间加减
来源：http://bc.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bi.newstarts.cn

[Q78] 当前时间
来源：http://eb.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qh.bjjhwx.cn

[Q79] 字符串拼接
来源：http://dq.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ix.szxytkj.cn

[Q80] 字符串截取
来源：http://cg.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yy.yuexingan06.cn

[Q81] 字符串替换
来源：http://ql.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lm.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://mf.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uh.chemitech.net.cn

[Q83] 大小写转换
来源：http://wg.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zx.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://zn.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://dj.shxzskj.cn

[Q85] 数值取整
来源：http://bu.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pb.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://un.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ki.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://kj.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xm.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://sq.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yk.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fp.nicolike.cn

[Q89] 判断表是否存在
来源：http://mb.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://om.shxzukj.cn

[Q90] 生成序号列
来源：http://iq.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ul.521024.cn

================================================================================
来源：http://gx.bjjhwx.cn

R. Bash 专题
来源：http://ac.bjjhwx.cn

================================================================================
来源：http://cl.521024.cn

[R01] shebang 与严格模式
来源：http://oe.szsharing.cn

#!/usr/bin/env bash
来源：http://tb.newstarts.cn

set -euo pipefail
来源：http://xn.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://zh.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://eq.nicolike.cn

[R03] 只读变量
来源：http://if.nszjky.cn

readonly PI=3.14
来源：http://xg.521024.cn

[R04] 位置参数
来源：http://im.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fw.yuntaijiaju.cn

[R05] 参数默认值
来源：http://hr.yuexingan06.cn

name="${1:-default}"
来源：http://cf.9csxet.cn

[R06] 判断命令是否存在
来源：http://sa.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://my.huanxung.cn

[R07] if 判断文件
来源：http://pm.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bs.hahajie.cn

[R08] 数值比较
来源：http://if.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zc.hnjuh.cn

[R09] 字符串比较
来源：http://pp.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pc.bjjhwx.cn

[R10] 正则匹配
来源：http://xx.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ae.chemitech.net.cn

[R11] case 多分支
来源：http://qi.gzmigu.cn

case "$1" in
来源：http://em.wgjwhj.cn

start) echo "启动" ;;
来源：http://mo.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://dq.521024.cn

*)     echo "未知命令" ;;
来源：http://ga.nicolike.cn

esac
来源：http://ru.shxzskj.cn

[R12] for 遍历文件
来源：http://ou.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://mt.bjjhwx.cn

[R13] for 计数循环
来源：http://bh.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ok.nicolike.cn

[R14] C 风格 for
来源：http://oq.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dr.szxytkj.cn

[R15] while 逐行读文件
来源：http://ud.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rb.bjjhwx.cn

[R16] until 等待条件
来源：http://hh.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cz.newstarts.cn

[R17] 数组定义与取值
来源：http://dy.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hd.newstarts.cn

[R18] 遍历数组
来源：http://ix.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sy.colortex.cn

[R19] 数组长度
来源：http://hg.shtwfgs.cn

echo "${#arr[@]}"
来源：http://as.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://wi.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sh.jianghongdianzi.cn

[R21] 字符串长度
来源：http://om.jctech888.com.cn

echo "${#s}"
来源：http://tk.muxihuayi.cn

[R22] 截取子串
来源：http://ba.9csxet.cn

echo "${s:0:5}"
来源：http://jc.shxzukj.cn

[R23] 字符串替换
来源：http://to.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://db.shxzskj.cn

[R24] 大小写转换
来源：http://tf.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xb.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://wz.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hp.szsharing.cn

[R26] 命令替换
来源：http://es.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://wp.szxytkj.cn

[R27] 算术展开
来源：http://zy.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://iq.asd995.cn

[R28] 浮点运算
来源：http://oz.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://mf.shtwfgs.cn

[R29] 定义函数
来源：http://yv.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tu.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://as.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://ey.newstarts.cn

[R31] 局部变量
来源：http://bm.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://wk.huixiangedu.cn

[R32] 参数个数校验
来源：http://cy.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bq.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://gm.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ad.shxzukj.cn

[R34] 退出时清理
来源：http://eb.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fb.panjiajie.cn

[R35] 后台执行并等待
来源：http://xd.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://is.hnjuh.cn

[R36] 并发执行多个任务
来源：http://vx.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fv.nszjky.cn

[R37] 把输出赋给变量
来源：http://gn.hahajie.cn

files=$(ls -1)
来源：http://zc.panjiajie.cn

[R38] 管道串联
来源：http://cl.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://pi.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://xl.huixiangedu.cn

cmd > out.log 2>&1
来源：http://wz.yuexingan06.cn

[R40] 追加写日志
来源：http://ma.newstarts.cn

echo "log" >> out.log
来源：http://un.panjiajie.cn

[R41] 丢弃输出
来源：http://fo.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://xq.jctech888.com.cn

[R42] 输入重定向
来源：http://bc.huixiangedu.cn

wc -l < a.txt
来源：http://yt.colortex.cn

[R43] 按名字查找文件
来源：http://lf.shxzukj.cn

find . -name "*.log" -type f
来源：http://gq.hnjuh.cn

[R44] 按修改时间查找
来源：http://bj.szxytkj.cn

find . -mtime -7 -type f
来源：http://wf.shxzskj.cn

[R45] 批量删除
来源：http://it.nszjky.cn

find . -name "*.tmp" -delete
来源：http://oo.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://sa.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lp.asd995.cn

[R47] sed 单行替换
来源：http://oc.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ni.colortex.cn

[R48] awk 取指定列
来源：http://ya.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://cj.9csxet.cn

[R49] awk 带条件
来源：http://fz.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://af.bjjhwx.cn

[R50] awk 求和
来源：http://jk.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fd.shtwfgs.cn

[R51] 排序去重取前几
来源：http://nv.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tf.bjjhwx.cn

[R52] 统计行数
来源：http://yy.hahajie.cn

wc -l a.txt
来源：http://tp.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://by.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ug.shtwfgs.cn

[R54] 比较两个文件
来源：http://ky.szxytkj.cn

diff a.txt b.txt
来源：http://cl.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://tz.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://di.szxytkj.cn

[R56] 远程拷贝
来源：http://oc.szsharing.cn

scp file user@host:/path/
来源：http://yd.huixiangedu.cn

[R57] 远程执行命令
来源：http://tw.nicolike.cn

ssh user@host 'uptime'
来源：http://kq.yuntaijiaju.cn

[R58] 下载文件
来源：http://pj.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sh.nicolike.cn

[R59] 发 POST JSON
来源：http://kj.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://db.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ph.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ek.wgjwhj.cn

[R61] 磁盘占用
来源：http://jt.bookmarksfly.cn

df -h;  du -sh *
来源：http://pd.panjiajie.cn

[R62] 找最占空间的文件
来源：http://kq.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://ey.colortex.cn

[R63] 内存与进程
来源：http://mg.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://zz.huanxung.cn

[R64] 结束进程
来源：http://re.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://fr.521024.cn

[R65] 查看端口占用
来源：http://qk.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ok.asd995.cn

[R66] 定时任务
来源：http://lo.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://pn.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://kz.bookmarksfly.cn

openssl rand -hex 16
来源：http://oj.bjjhwx.cn

[R68] 计算文件校验值
来源：http://bz.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zz.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://ro.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://wb.huixiangedu.cn

[R70] 时间戳与互转
来源：http://ld.szsharing.cn

date +%s;  date -d @1700000000
来源：http://us.521024.cn

[R71] 日期格式化
来源：http://hh.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uh.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://oe.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://os.yuntaijiaju.cn

[R73] 分割大日志
来源：http://qp.chemitech.net.cn

split -l 1000 big.log part_
来源：http://jj.asd995.cn

[R74] 批量重命名
来源：http://ft.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hm.haigaiapp.cn

[R75] 导出环境变量
来源：http://qu.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://fl.hnjuh.cn

[R76] 使用临时文件
来源：http://zb.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://or.huixiangedu.cn

[R77] 读取用户输入
来源：http://yg.shxzukj.cn

read -rp "请输入: " ans
来源：http://xe.nszjky.cn

[R78] 交互式菜单
来源：http://dm.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://aa.szsharing.cn

[R79] 解析命令行选项
来源：http://vv.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uq.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://zf.colortex.cn

time ./run.sh
来源：http://qq.shtwfgs.cn

================================================================================
来源：http://zx.bjjhwx.cn

S. C / C++ 专题
来源：http://md.yuexingan06.cn

================================================================================
来源：http://ro.yuntaijiaju.cn

[S01] C：Hello World
来源：http://uc.lnxyls.cn

#include <stdio.h>
来源：http://pv.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vf.newstarts.cn

[S02] C：变量与格式化输出
来源：http://sx.521024.cn

int a = 10; printf("%d\n", a);
来源：http://nc.yuntaijiaju.cn

[S03] C：读入整数
来源：http://jp.9csxet.cn

int x; scanf("%d", &x);
来源：http://ut.newstarts.cn

[S04] C：字符串复制
来源：http://bt.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://en.panjiajie.cn

[S05] C：字符串长度
来源：http://qt.huanxung.cn

strlen(s)
来源：http://uy.yuexingan06.cn

[S06] C：字符串比较
来源：http://tv.shxzukj.cn

strcmp(a, b) == 0
来源：http://bp.nicolike.cn

[S07] C：数组遍历求和
来源：http://nq.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mj.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://ev.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ac.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://km.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fp.shxzukj.cn

[S10] C：指针与解引用
来源：http://hw.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://sk.shtwfgs.cn

[S11] C：逐行读文件
来源：http://rh.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://pa.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hr.nicolike.cn

fclose(f);
来源：http://lp.9csxet.cn

[S12] C：写文件
来源：http://cc.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wp.szsharing.cn

[S13] C：宏定义
来源：http://yb.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tb.newstarts.cn

[S14] C：枚举
来源：http://zn.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://sf.yuntaijiaju.cn

[S15] C：类型转换
来源：http://ml.jianghongdianzi.cn

(double) a / b
来源：http://fz.huanxung.cn

[S16] C：位操作置位
来源：http://ti.szxytkj.cn

x |= (1 << 3);
来源：http://hu.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://ej.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jv.asd995.cn

[S18] C：命令行参数
来源：http://xp.haigaiapp.cn

int main(int argc, char **argv)
来源：http://uu.yuexingan06.cn

[S19] C：快速排序
来源：http://gr.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ot.hnjuh.cn

[S20] C：二分查找
来源：http://od.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tt.wgjwhj.cn

[S21] C：字符类别判断
来源：http://zl.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qr.huanxung.cn

[S22] C：字符串转数字
来源：http://dq.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ou.colortex.cn

[S23] C：随机数
来源：http://rx.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gp.jctech888.com.cn

[S24] C：获取本地时间
来源：http://xe.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ey.bjjhwx.cn

[S25] C：内存拷贝
来源：http://mc.huixiangedu.cn

memcpy(dst, src, n);
来源：http://uz.nicolike.cn

[S26] C：内存清零
来源：http://lz.9csxet.cn

memset(a, 0, sizeof a);
来源：http://lp.bookmarksfly.cn

[S27] C：定义常量
来源：http://xt.szsharing.cn

const double PI = 3.14159;
来源：http://wd.lnxyls.cn

[S28] C：静态变量
来源：http://gi.521024.cn

static int counter = 0;
来源：http://al.huanxung.cn

[S29] C：变参函数
来源：http://jb.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zs.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://vr.huanxung.cn

#ifndef X_H
来源：http://uw.haigaiapp.cn

#define X_H
来源：http://ki.panjiajie.cn

#endif
来源：http://mh.asd995.cn

[S31] C++：Hello World
来源：http://bk.haigaiapp.cn

#include <iostream>
来源：http://ei.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://ih.wgjwhj.cn

[S32] C++：字符串
来源：http://gr.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://pe.9csxet.cn

[S33] C++：vector 增删
来源：http://ks.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bp.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://tv.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://bq.chemitech.net.cn

[S35] C++：map
来源：http://yk.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://we.jctech888.com.cn

[S36] C++：unordered_map
来源：http://yf.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gb.nicolike.cn

[S37] C++：set
来源：http://kj.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sv.bjjhwx.cn

[S38] C++：排序
来源：http://bh.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://mx.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://rm.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eb.asd995.cn

[S40] C++：查找元素
来源：http://xy.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hx.9csxet.cn

[S41] C++：类与构造函数
来源：http://fe.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sg.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://lq.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://pw.9csxet.cn

[S43] C++：智能指针
来源：http://yv.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://lb.shxzukj.cn

[S44] C++：引用传参
来源：http://th.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://lb.newstarts.cn

[S45] C++：lambda
来源：http://xg.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yq.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://kq.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gq.wgjwhj.cn


<!-- 参考信息 -->