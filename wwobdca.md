代发 wailian999

[Q76] 按天统计
来源：http://yw.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gn.jctech888.com.cn

[Q77] 时间加减
来源：http://jw.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sx.521024.cn

[Q78] 当前时间
来源：http://jj.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cp.colortex.cn

[Q79] 字符串拼接
来源：http://ln.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uq.shxzskj.cn

[Q80] 字符串截取
来源：http://ni.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hc.yuexingan06.cn

[Q81] 字符串替换
来源：http://yf.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ho.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://ov.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dc.asd995.cn

[Q83] 大小写转换
来源：http://om.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uc.hnjuh.cn

[Q84] 去除首尾空格
来源：http://sr.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://za.lnxyls.cn

[Q85] 数值取整
来源：http://dy.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pj.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://ry.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gf.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://hf.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kt.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://cv.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rp.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://so.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://jz.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ay.huixiangedu.cn

[Q90] 生成序号列
来源：http://nk.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hk.shxzskj.cn

================================================================================
来源：http://jv.colortex.cn

R. Bash 专题
来源：http://es.huixinmuqiang.cn

================================================================================
来源：http://rv.asd995.cn

[R01] shebang 与严格模式
来源：http://jq.huanxung.cn

#!/usr/bin/env bash
来源：http://cz.huixiangedu.cn

set -euo pipefail
来源：http://vr.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://tf.9csxet.cn

name="Tom"; echo "$name"
来源：http://eb.9csxet.cn

[R03] 只读变量
来源：http://dk.colortex.cn

readonly PI=3.14
来源：http://ws.jianghongdianzi.cn

[R04] 位置参数
来源：http://iz.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kt.bjjhwx.cn

[R05] 参数默认值
来源：http://ut.lnxyls.cn

name="${1:-default}"
来源：http://pa.9csxet.cn

[R06] 判断命令是否存在
来源：http://vz.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zi.bookmarksfly.cn

[R07] if 判断文件
来源：http://vu.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wr.nicolike.cn

[R08] 数值比较
来源：http://if.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yi.gzmigu.cn

[R09] 字符串比较
来源：http://tm.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mt.bookmarksfly.cn

[R10] 正则匹配
来源：http://uj.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xb.shxzskj.cn

[R11] case 多分支
来源：http://vk.shxzukj.cn

case "$1" in
来源：http://hs.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://vx.szsharing.cn

stop)  echo "停止" ;;
来源：http://qr.colortex.cn

*)     echo "未知命令" ;;
来源：http://uf.yuexingan06.cn

esac
来源：http://su.chemitech.net.cn

[R12] for 遍历文件
来源：http://gp.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://jv.bookmarksfly.cn

[R13] for 计数循环
来源：http://xv.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://km.lnxyls.cn

[R14] C 风格 for
来源：http://jm.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nf.lnxyls.cn

[R15] while 逐行读文件
来源：http://uo.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iy.yuntaijiaju.cn

[R16] until 等待条件
来源：http://be.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xj.asd995.cn

[R17] 数组定义与取值
来源：http://eo.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mo.szxytkj.cn

[R18] 遍历数组
来源：http://qu.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://el.huixinmuqiang.cn

[R19] 数组长度
来源：http://mi.bjjhwx.cn

echo "${#arr[@]}"
来源：http://ui.colortex.cn

[R20] 关联数组（字典）
来源：http://fi.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dw.9csxet.cn

[R21] 字符串长度
来源：http://dt.lnxyls.cn

echo "${#s}"
来源：http://xx.panjiajie.cn

[R22] 截取子串
来源：http://so.hnjuh.cn

echo "${s:0:5}"
来源：http://st.jctech888.com.cn

[R23] 字符串替换
来源：http://vk.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ts.nicolike.cn

[R24] 大小写转换
来源：http://es.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hg.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://ny.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://es.521024.cn

[R26] 命令替换
来源：http://ha.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://pv.gzmigu.cn

[R27] 算术展开
来源：http://sc.szsharing.cn

echo $((1 + 2 * 3))
来源：http://xg.nszjky.cn

[R28] 浮点运算
来源：http://ht.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://wz.nszjky.cn

[R29] 定义函数
来源：http://dk.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fi.bjjhwx.cn

[R30] 函数返回状态码
来源：http://ua.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://kh.szxytkj.cn

[R31] 局部变量
来源：http://tq.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://xv.asd995.cn

[R32] 参数个数校验
来源：http://mp.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sj.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://jq.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hy.521024.cn

