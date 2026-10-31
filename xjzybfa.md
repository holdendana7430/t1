代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hn.hnjuh.cn

[Q75] 日期格式化
来源：http://rx.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ge.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dt.bjjhwx.cn

[Q76] 按天统计
来源：http://ty.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://co.szsharing.cn

[Q77] 时间加减
来源：http://sw.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ou.huixiangedu.cn

[Q78] 当前时间
来源：http://wy.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://or.szsharing.cn

[Q79] 字符串拼接
来源：http://vy.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mx.huanxung.cn

[Q80] 字符串截取
来源：http://ru.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cq.colortex.cn

[Q81] 字符串替换
来源：http://kh.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bd.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://kz.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tp.shtwfgs.cn

[Q83] 大小写转换
来源：http://ux.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zp.huanxung.cn

[Q84] 去除首尾空格
来源：http://ui.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://kk.jianghongdianzi.cn

[Q85] 数值取整
来源：http://xj.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fq.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://iq.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ge.nszjky.cn

[Q87] JSON 字段做条件
来源：http://nx.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oo.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://hg.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fq.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ut.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://ze.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://as.panjiajie.cn

[Q90] 生成序号列
来源：http://jx.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://by.chemitech.net.cn

================================================================================
来源：http://nt.panjiajie.cn

R. Bash 专题
来源：http://yo.haigaiapp.cn

================================================================================
来源：http://ou.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://la.521024.cn

#!/usr/bin/env bash
来源：http://lm.newstarts.cn

set -euo pipefail
来源：http://ii.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://uy.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://vd.huixiangedu.cn

[R03] 只读变量
来源：http://qq.huixinmuqiang.cn

readonly PI=3.14
来源：http://ft.lnxyls.cn

[R04] 位置参数
来源：http://nv.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yp.yuexingan06.cn

[R05] 参数默认值
来源：http://ud.yuexingan06.cn

name="${1:-default}"
来源：http://fo.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://vw.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wt.521024.cn

[R07] if 判断文件
来源：http://ua.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tw.wgjwhj.cn

[R08] 数值比较
来源：http://jk.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zu.colortex.cn

[R09] 字符串比较
来源：http://hg.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iq.shtwfgs.cn

[R10] 正则匹配
来源：http://wn.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ph.lnxyls.cn

[R11] case 多分支
来源：http://sa.521024.cn

case "$1" in
来源：http://mt.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://bo.nicolike.cn

stop)  echo "停止" ;;
来源：http://mx.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://kx.szsharing.cn

esac
来源：http://gu.huixiangedu.cn

[R12] for 遍历文件
来源：http://xe.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://cg.chemitech.net.cn

[R13] for 计数循环
来源：http://fr.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://yu.huixinmuqiang.cn

[R14] C 风格 for
来源：http://bj.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xh.jctech888.com.cn

[R15] while 逐行读文件
来源：http://bt.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xh.chemitech.net.cn

[R16] until 等待条件
来源：http://yn.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://al.szsharing.cn

[R17] 数组定义与取值
来源：http://vf.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zx.haigaiapp.cn

[R18] 遍历数组
来源：http://mm.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vg.lnxyls.cn

[R19] 数组长度
来源：http://bd.newstarts.cn

echo "${#arr[@]}"
来源：http://nd.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://mu.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ms.shtwfgs.cn

[R21] 字符串长度
来源：http://qd.521024.cn

echo "${#s}"
来源：http://gm.szxytkj.cn

[R22] 截取子串
来源：http://kd.szxytkj.cn

echo "${s:0:5}"
来源：http://zs.huixinmuqiang.cn

[R23] 字符串替换
来源：http://cm.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oj.shxzukj.cn

[R24] 大小写转换
来源：http://be.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cd.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://uo.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ec.jctech888.com.cn

[R26] 命令替换
来源：http://kj.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://zn.521024.cn

[R27] 算术展开
来源：http://gr.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://cr.bookmarksfly.cn

[R28] 浮点运算
来源：http://nm.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ns.huanxung.cn

[R29] 定义函数
来源：http://wc.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qv.szsharing.cn

[R30] 函数返回状态码
来源：http://zt.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ag.chemitech.net.cn

[R31] 局部变量
来源：http://hk.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://dn.chemitech.net.cn

[R32] 参数个数校验
来源：http://nq.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://le.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://cu.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jk.wgjwhj.cn

