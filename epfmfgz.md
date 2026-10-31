代发 wailian999

[Q76] 按天统计
来源：http://fk.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yx.shxzukj.cn

[Q77] 时间加减
来源：http://wm.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://re.9csxet.cn

[Q78] 当前时间
来源：http://rr.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ga.hahajie.cn

[Q79] 字符串拼接
来源：http://tz.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://th.gzmigu.cn

[Q80] 字符串截取
来源：http://jx.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gb.shxzskj.cn

[Q81] 字符串替换
来源：http://yn.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ls.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://co.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mp.huanxung.cn

[Q83] 大小写转换
来源：http://fk.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vo.gzmigu.cn

[Q84] 去除首尾空格
来源：http://pw.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://oc.panjiajie.cn

[Q85] 数值取整
来源：http://pw.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ym.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://mu.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xf.521024.cn

[Q87] JSON 字段做条件
来源：http://qo.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hu.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://fg.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wr.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rp.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://vu.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://en.szsharing.cn

[Q90] 生成序号列
来源：http://ir.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ek.shtwfgs.cn

================================================================================
来源：http://gy.colortex.cn

R. Bash 专题
来源：http://xo.yuntaijiaju.cn

================================================================================
来源：http://it.nicolike.cn

[R01] shebang 与严格模式
来源：http://iy.asd995.cn

#!/usr/bin/env bash
来源：http://xi.huixinmuqiang.cn

set -euo pipefail
来源：http://eq.szxytkj.cn

[R02] 变量赋值与使用
来源：http://dx.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://zj.9csxet.cn

[R03] 只读变量
来源：http://ad.gzmigu.cn

readonly PI=3.14
来源：http://fy.yuexingan06.cn

[R04] 位置参数
来源：http://vp.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nv.yuntaijiaju.cn

[R05] 参数默认值
来源：http://lg.gzmigu.cn

name="${1:-default}"
来源：http://pp.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://wz.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ag.huixinmuqiang.cn

[R07] if 判断文件
来源：http://zj.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ey.huixiangedu.cn

[R08] 数值比较
来源：http://kv.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vc.asd995.cn

[R09] 字符串比较
来源：http://rb.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oi.shxzukj.cn

[R10] 正则匹配
来源：http://vm.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uo.huanxung.cn

[R11] case 多分支
来源：http://bu.nicolike.cn

case "$1" in
来源：http://ir.lnxyls.cn

start) echo "启动" ;;
来源：http://gx.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://xw.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://ud.huixinmuqiang.cn

esac
来源：http://kr.hahajie.cn

[R12] for 遍历文件
来源：http://iv.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://te.wgjwhj.cn

[R13] for 计数循环
来源：http://wr.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://et.shxzskj.cn

[R14] C 风格 for
来源：http://vb.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jm.gzmigu.cn

[R15] while 逐行读文件
来源：http://xq.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://af.9csxet.cn

[R16] until 等待条件
来源：http://sc.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lw.nszjky.cn

[R17] 数组定义与取值
来源：http://pc.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hm.hahajie.cn

[R18] 遍历数组
来源：http://zs.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pa.jctech888.com.cn

[R19] 数组长度
来源：http://mi.nicolike.cn

echo "${#arr[@]}"
来源：http://aa.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://zo.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xg.yuexingan06.cn

[R21] 字符串长度
来源：http://xq.huanxung.cn

echo "${#s}"
来源：http://fx.colortex.cn

[R22] 截取子串
来源：http://ul.gzmigu.cn

echo "${s:0:5}"
来源：http://sr.9csxet.cn

[R23] 字符串替换
来源：http://dm.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sc.bookmarksfly.cn

[R24] 大小写转换
来源：http://ns.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bv.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://tq.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dm.muxihuayi.cn

[R26] 命令替换
来源：http://xx.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://ck.hnjuh.cn

[R27] 算术展开
来源：http://aj.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://ca.muxihuayi.cn

[R28] 浮点运算
来源：http://eo.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://ey.gzmigu.cn

[R29] 定义函数
来源：http://ly.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fx.newstarts.cn

[R30] 函数返回状态码
来源：http://xc.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://xe.521024.cn

[R31] 局部变量
来源：http://eg.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://cn.huanxung.cn

[R32] 参数个数校验
来源：http://ee.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tq.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://pz.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kw.gzmigu.cn

