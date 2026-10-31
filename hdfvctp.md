代发 wailian999

[Q76] 按天统计
来源：http://ru.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ps.panjiajie.cn

[Q77] 时间加减
来源：http://xx.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fs.szxytkj.cn

[Q78] 当前时间
来源：http://ht.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pa.chemitech.net.cn

[Q79] 字符串拼接
来源：http://yd.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tv.newstarts.cn

[Q80] 字符串截取
来源：http://ak.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fn.jctech888.com.cn

[Q81] 字符串替换
来源：http://sq.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jd.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://cw.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ob.huixiangedu.cn

[Q83] 大小写转换
来源：http://hl.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ux.lnxyls.cn

[Q84] 去除首尾空格
来源：http://hs.521024.cn

SELECT TRIM(name) FROM users;
来源：http://mq.bjjhwx.cn

[Q85] 数值取整
来源：http://ep.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hm.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://mo.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aq.9csxet.cn

[Q87] JSON 字段做条件
来源：http://tn.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vf.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://da.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wc.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uo.hnjuh.cn

[Q89] 判断表是否存在
来源：http://vo.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fc.szxytkj.cn

[Q90] 生成序号列
来源：http://ir.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lw.lnxyls.cn

================================================================================
来源：http://bc.nicolike.cn

R. Bash 专题
来源：http://oe.jctech888.com.cn

================================================================================
来源：http://ui.shxzukj.cn

[R01] shebang 与严格模式
来源：http://zh.newstarts.cn

#!/usr/bin/env bash
来源：http://wg.muxihuayi.cn

set -euo pipefail
来源：http://ob.asd995.cn

[R02] 变量赋值与使用
来源：http://xs.huanxung.cn

name="Tom"; echo "$name"
来源：http://kt.chemitech.net.cn

[R03] 只读变量
来源：http://gq.newstarts.cn

readonly PI=3.14
来源：http://rn.wgjwhj.cn

[R04] 位置参数
来源：http://rg.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ax.bookmarksfly.cn

[R05] 参数默认值
来源：http://se.hnjuh.cn

name="${1:-default}"
来源：http://tz.asd995.cn

[R06] 判断命令是否存在
来源：http://pq.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uz.asd995.cn

[R07] if 判断文件
来源：http://gu.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cm.521024.cn

[R08] 数值比较
来源：http://ro.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rn.hahajie.cn

[R09] 字符串比较
来源：http://qa.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fo.yuntaijiaju.cn

[R10] 正则匹配
来源：http://uj.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ep.nicolike.cn

[R11] case 多分支
来源：http://vw.huanxung.cn

case "$1" in
来源：http://il.bookmarksfly.cn

start) echo "启动" ;;
来源：http://gw.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://rb.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://rh.szsharing.cn

esac
来源：http://nn.haigaiapp.cn

[R12] for 遍历文件
来源：http://um.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://kj.gzmigu.cn

[R13] for 计数循环
来源：http://or.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://nv.huixiangedu.cn

[R14] C 风格 for
来源：http://ig.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wx.lnxyls.cn

[R15] while 逐行读文件
来源：http://zs.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://li.asd995.cn

[R16] until 等待条件
来源：http://ld.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sj.panjiajie.cn

[R17] 数组定义与取值
来源：http://yk.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aj.wgjwhj.cn

[R18] 遍历数组
来源：http://is.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iw.jianghongdianzi.cn

[R19] 数组长度
来源：http://pq.panjiajie.cn

echo "${#arr[@]}"
来源：http://bi.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://fc.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sf.newstarts.cn

[R21] 字符串长度
来源：http://vp.hahajie.cn

echo "${#s}"
来源：http://nv.nszjky.cn

[R22] 截取子串
来源：http://da.shxzukj.cn

echo "${s:0:5}"
来源：http://ov.shtwfgs.cn

[R23] 字符串替换
来源：http://xt.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sg.colortex.cn

[R24] 大小写转换
来源：http://ht.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://db.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://jp.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://na.colortex.cn

[R26] 命令替换
来源：http://ch.colortex.cn

now=$(date +%F); echo "$now"
来源：http://st.hahajie.cn

[R27] 算术展开
来源：http://ek.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://qu.hnjuh.cn

[R28] 浮点运算
来源：http://ld.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://kx.bjjhwx.cn

[R29] 定义函数
来源：http://bn.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://by.nszjky.cn

[R30] 函数返回状态码
来源：http://rt.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://wh.szxytkj.cn

[R31] 局部变量
来源：http://qy.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://wk.wgjwhj.cn