[R34] 退出时清理
来源：http://rc.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bs.panjiajie.cn

[R35] 后台执行并等待
来源：http://th.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qv.szsharing.cn

[R36] 并发执行多个任务
来源：http://ps.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ij.shxzskj.cn

[R37] 把输出赋给变量
来源：http://qs.hnjuh.cn

files=$(ls -1)
来源：http://pb.yuexingan06.cn

[R38] 管道串联
来源：http://oj.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://vo.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://fq.hnjuh.cn

cmd > out.log 2>&1
来源：http://ay.hnjuh.cn

[R40] 追加写日志
来源：http://uq.hnjuh.cn

echo "log" >> out.log
来源：http://fm.panjiajie.cn

[R41] 丢弃输出
来源：http://wt.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://gh.hahajie.cn

[R42] 输入重定向
来源：http://cn.wgjwhj.cn

wc -l < a.txt
来源：http://ig.jctech888.com.cn

[R43] 按名字查找文件
来源：http://hn.newstarts.cn

find . -name "*.log" -type f
来源：http://vx.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://sa.colortex.cn

find . -mtime -7 -type f
来源：http://cz.shtwfgs.cn

[R45] 批量删除
来源：http://nz.nicolike.cn

find . -name "*.tmp" -delete
来源：http://dx.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://ei.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mp.huixiangedu.cn

[R47] sed 单行替换
来源：http://wx.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bo.9csxet.cn

[R48] awk 取指定列
来源：http://tz.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://pj.nicolike.cn

[R49] awk 带条件
来源：http://uf.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sq.yuntaijiaju.cn

[R50] awk 求和
来源：http://ml.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bc.szsharing.cn

[R51] 排序去重取前几
来源：http://xw.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ui.szxytkj.cn

[R52] 统计行数
来源：http://ff.bjjhwx.cn

wc -l a.txt
来源：http://db.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://md.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ry.shxzskj.cn

[R54] 比较两个文件
来源：http://st.521024.cn

diff a.txt b.txt
来源：http://kn.huixiangedu.cn

[R55] 压缩与解压
来源：http://rj.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qs.yuexingan06.cn

[R56] 远程拷贝
来源：http://fh.nicolike.cn

scp file user@host:/path/
来源：http://dw.nszjky.cn

[R57] 远程执行命令
来源：http://mp.521024.cn

ssh user@host 'uptime'
来源：http://sf.wgjwhj.cn

[R58] 下载文件
来源：http://pr.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jk.hnjuh.cn

[R59] 发 POST JSON
来源：http://ro.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mn.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://qz.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tn.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://nc.muxihuayi.cn

df -h;  du -sh *
来源：http://id.panjiajie.cn

[R62] 找最占空间的文件
来源：http://kd.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://ab.nicolike.cn

[R63] 内存与进程
来源：http://sd.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://ud.gzmigu.cn

[R64] 结束进程
来源：http://rc.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://oq.colortex.cn

[R65] 查看端口占用
来源：http://jo.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nc.521024.cn

[R66] 定时任务
来源：http://wh.haigaiapp.cn

crontab -e;  crontab -l
来源：http://wy.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://em.asd995.cn

openssl rand -hex 16
来源：http://kl.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://mo.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wb.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://tu.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://hr.szsharing.cn

[R70] 时间戳与互转
来源：http://fx.huanxung.cn

date +%s;  date -d @1700000000
来源：http://ao.hahajie.cn

[R71] 日期格式化
来源：http://ee.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zx.lnxyls.cn

[R72] 等待端口就绪
来源：http://fe.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://go.bjjhwx.cn

[R73] 分割大日志
来源：http://sn.shxzskj.cn

split -l 1000 big.log part_
来源：http://mq.wgjwhj.cn

[R74] 批量重命名
来源：http://wg.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wu.szxytkj.cn

[R75] 导出环境变量
来源：http://uw.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://le.panjiajie.cn

[R76] 使用临时文件
来源：http://dq.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fa.szsharing.cn

[R77] 读取用户输入
来源：http://as.9csxet.cn

read -rp "请输入: " ans
来源：http://es.hnjuh.cn

[R78] 交互式菜单
来源：http://bk.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://em.wgjwhj.cn

[R79] 解析命令行选项
来源：http://oj.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tl.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://zl.huixinmuqiang.cn