[R34] 退出时清理
来源：http://vy.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ef.9csxet.cn

[R35] 后台执行并等待
来源：http://cc.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jf.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://nr.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sz.nicolike.cn

[R37] 把输出赋给变量
来源：http://yu.colortex.cn

files=$(ls -1)
来源：http://pv.asd995.cn

[R38] 管道串联
来源：http://ls.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://nn.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://za.jctech888.com.cn

cmd > out.log 2>&1
来源：http://ej.lnxyls.cn

[R40] 追加写日志
来源：http://jq.bookmarksfly.cn

echo "log" >> out.log
来源：http://ak.szsharing.cn

[R41] 丢弃输出
来源：http://mt.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://hb.colortex.cn

[R42] 输入重定向
来源：http://kz.nicolike.cn

wc -l < a.txt
来源：http://ut.asd995.cn

[R43] 按名字查找文件
来源：http://ph.huixiangedu.cn

find . -name "*.log" -type f
来源：http://qs.huanxung.cn

[R44] 按修改时间查找
来源：http://xy.newstarts.cn

find . -mtime -7 -type f
来源：http://ma.nicolike.cn

[R45] 批量删除
来源：http://bw.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://tp.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://jn.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://if.shxzukj.cn

[R47] sed 单行替换
来源：http://ry.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kg.huanxung.cn

[R48] awk 取指定列
来源：http://st.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://at.huixiangedu.cn

[R49] awk 带条件
来源：http://qh.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fy.9csxet.cn

[R50] awk 求和
来源：http://lm.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xo.haigaiapp.cn

[R51] 排序去重取前几
来源：http://qq.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kz.lnxyls.cn

[R52] 统计行数
来源：http://ei.shxzskj.cn

wc -l a.txt
来源：http://ck.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://gv.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://is.gzmigu.cn

[R54] 比较两个文件
来源：http://nu.bjjhwx.cn

diff a.txt b.txt
来源：http://ry.shtwfgs.cn

[R55] 压缩与解压
来源：http://ds.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wb.szxytkj.cn

[R56] 远程拷贝
来源：http://pb.huixiangedu.cn

scp file user@host:/path/
来源：http://uk.wgjwhj.cn

[R57] 远程执行命令
来源：http://ld.chemitech.net.cn

ssh user@host 'uptime'
来源：http://sp.9csxet.cn

[R58] 下载文件
来源：http://gu.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dn.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://zj.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dp.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://qz.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://li.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://zh.newstarts.cn

df -h;  du -sh *
来源：http://js.szsharing.cn

[R62] 找最占空间的文件
来源：http://mr.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://xk.bookmarksfly.cn

[R63] 内存与进程
来源：http://nq.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://yy.chemitech.net.cn

[R64] 结束进程
来源：http://xb.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://yr.hnjuh.cn

[R65] 查看端口占用
来源：http://ce.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fh.asd995.cn

[R66] 定时任务
来源：http://go.panjiajie.cn

crontab -e;  crontab -l
来源：http://jz.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://gc.jianghongdianzi.cn

openssl rand -hex 16
来源：http://qm.nszjky.cn

[R68] 计算文件校验值
来源：http://at.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wt.haigaiapp.cn

[R69] 生成随机密码
来源：http://al.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://mm.szxytkj.cn

[R70] 时间戳与互转
来源：http://jl.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://tc.521024.cn

[R71] 日期格式化
来源：http://ii.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sp.9csxet.cn

[R72] 等待端口就绪
来源：http://mq.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gj.yuntaijiaju.cn

[R73] 分割大日志
来源：http://lh.jctech888.com.cn

split -l 1000 big.log part_
来源：http://lw.panjiajie.cn

[R74] 批量重命名
来源：http://lx.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ip.yuexingan06.cn

[R75] 导出环境变量
来源：http://eq.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://sn.asd995.cn

[R76] 使用临时文件
来源：http://pw.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pp.wgjwhj.cn

[R77] 读取用户输入
来源：http://tf.hahajie.cn

read -rp "请输入: " ans
来源：http://tg.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://uy.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ee.nicolike.cn

[R79] 解析命令行选项
来源：http://yo.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mc.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://oe.jianghongdianzi.cn

time ./run.sh
来源：http://xf.panjiajie.cn

