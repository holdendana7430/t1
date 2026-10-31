代发 wailian999

SHOW INDEX FROM users;
来源：http://zm.szsharing.cn

[Q73] 查看表状态
来源：http://xv.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vc.szxytkj.cn

[Q74] 强制使用索引
来源：http://uv.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gj.bjjhwx.cn

[Q75] 日期格式化
来源：http://zi.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gu.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tg.huixiangedu.cn

[Q76] 按天统计
来源：http://rn.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://su.hahajie.cn

[Q77] 时间加减
来源：http://za.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qc.panjiajie.cn

[Q78] 当前时间
来源：http://xs.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ky.colortex.cn

[Q79] 字符串拼接
来源：http://mo.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://za.muxihuayi.cn

[Q80] 字符串截取
来源：http://ug.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vu.chemitech.net.cn

[Q81] 字符串替换
来源：http://lm.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yk.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://rl.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mc.nszjky.cn

[Q83] 大小写转换
来源：http://vo.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wa.asd995.cn

[Q84] 去除首尾空格
来源：http://ky.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://se.hnjuh.cn

[Q85] 数值取整
来源：http://fc.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wv.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://sr.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eo.huanxung.cn

[Q87] JSON 字段做条件
来源：http://pr.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vt.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://bc.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pm.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bi.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://az.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ws.chemitech.net.cn

[Q90] 生成序号列
来源：http://dd.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mx.9csxet.cn

================================================================================
来源：http://fa.bookmarksfly.cn

R. Bash 专题
来源：http://ag.yuexingan06.cn

================================================================================
来源：http://cr.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://yw.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://zi.bjjhwx.cn

set -euo pipefail
来源：http://sj.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://dy.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://yx.huixiangedu.cn

[R03] 只读变量
来源：http://ff.haigaiapp.cn

readonly PI=3.14
来源：http://bh.huixiangedu.cn

[R04] 位置参数
来源：http://xn.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ek.bookmarksfly.cn

[R05] 参数默认值
来源：http://xf.szxytkj.cn

name="${1:-default}"
来源：http://pp.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://ov.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hf.yuexingan06.cn

[R07] if 判断文件
来源：http://zg.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vp.nicolike.cn

[R08] 数值比较
来源：http://pd.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ib.yuexingan06.cn

[R09] 字符串比较
来源：http://ab.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qp.bookmarksfly.cn

[R10] 正则匹配
来源：http://jf.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dl.jianghongdianzi.cn

[R11] case 多分支
来源：http://yk.521024.cn

case "$1" in
来源：http://kd.hnjuh.cn

start) echo "启动" ;;
来源：http://ee.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://na.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://zm.yuntaijiaju.cn

esac
来源：http://xw.shxzukj.cn

[R12] for 遍历文件
来源：http://fl.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://zl.jctech888.com.cn

[R13] for 计数循环
来源：http://lu.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ev.521024.cn

[R14] C 风格 for
来源：http://ql.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wb.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://qc.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nw.lnxyls.cn

[R16] until 等待条件
来源：http://fc.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ew.hnjuh.cn

[R17] 数组定义与取值
来源：http://ou.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vc.newstarts.cn

[R18] 遍历数组
来源：http://xl.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://se.9csxet.cn

[R19] 数组长度
来源：http://tg.szxytkj.cn

echo "${#arr[@]}"
来源：http://ky.gzmigu.cn

[R20] 关联数组（字典）
来源：http://kx.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vb.haigaiapp.cn

[R21] 字符串长度
来源：http://xv.shxzskj.cn

echo "${#s}"
来源：http://zl.lnxyls.cn

[R22] 截取子串
来源：http://yi.panjiajie.cn

echo "${s:0:5}"
来源：http://lh.colortex.cn

[R23] 字符串替换
来源：http://bl.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://na.bjjhwx.cn

[R24] 大小写转换
来源：http://bx.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gb.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://ke.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iq.nszjky.cn

[R26] 命令替换
来源：http://at.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://hf.szxytkj.cn

[R27] 算术展开
来源：http://vj.colortex.cn

echo $((1 + 2 * 3))
来源：http://no.huixiangedu.cn

[R28] 浮点运算
来源：http://fl.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://gh.newstarts.cn

[R29] 定义函数
来源：http://sb.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kz.asd995.cn

[R30] 函数返回状态码
来源：http://ji.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://yr.hnjuh.cn