[R34] 退出时清理
来源：http://wn.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pj.haigaiapp.cn

[R35] 后台执行并等待
来源：http://yt.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ef.szsharing.cn

[R36] 并发执行多个任务
来源：http://tp.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ot.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://zp.szsharing.cn

files=$(ls -1)
来源：http://gl.shtwfgs.cn

[R38] 管道串联
来源：http://pr.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://zw.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://id.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://xg.hahajie.cn

[R40] 追加写日志
来源：http://xm.chemitech.net.cn

echo "log" >> out.log
来源：http://np.nszjky.cn

[R41] 丢弃输出
来源：http://zd.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://ro.chemitech.net.cn

[R42] 输入重定向
来源：http://id.szsharing.cn

wc -l < a.txt
来源：http://zt.newstarts.cn

[R43] 按名字查找文件
来源：http://bs.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://fo.hahajie.cn

[R44] 按修改时间查找
来源：http://ci.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://ye.nicolike.cn

[R45] 批量删除
来源：http://so.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://vp.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://jq.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wg.bjjhwx.cn

[R47] sed 单行替换
来源：http://ds.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fs.lnxyls.cn

[R48] awk 取指定列
来源：http://mn.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://ba.szsharing.cn

[R49] awk 带条件
来源：http://pt.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kx.panjiajie.cn

[R50] awk 求和
来源：http://jm.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rd.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://iz.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cb.panjiajie.cn

[R52] 统计行数
来源：http://uh.shtwfgs.cn

wc -l a.txt
来源：http://fq.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://gw.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tm.hnjuh.cn

[R54] 比较两个文件
来源：http://zv.panjiajie.cn

diff a.txt b.txt
来源：http://xi.lnxyls.cn

[R55] 压缩与解压
来源：http://if.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gd.asd995.cn

[R56] 远程拷贝
来源：http://ma.newstarts.cn

scp file user@host:/path/
来源：http://sl.jctech888.com.cn

[R57] 远程执行命令
来源：http://sx.shxzskj.cn

ssh user@host 'uptime'
来源：http://qz.shtwfgs.cn

[R58] 下载文件
来源：http://gp.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yt.9csxet.cn

[R59] 发 POST JSON
来源：http://de.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wr.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://dx.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vw.9csxet.cn

[R61] 磁盘占用
来源：http://wi.jianghongdianzi.cn

df -h;  du -sh *
来源：http://mv.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://rw.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://pl.szsharing.cn

[R63] 内存与进程
来源：http://tl.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://md.jctech888.com.cn

[R64] 结束进程
来源：http://bn.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://ql.lnxyls.cn

[R65] 查看端口占用
来源：http://lq.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qw.shtwfgs.cn

[R66] 定时任务
来源：http://gt.huixiangedu.cn

crontab -e;  crontab -l
来源：http://ud.9csxet.cn

[R67] 生成随机十六进制串
来源：http://kn.colortex.cn

openssl rand -hex 16
来源：http://ib.jctech888.com.cn

[R68] 计算文件校验值
来源：http://hp.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ss.bookmarksfly.cn

[R69] 生成随机密码
来源：http://dl.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://vr.shxzukj.cn

[R70] 时间戳与互转
来源：http://pm.asd995.cn

date +%s;  date -d @1700000000
来源：http://iv.huixinmuqiang.cn

[R71] 日期格式化
来源：http://ov.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vt.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://me.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pb.nicolike.cn

[R73] 分割大日志
来源：http://zz.colortex.cn

split -l 1000 big.log part_
来源：http://qu.szxytkj.cn

[R74] 批量重命名
来源：http://lw.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fb.9csxet.cn

[R75] 导出环境变量
来源：http://ms.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://du.szxytkj.cn

[R76] 使用临时文件
来源：http://mz.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tp.yuexingan06.cn

[R77] 读取用户输入
来源：http://vi.muxihuayi.cn

read -rp "请输入: " ans
来源：http://kr.nicolike.cn

[R78] 交互式菜单
来源：http://gj.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dc.szxytkj.cn

[R79] 解析命令行选项
来源：http://sg.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zp.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://ig.szsharing.cn

time ./run.sh
来源：http://pz.hnjuh.cn

================================================================================
来源：http://vy.shxzukj.cn

S. C / C++ 专题
来源：http://zs.shtwfgs.cn

================================================================================
来源：http://nk.jianghongdianzi.cn

[S01] C：Hello World
来源：http://ql.gzmigu.cn