[R32] 参数个数校验
来源：http://kz.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nq.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://cm.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rr.huanxung.cn

[R34] 退出时清理
来源：http://ks.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sw.szsharing.cn

[R35] 后台执行并等待
来源：http://gf.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fz.shxzskj.cn

[R36] 并发执行多个任务
来源：http://aw.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aw.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://pp.wgjwhj.cn

files=$(ls -1)
来源：http://kp.muxihuayi.cn

[R38] 管道串联
来源：http://jp.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://bu.521024.cn

[R39] 重定向标准输出与错误
来源：http://qw.huixiangedu.cn

cmd > out.log 2>&1
来源：http://ks.jctech888.com.cn

[R40] 追加写日志
来源：http://ej.521024.cn

echo "log" >> out.log
来源：http://bv.chemitech.net.cn

[R41] 丢弃输出
来源：http://oe.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://yq.lnxyls.cn

[R42] 输入重定向
来源：http://bb.huixiangedu.cn

wc -l < a.txt
来源：http://hn.huixiangedu.cn

[R43] 按名字查找文件
来源：http://py.szxytkj.cn

find . -name "*.log" -type f
来源：http://vj.9csxet.cn

[R44] 按修改时间查找
来源：http://ge.huixiangedu.cn

find . -mtime -7 -type f
来源：http://xg.colortex.cn

[R45] 批量删除
来源：http://gr.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://lg.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://vf.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://el.shxzskj.cn

[R47] sed 单行替换
来源：http://vg.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jg.wgjwhj.cn

[R48] awk 取指定列
来源：http://og.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://cc.gzmigu.cn

[R49] awk 带条件
来源：http://bh.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://br.shtwfgs.cn

[R50] awk 求和
来源：http://zi.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wt.yuexingan06.cn

[R51] 排序去重取前几
来源：http://hw.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ze.huanxung.cn

[R52] 统计行数
来源：http://ve.wgjwhj.cn

wc -l a.txt
来源：http://vf.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://hv.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jc.newstarts.cn

[R54] 比较两个文件
来源：http://jm.huixinmuqiang.cn

diff a.txt b.txt
来源：http://ac.shxzukj.cn

[R55] 压缩与解压
来源：http://dy.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uk.hahajie.cn

[R56] 远程拷贝
来源：http://vu.gzmigu.cn

scp file user@host:/path/
来源：http://ml.huixiangedu.cn

[R57] 远程执行命令
来源：http://jd.gzmigu.cn

ssh user@host 'uptime'
来源：http://me.gzmigu.cn

[R58] 下载文件
来源：http://tx.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ln.shxzukj.cn

[R59] 发 POST JSON
来源：http://sr.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ed.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://bm.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gy.huanxung.cn

[R61] 磁盘占用
来源：http://nt.newstarts.cn

df -h;  du -sh *
来源：http://by.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://gw.521024.cn

du -ah . | sort -rh | head -10
来源：http://op.panjiajie.cn

[R63] 内存与进程
来源：http://ta.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://nz.szsharing.cn

[R64] 结束进程
来源：http://lx.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://yo.muxihuayi.cn

[R65] 查看端口占用
来源：http://ct.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hu.huixiangedu.cn

[R66] 定时任务
来源：http://st.asd995.cn

crontab -e;  crontab -l
来源：http://mk.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://xg.bjjhwx.cn

openssl rand -hex 16
来源：http://kb.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://gg.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://is.wgjwhj.cn

[R69] 生成随机密码
来源：http://wk.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://sc.chemitech.net.cn

[R70] 时间戳与互转
来源：http://cj.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://wk.chemitech.net.cn

[R71] 日期格式化
来源：http://ba.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tn.panjiajie.cn

[R72] 等待端口就绪
来源：http://qh.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uj.panjiajie.cn

[R73] 分割大日志
来源：http://is.wgjwhj.cn

split -l 1000 big.log part_
来源：http://rl.jianghongdianzi.cn

[R74] 批量重命名
来源：http://lu.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dl.hahajie.cn

[R75] 导出环境变量
来源：http://bz.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://hy.lnxyls.cn

[R76] 使用临时文件
来源：http://jt.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rg.huanxung.cn

[R77] 读取用户输入
来源：http://sy.521024.cn

read -rp "请输入: " ans
来源：http://rf.shxzukj.cn

[R78] 交互式菜单
来源：http://it.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://po.chemitech.net.cn

[R79] 解析命令行选项
来源：http://sf.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pw.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://ly.shxzskj.cn