time ./run.sh
来源：http://fd.gzmigu.cn

================================================================================
来源：http://ym.szxytkj.cn

S. C / C++ 专题
来源：http://wo.muxihuayi.cn

================================================================================
来源：http://gl.huanxung.cn

[S01] C：Hello World
来源：http://gz.szsharing.cn

#include <stdio.h>
来源：http://gt.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bc.9csxet.cn

[S02] C：变量与格式化输出
来源：http://xl.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://ed.huixinmuqiang.cn

[S03] C：读入整数
来源：http://qs.nszjky.cn

int x; scanf("%d", &x);
来源：http://bi.panjiajie.cn

[S04] C：字符串复制
来源：http://et.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xj.nicolike.cn

[S05] C：字符串长度
来源：http://qr.huixinmuqiang.cn

strlen(s)
来源：http://rc.huanxung.cn

[S06] C：字符串比较
来源：http://jq.huanxung.cn

strcmp(a, b) == 0
来源：http://vr.shxzukj.cn

[S07] C：数组遍历求和
来源：http://bl.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xz.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://la.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sz.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://mz.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ma.hahajie.cn

[S10] C：指针与解引用
来源：http://cc.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://ac.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://tx.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://zq.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jw.szsharing.cn

fclose(f);
来源：http://ds.huixinmuqiang.cn

[S12] C：写文件
来源：http://sm.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ir.hnjuh.cn

[S13] C：宏定义
来源：http://kz.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ly.jianghongdianzi.cn

[S14] C：枚举
来源：http://dk.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ab.jianghongdianzi.cn

[S15] C：类型转换
来源：http://ci.bookmarksfly.cn

(double) a / b
来源：http://xn.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://rp.huixinmuqiang.cn

x |= (1 << 3);
来源：http://br.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://ld.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vl.szxytkj.cn

[S18] C：命令行参数
来源：http://bk.hnjuh.cn

int main(int argc, char **argv)
来源：http://hh.huanxung.cn

[S19] C：快速排序
来源：http://xt.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://le.hahajie.cn

[S20] C：二分查找
来源：http://zx.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jy.panjiajie.cn

[S21] C：字符类别判断
来源：http://jv.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cr.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://st.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dr.szxytkj.cn

[S23] C：随机数
来源：http://ea.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://aa.nicolike.cn

[S24] C：获取本地时间
来源：http://kd.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ha.newstarts.cn

[S25] C：内存拷贝
来源：http://dk.szsharing.cn

memcpy(dst, src, n);
来源：http://dz.bookmarksfly.cn

[S26] C：内存清零
来源：http://ty.huanxung.cn

memset(a, 0, sizeof a);
来源：http://wi.shtwfgs.cn

[S27] C：定义常量
来源：http://mk.colortex.cn

const double PI = 3.14159;
来源：http://rt.panjiajie.cn

[S28] C：静态变量
来源：http://mg.gzmigu.cn

static int counter = 0;
来源：http://gp.szxytkj.cn

[S29] C：变参函数
来源：http://pz.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wc.wgjwhj.cn

[S30] C：头文件保护
来源：http://iw.yuexingan06.cn

#ifndef X_H
来源：http://bm.gzmigu.cn

#define X_H
来源：http://cm.lnxyls.cn

#endif
来源：http://gr.bookmarksfly.cn

[S31] C++：Hello World
来源：http://vo.yuntaijiaju.cn

#include <iostream>
来源：http://mn.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://iv.521024.cn

[S32] C++：字符串
来源：http://nh.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://af.bjjhwx.cn

[S33] C++：vector 增删
来源：http://pf.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ok.nszjky.cn

[S34] C++：遍历 vector
来源：http://kl.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://az.haigaiapp.cn

[S35] C++：map
来源：http://ym.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ef.huixiangedu.cn

[S36] C++：unordered_map
来源：http://vx.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vo.lnxyls.cn

[S37] C++：set
来源：http://zu.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ra.panjiajie.cn

[S38] C++：排序
来源：http://ar.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://lt.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://db.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yg.shxzukj.cn

[S40] C++：查找元素
来源：http://ek.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dd.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://mm.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zp.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://ps.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://fa.chemitech.net.cn

[S43] C++：智能指针
来源：http://hp.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://id.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://qc.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://ez.huixiangedu.cn


<!-- 参考信息 -->