#include <stdio.h>
来源：http://pq.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xb.hahajie.cn

[S02] C：变量与格式化输出
来源：http://qj.521024.cn

int a = 10; printf("%d\n", a);
来源：http://lo.jianghongdianzi.cn

[S03] C：读入整数
来源：http://wv.521024.cn

int x; scanf("%d", &x);
来源：http://xg.shtwfgs.cn

[S04] C：字符串复制
来源：http://ka.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ed.szxytkj.cn

[S05] C：字符串长度
来源：http://nw.asd995.cn

strlen(s)
来源：http://qx.shtwfgs.cn

[S06] C：字符串比较
来源：http://zf.shxzukj.cn

strcmp(a, b) == 0
来源：http://le.panjiajie.cn

[S07] C：数组遍历求和
来源：http://bb.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://my.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://tb.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://co.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://yq.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gw.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://yd.szsharing.cn

int *p = &a;  *p = 5;
来源：http://qu.bjjhwx.cn

[S11] C：逐行读文件
来源：http://sz.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://ik.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qe.yuntaijiaju.cn

fclose(f);
来源：http://kw.szsharing.cn

[S12] C：写文件
来源：http://mi.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lc.bjjhwx.cn

[S13] C：宏定义
来源：http://dx.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sn.asd995.cn

[S14] C：枚举
来源：http://nn.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://zw.chemitech.net.cn

[S15] C：类型转换
来源：http://yk.nicolike.cn

(double) a / b
来源：http://hy.szxytkj.cn

[S16] C：位操作置位
来源：http://jg.gzmigu.cn

x |= (1 << 3);
来源：http://it.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://ie.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wl.shxzukj.cn

[S18] C：命令行参数
来源：http://to.huixiangedu.cn

int main(int argc, char **argv)
来源：http://tx.chemitech.net.cn

[S19] C：快速排序
来源：http://qm.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fz.szsharing.cn

[S20] C：二分查找
来源：http://zg.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yt.hnjuh.cn

[S21] C：字符类别判断
来源：http://jn.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wt.colortex.cn

[S22] C：字符串转数字
来源：http://fx.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vf.bookmarksfly.cn

[S23] C：随机数
来源：http://zk.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ab.bjjhwx.cn

[S24] C：获取本地时间
来源：http://ce.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ul.hnjuh.cn

[S25] C：内存拷贝
来源：http://yv.panjiajie.cn

memcpy(dst, src, n);
来源：http://to.bjjhwx.cn

[S26] C：内存清零
来源：http://qj.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://im.shxzskj.cn

[S27] C：定义常量
来源：http://ik.panjiajie.cn

const double PI = 3.14159;
来源：http://lp.jctech888.com.cn

[S28] C：静态变量
来源：http://ba.huixiangedu.cn

static int counter = 0;
来源：http://iy.yuexingan06.cn

[S29] C：变参函数
来源：http://af.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pk.hnjuh.cn

[S30] C：头文件保护
来源：http://ss.nszjky.cn

#ifndef X_H
来源：http://wt.chemitech.net.cn

#define X_H
来源：http://ut.lnxyls.cn

#endif
来源：http://ve.wgjwhj.cn

[S31] C++：Hello World
来源：http://gd.chemitech.net.cn

#include <iostream>
来源：http://xm.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://xv.hahajie.cn

[S32] C++：字符串
来源：http://gd.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://rb.huanxung.cn

[S33] C++：vector 增删
来源：http://cv.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://de.szsharing.cn

[S34] C++：遍历 vector
来源：http://te.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://kn.gzmigu.cn

[S35] C++：map
来源：http://nh.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zj.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://bk.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vn.yuexingan06.cn

[S37] C++：set
来源：http://ca.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aj.huixiangedu.cn

[S38] C++：排序
来源：http://iz.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://bt.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://ze.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ap.lnxyls.cn

[S40] C++：查找元素
来源：http://er.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ib.gzmigu.cn

[S41] C++：类与构造函数
来源：http://ws.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://op.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://td.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://ss.hnjuh.cn

[S43] C++：智能指针
来源：http://ak.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://hn.521024.cn

[S44] C++：引用传参
来源：http://kt.hahajie.cn

void inc(int &x) { ++x; }
来源：http://ae.yuexingan06.cn

[S45] C++：lambda
来源：http://jq.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zz.huanxung.cn

[S46] C++：函数模板
来源：http://bz.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ok.huixiangedu.cn


<!-- 参考信息 -->