[R31] 局部变量
来源：http://ha.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://ca.szsharing.cn

[R32] 参数个数校验
来源：http://jj.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://km.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://ln.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xw.shxzskj.cn

[R34] 退出时清理
来源：http://rp.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xw.wgjwhj.cn

[R35] 后台执行并等待
来源：http://hq.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cv.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://wm.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gj.hahajie.cn

[R37] 把输出赋给变量
来源：http://fb.huixinmuqiang.cn

files=$(ls -1)
来源：http://mf.haigaiapp.cn

[R38] 管道串联
来源：http://kc.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://jm.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://ls.haigaiapp.cn

cmd > out.log 2>&1
来源：http://gu.huanxung.cn

[R40] 追加写日志
来源：http://ak.wgjwhj.cn

echo "log" >> out.log
来源：http://om.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://fm.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://hq.haigaiapp.cn

[R42] 输入重定向
来源：http://co.hnjuh.cn

wc -l < a.txt
来源：http://cc.9csxet.cn

[R43] 按名字查找文件
来源：http://ik.asd995.cn

find . -name "*.log" -type f
来源：http://qs.hahajie.cn

[R44] 按修改时间查找
来源：http://lp.bjjhwx.cn

find . -mtime -7 -type f
来源：http://mz.yuexingan06.cn

[R45] 批量删除
来源：http://rv.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://ec.hnjuh.cn

[R46] 递归替换文件内容
来源：http://kr.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hk.shtwfgs.cn

[R47] sed 单行替换
来源：http://kf.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ol.nszjky.cn

[R48] awk 取指定列
来源：http://ji.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://be.yuexingan06.cn

[R49] awk 带条件
来源：http://dz.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://co.shtwfgs.cn

[R50] awk 求和
来源：http://qy.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ti.asd995.cn

[R51] 排序去重取前几
来源：http://yr.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gk.haigaiapp.cn

[R52] 统计行数
来源：http://cs.lnxyls.cn

wc -l a.txt
来源：http://uw.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://wn.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kt.hahajie.cn

[R54] 比较两个文件
来源：http://lw.bookmarksfly.cn

diff a.txt b.txt
来源：http://eo.hnjuh.cn

[R55] 压缩与解压
来源：http://wr.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mv.panjiajie.cn

[R56] 远程拷贝
来源：http://zi.shtwfgs.cn

scp file user@host:/path/
来源：http://kk.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://rq.chemitech.net.cn

ssh user@host 'uptime'
来源：http://tt.szxytkj.cn

[R58] 下载文件
来源：http://wj.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tk.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://qd.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jd.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://rq.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eu.jctech888.com.cn

[R61] 磁盘占用
来源：http://qs.panjiajie.cn

df -h;  du -sh *
来源：http://uc.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://fd.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://hy.gzmigu.cn

[R63] 内存与进程
来源：http://oy.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://uf.colortex.cn

[R64] 结束进程
来源：http://ij.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://ws.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://yq.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yo.hahajie.cn

[R66] 定时任务
来源：http://nb.colortex.cn

crontab -e;  crontab -l
来源：http://gj.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://fb.nszjky.cn

openssl rand -hex 16
来源：http://oe.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://qj.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mh.shxzskj.cn

[R69] 生成随机密码
来源：http://qq.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://wp.colortex.cn

[R70] 时间戳与互转
来源：http://vi.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://ka.nicolike.cn

[R71] 日期格式化
来源：http://mp.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rj.szxytkj.cn

[R72] 等待端口就绪
来源：http://ka.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xh.bjjhwx.cn

[R73] 分割大日志
来源：http://pc.shxzskj.cn

split -l 1000 big.log part_
来源：http://uc.haigaiapp.cn

[R74] 批量重命名
来源：http://yu.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ax.gzmigu.cn

[R75] 导出环境变量
来源：http://mc.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://nx.hnjuh.cn

[R76] 使用临时文件
来源：http://gr.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vi.9csxet.cn

[R77] 读取用户输入
来源：http://mn.hnjuh.cn

read -rp "请输入: " ans
来源：http://cd.jctech888.com.cn

[R78] 交互式菜单
来源：http://sj.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yw.muxihuayi.cn

[R79] 解析命令行选项
来源：http://su.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ds.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://mk.hahajie.cn

time ./run.sh
来源：http://ra.asd995.cn