time ./run.sh
来源：http://kk.bookmarksfly.cn

================================================================================
来源：http://ho.wgjwhj.cn

S. C / C++ 专题
来源：http://uz.hahajie.cn

================================================================================
来源：http://rf.hnjuh.cn

[S01] C：Hello World
来源：http://vi.nszjky.cn

#include <stdio.h>
来源：http://no.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sw.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://sz.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://wm.huixiangedu.cn

[S03] C：读入整数
来源：http://bp.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://oh.shtwfgs.cn

[S04] C：字符串复制
来源：http://yo.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ob.lnxyls.cn

[S05] C：字符串长度
来源：http://vg.hahajie.cn

strlen(s)
来源：http://cf.huanxung.cn

[S06] C：字符串比较
来源：http://en.gzmigu.cn

strcmp(a, b) == 0
来源：http://ki.shxzukj.cn

[S07] C：数组遍历求和
来源：http://vg.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ml.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://qt.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ts.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://sq.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ut.nszjky.cn

[S10] C：指针与解引用
来源：http://gs.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://up.wgjwhj.cn

[S11] C：逐行读文件
来源：http://qf.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://zj.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zi.muxihuayi.cn

fclose(f);
来源：http://qg.nszjky.cn

[S12] C：写文件
来源：http://io.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://au.szsharing.cn

[S13] C：宏定义
来源：http://zu.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bq.hahajie.cn

[S14] C：枚举
来源：http://gq.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://dq.nszjky.cn

[S15] C：类型转换
来源：http://jz.nicolike.cn

(double) a / b
来源：http://vj.jctech888.com.cn

[S16] C：位操作置位
来源：http://bu.nszjky.cn

x |= (1 << 3);
来源：http://bc.hahajie.cn

[S17] C：安全拼接字符串
来源：http://xa.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uv.haigaiapp.cn

[S18] C：命令行参数
来源：http://ds.lnxyls.cn

int main(int argc, char **argv)
来源：http://wo.huanxung.cn

[S19] C：快速排序
来源：http://wh.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ib.colortex.cn

[S20] C：二分查找
来源：http://gz.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dy.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://yo.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hu.newstarts.cn

[S22] C：字符串转数字
来源：http://io.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ya.jianghongdianzi.cn

[S23] C：随机数
来源：http://sd.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ln.lnxyls.cn

[S24] C：获取本地时间
来源：http://aj.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mc.chemitech.net.cn

[S25] C：内存拷贝
来源：http://xv.chemitech.net.cn

memcpy(dst, src, n);
来源：http://pt.huixinmuqiang.cn

[S26] C：内存清零
来源：http://qw.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://hq.lnxyls.cn

[S27] C：定义常量
来源：http://vm.muxihuayi.cn

const double PI = 3.14159;
来源：http://km.yuexingan06.cn

[S28] C：静态变量
来源：http://bx.huixinmuqiang.cn

static int counter = 0;
来源：http://kz.asd995.cn

[S29] C：变参函数
来源：http://zi.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hy.shtwfgs.cn

[S30] C：头文件保护
来源：http://ml.yuntaijiaju.cn

#ifndef X_H
来源：http://pn.nszjky.cn

#define X_H
来源：http://qz.colortex.cn

#endif
来源：http://gt.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://pt.9csxet.cn

#include <iostream>
来源：http://za.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://de.shxzukj.cn

[S32] C++：字符串
来源：http://pf.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://pr.haigaiapp.cn

[S33] C++：vector 增删
来源：http://vx.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mx.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://kd.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://dj.shtwfgs.cn

[S35] C++：map
来源：http://is.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jt.shtwfgs.cn

[S36] C++：unordered_map
来源：http://cl.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bi.colortex.cn

[S37] C++：set
来源：http://qy.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ec.jianghongdianzi.cn

[S38] C++：排序
来源：http://gp.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://iu.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://nk.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yu.nszjky.cn

[S40] C++：查找元素
来源：http://ax.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zq.shxzukj.cn

[S41] C++：类与构造函数
来源：http://aj.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nk.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://xg.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://up.shtwfgs.cn

[S43] C++：智能指针
来源：http://sw.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://ar.szsharing.cn

[S44] C++：引用传参
来源：http://bj.nicolike.cn

void inc(int &x) { ++x; }
来源：http://np.hahajie.cn

[S45] C++：lambda
来源：http://sv.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zq.asd995.cn

[S46] C++：函数模板
来源：http://ag.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bs.9csxet.cn


<!-- 参考信息 -->