================================================================================
来源：http://cj.shxzskj.cn

S. C / C++ 专题
来源：http://wr.huixiangedu.cn

================================================================================
来源：http://et.bookmarksfly.cn

[S01] C：Hello World
来源：http://hi.wgjwhj.cn

#include <stdio.h>
来源：http://of.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ex.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://hl.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://eb.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ar.9csxet.cn

int x; scanf("%d", &x);
来源：http://ia.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://rw.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vm.szxytkj.cn

[S05] C：字符串长度
来源：http://ik.wgjwhj.cn

strlen(s)
来源：http://ag.wgjwhj.cn

[S06] C：字符串比较
来源：http://wu.huanxung.cn

strcmp(a, b) == 0
来源：http://wb.newstarts.cn

[S07] C：数组遍历求和
来源：http://nd.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dp.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://hh.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nu.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://go.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nl.szsharing.cn

[S10] C：指针与解引用
来源：http://jk.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://bt.muxihuayi.cn

[S11] C：逐行读文件
来源：http://og.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://sq.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://um.asd995.cn

fclose(f);
来源：http://bk.nicolike.cn

[S12] C：写文件
来源：http://mx.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ju.asd995.cn

[S13] C：宏定义
来源：http://jp.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dc.haigaiapp.cn

[S14] C：枚举
来源：http://di.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://sb.colortex.cn

[S15] C：类型转换
来源：http://mr.9csxet.cn

(double) a / b
来源：http://ug.newstarts.cn

[S16] C：位操作置位
来源：http://yn.shtwfgs.cn

x |= (1 << 3);
来源：http://tg.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://om.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eb.hahajie.cn

[S18] C：命令行参数
来源：http://uq.hnjuh.cn

int main(int argc, char **argv)
来源：http://pv.panjiajie.cn

[S19] C：快速排序
来源：http://yg.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ky.lnxyls.cn

[S20] C：二分查找
来源：http://lh.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ci.521024.cn

[S21] C：字符类别判断
来源：http://kl.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fo.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://io.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ok.hnjuh.cn

[S23] C：随机数
来源：http://xv.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cx.panjiajie.cn

[S24] C：获取本地时间
来源：http://js.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hf.szxytkj.cn

[S25] C：内存拷贝
来源：http://jn.huanxung.cn

memcpy(dst, src, n);
来源：http://ja.jianghongdianzi.cn

[S26] C：内存清零
来源：http://ba.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://uf.huixinmuqiang.cn

[S27] C：定义常量
来源：http://my.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://ne.yuntaijiaju.cn

[S28] C：静态变量
来源：http://tu.wgjwhj.cn

static int counter = 0;
来源：http://ec.wgjwhj.cn

[S29] C：变参函数
来源：http://fe.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yb.521024.cn

[S30] C：头文件保护
来源：http://ci.colortex.cn

#ifndef X_H
来源：http://uq.nszjky.cn

#define X_H
来源：http://ly.521024.cn

#endif
来源：http://it.gzmigu.cn

[S31] C++：Hello World
来源：http://zg.bjjhwx.cn

#include <iostream>
来源：http://ba.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://em.gzmigu.cn

[S32] C++：字符串
来源：http://em.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://by.bjjhwx.cn

[S33] C++：vector 增删
来源：http://su.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ph.szsharing.cn

[S34] C++：遍历 vector
来源：http://iy.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://nr.yuntaijiaju.cn

[S35] C++：map
来源：http://vu.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fn.9csxet.cn

[S36] C++：unordered_map
来源：http://tm.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nn.521024.cn

[S37] C++：set
来源：http://yy.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vi.nszjky.cn

[S38] C++：排序
来源：http://ua.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://il.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://ue.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sf.9csxet.cn

[S40] C++：查找元素
来源：http://ro.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vy.gzmigu.cn

[S41] C++：类与构造函数
来源：http://fw.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ob.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://av.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://se.wgjwhj.cn

[S43] C++：智能指针
来源：http://di.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://jd.nicolike.cn

[S44] C++：引用传参
来源：http://ph.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://lv.nicolike.cn

[S45] C++：lambda
来源：http://cq.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bf.huixiangedu.cn

[S46] C++：函数模板
来源：http://cd.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jc.newstarts.cn


<!-- 参考信息 -->