================================================================================
来源：http://lq.muxihuayi.cn

S. C / C++ 专题
来源：http://no.hahajie.cn

================================================================================
来源：http://jv.gzmigu.cn

[S01] C：Hello World
来源：http://ev.nicolike.cn

#include <stdio.h>
来源：http://iq.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iy.521024.cn

[S02] C：变量与格式化输出
来源：http://tr.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://qn.yuntaijiaju.cn

[S03] C：读入整数
来源：http://fx.nszjky.cn

int x; scanf("%d", &x);
来源：http://xm.panjiajie.cn

[S04] C：字符串复制
来源：http://iw.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zw.hnjuh.cn

[S05] C：字符串长度
来源：http://ue.huixiangedu.cn

strlen(s)
来源：http://yv.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://xo.shxzskj.cn

strcmp(a, b) == 0
来源：http://pf.hnjuh.cn

[S07] C：数组遍历求和
来源：http://jn.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jv.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://km.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hx.asd995.cn

[S09] C：结构体定义与初始化
来源：http://aw.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fb.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://db.huanxung.cn

int *p = &a;  *p = 5;
来源：http://mp.chemitech.net.cn

[S11] C：逐行读文件
来源：http://zo.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://pr.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ap.asd995.cn

fclose(f);
来源：http://xu.newstarts.cn

[S12] C：写文件
来源：http://lk.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qd.nicolike.cn

[S13] C：宏定义
来源：http://hs.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gd.shxzukj.cn

[S14] C：枚举
来源：http://lm.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://ez.yuntaijiaju.cn

[S15] C：类型转换
来源：http://ba.bookmarksfly.cn

(double) a / b
来源：http://as.521024.cn

[S16] C：位操作置位
来源：http://fw.muxihuayi.cn

x |= (1 << 3);
来源：http://bc.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://fc.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uq.wgjwhj.cn

[S18] C：命令行参数
来源：http://ep.asd995.cn

int main(int argc, char **argv)
来源：http://ph.chemitech.net.cn

[S19] C：快速排序
来源：http://en.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ff.hahajie.cn

[S20] C：二分查找
来源：http://am.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vn.chemitech.net.cn

[S21] C：字符类别判断
来源：http://qg.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://er.chemitech.net.cn

[S22] C：字符串转数字
来源：http://fy.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nz.shxzskj.cn

[S23] C：随机数
来源：http://ix.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ht.haigaiapp.cn

[S24] C：获取本地时间
来源：http://kb.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ah.jctech888.com.cn

[S25] C：内存拷贝
来源：http://eu.gzmigu.cn

memcpy(dst, src, n);
来源：http://ok.panjiajie.cn

[S26] C：内存清零
来源：http://qc.colortex.cn

memset(a, 0, sizeof a);
来源：http://st.hnjuh.cn

[S27] C：定义常量
来源：http://su.9csxet.cn

const double PI = 3.14159;
来源：http://vq.shxzukj.cn

[S28] C：静态变量
来源：http://rx.muxihuayi.cn

static int counter = 0;
来源：http://ak.szsharing.cn

[S29] C：变参函数
来源：http://oa.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tc.bookmarksfly.cn

[S30] C：头文件保护
来源：http://tv.gzmigu.cn

#ifndef X_H
来源：http://cl.haigaiapp.cn

#define X_H
来源：http://bx.chemitech.net.cn

#endif
来源：http://nm.nicolike.cn

[S31] C++：Hello World
来源：http://yy.bookmarksfly.cn

#include <iostream>
来源：http://ai.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://ga.newstarts.cn

[S32] C++：字符串
来源：http://la.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://lo.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://il.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cm.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://ix.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://ua.szxytkj.cn

[S35] C++：map
来源：http://cw.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ao.szxytkj.cn

[S36] C++：unordered_map
来源：http://jo.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://th.panjiajie.cn

[S37] C++：set
来源：http://mn.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oi.gzmigu.cn

[S38] C++：排序
来源：http://uu.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://gd.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://bk.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bm.muxihuayi.cn

[S40] C++：查找元素
来源：http://qi.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bb.9csxet.cn

[S41] C++：类与构造函数
来源：http://mv.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oy.nszjky.cn

[S42] C++：继承与虚函数
来源：http://pm.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://mx.wgjwhj.cn


<!-- 参考信息 -->