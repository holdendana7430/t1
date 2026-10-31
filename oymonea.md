代发 wailian999

[Q78] 当前时间
来源：http://xl.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ca.wgjwhj.cn

[Q79] 字符串拼接
来源：http://jy.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qo.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://jk.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kw.colortex.cn

[Q81] 字符串替换
来源：http://tz.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nl.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://fw.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zu.colortex.cn

[Q83] 大小写转换
来源：http://or.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gj.panjiajie.cn

[Q84] 去除首尾空格
来源：http://qg.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://ok.wgjwhj.cn

[Q85] 数值取整
来源：http://vi.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kt.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://yc.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yg.9csxet.cn

[Q87] JSON 字段做条件
来源：http://ng.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rm.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://sy.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iz.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kh.gzmigu.cn

[Q89] 判断表是否存在
来源：http://ha.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wx.521024.cn

[Q90] 生成序号列
来源：http://dk.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zh.haigaiapp.cn

================================================================================
来源：http://oy.colortex.cn

R. Bash 专题
来源：http://zc.shxzskj.cn

================================================================================
来源：http://md.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://hw.haigaiapp.cn

#!/usr/bin/env bash
来源：http://yo.newstarts.cn

set -euo pipefail
来源：http://zc.panjiajie.cn

[R02] 变量赋值与使用
来源：http://df.nicolike.cn

name="Tom"; echo "$name"
来源：http://cb.huanxung.cn

[R03] 只读变量
来源：http://jp.jctech888.com.cn

readonly PI=3.14
来源：http://fg.haigaiapp.cn

[R04] 位置参数
来源：http://fk.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://en.asd995.cn

[R05] 参数默认值
来源：http://rb.lnxyls.cn

name="${1:-default}"
来源：http://mz.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://wa.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qo.szxytkj.cn

[R07] if 判断文件
来源：http://ah.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cm.szsharing.cn

[R08] 数值比较
来源：http://ru.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xh.nicolike.cn

[R09] 字符串比较
来源：http://wb.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yv.wgjwhj.cn

[R10] 正则匹配
来源：http://nt.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fh.hahajie.cn

[R11] case 多分支
来源：http://qk.nszjky.cn

case "$1" in
来源：http://ee.lnxyls.cn

start) echo "启动" ;;
来源：http://yy.huanxung.cn

stop)  echo "停止" ;;
来源：http://kb.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://te.nszjky.cn

esac
来源：http://hc.szxytkj.cn

[R12] for 遍历文件
来源：http://yl.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://nv.9csxet.cn

[R13] for 计数循环
来源：http://gh.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://au.szxytkj.cn

[R14] C 风格 for
来源：http://gx.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wi.shxzskj.cn

[R15] while 逐行读文件
来源：http://yw.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://em.panjiajie.cn

[R16] until 等待条件
来源：http://tq.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bc.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://os.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mr.jctech888.com.cn

[R18] 遍历数组
来源：http://jm.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ag.9csxet.cn

[R19] 数组长度
来源：http://cu.nicolike.cn

echo "${#arr[@]}"
来源：http://tw.gzmigu.cn

[R20] 关联数组（字典）
来源：http://fl.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mn.panjiajie.cn

[R21] 字符串长度
来源：http://ie.jianghongdianzi.cn

echo "${#s}"
来源：http://rn.huixiangedu.cn

[R22] 截取子串
来源：http://qp.shtwfgs.cn

echo "${s:0:5}"
来源：http://wj.asd995.cn

[R23] 字符串替换
来源：http://bm.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://un.521024.cn

[R24] 大小写转换
来源：http://ck.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ai.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://zu.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://or.panjiajie.cn

[R26] 命令替换
来源：http://pq.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://ke.szsharing.cn

[R27] 算术展开
来源：http://gf.9csxet.cn

echo $((1 + 2 * 3))
来源：http://vr.shxzskj.cn

[R28] 浮点运算
来源：http://fq.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://vd.szsharing.cn

[R29] 定义函数
来源：http://lx.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eg.colortex.cn

[R30] 函数返回状态码
来源：http://lu.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://so.huixinmuqiang.cn

[R31] 局部变量
来源：http://fj.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://cf.jctech888.com.cn

[R32] 参数个数校验
来源：http://ql.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ts.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://jd.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dd.jianghongdianzi.cn

[R34] 退出时清理
来源：http://ev.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dm.huanxung.cn

[R35] 后台执行并等待
来源：http://hp.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bk.9csxet.cn

[R36] 并发执行多个任务
来源：http://yy.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vj.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://pr.jctech888.com.cn

files=$(ls -1)
来源：http://rk.szxytkj.cn

[R38] 管道串联
来源：http://to.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://eo.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://dp.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://fy.huixiangedu.cn

[R40] 追加写日志
来源：http://ry.nszjky.cn

echo "log" >> out.log
来源：http://ss.newstarts.cn

[R41] 丢弃输出
来源：http://ix.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://oc.huixiangedu.cn

[R42] 输入重定向
来源：http://nq.colortex.cn

wc -l < a.txt
来源：http://no.shxzskj.cn

[R43] 按名字查找文件
来源：http://je.huanxung.cn

find . -name "*.log" -type f
来源：http://er.panjiajie.cn

[R44] 按修改时间查找
来源：http://vb.9csxet.cn

find . -mtime -7 -type f
来源：http://tt.jianghongdianzi.cn

[R45] 批量删除
来源：http://ae.hahajie.cn

find . -name "*.tmp" -delete
来源：http://oq.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://hc.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yt.chemitech.net.cn

[R47] sed 单行替换
来源：http://lm.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mo.szxytkj.cn

[R48] awk 取指定列
来源：http://zy.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://ve.szsharing.cn

[R49] awk 带条件
来源：http://zr.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ip.newstarts.cn

[R50] awk 求和
来源：http://fu.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eq.haigaiapp.cn

[R51] 排序去重取前几
来源：http://oy.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wd.shxzskj.cn

[R52] 统计行数
来源：http://ye.nicolike.cn

wc -l a.txt
来源：http://nx.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://jd.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pc.nszjky.cn

[R54] 比较两个文件
来源：http://ai.muxihuayi.cn

diff a.txt b.txt
来源：http://op.chemitech.net.cn

[R55] 压缩与解压
来源：http://lr.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xb.szsharing.cn

[R56] 远程拷贝
来源：http://pm.huixinmuqiang.cn

scp file user@host:/path/
来源：http://sf.asd995.cn

[R57] 远程执行命令
来源：http://ru.9csxet.cn

ssh user@host 'uptime'
来源：http://rz.jianghongdianzi.cn

[R58] 下载文件
来源：http://xx.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://be.shxzukj.cn

[R59] 发 POST JSON
来源：http://hl.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://av.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://sj.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cl.panjiajie.cn

[R61] 磁盘占用
来源：http://ic.huixiangedu.cn

df -h;  du -sh *
来源：http://cy.nicolike.cn

[R62] 找最占空间的文件
来源：http://rf.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://yv.gzmigu.cn

[R63] 内存与进程
来源：http://cy.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://hb.gzmigu.cn

[R64] 结束进程
来源：http://wk.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://ro.haigaiapp.cn

[R65] 查看端口占用
来源：http://qo.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://up.9csxet.cn

[R66] 定时任务
来源：http://iw.szxytkj.cn

crontab -e;  crontab -l
来源：http://un.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://zz.yuntaijiaju.cn

openssl rand -hex 16
来源：http://cu.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://pw.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hd.huanxung.cn

[R69] 生成随机密码
来源：http://jj.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://dl.muxihuayi.cn

[R70] 时间戳与互转
来源：http://hj.asd995.cn

date +%s;  date -d @1700000000
来源：http://uw.huixiangedu.cn

[R71] 日期格式化
来源：http://ip.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wd.hahajie.cn

[R72] 等待端口就绪
来源：http://tv.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ak.9csxet.cn

[R73] 分割大日志
来源：http://ln.hahajie.cn

split -l 1000 big.log part_
来源：http://ip.haigaiapp.cn

[R74] 批量重命名
来源：http://ye.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uo.bookmarksfly.cn

[R75] 导出环境变量
来源：http://lt.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://mg.521024.cn

[R76] 使用临时文件
来源：http://fc.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jc.huixiangedu.cn

[R77] 读取用户输入
来源：http://fm.huanxung.cn

read -rp "请输入: " ans
来源：http://qe.shxzskj.cn

[R78] 交互式菜单
来源：http://wi.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yl.bjjhwx.cn

[R79] 解析命令行选项
来源：http://jh.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fz.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://qp.lnxyls.cn

time ./run.sh
来源：http://rk.colortex.cn

================================================================================
来源：http://pv.szxytkj.cn

S. C / C++ 专题
来源：http://vu.lnxyls.cn

================================================================================
来源：http://od.panjiajie.cn

[S01] C：Hello World
来源：http://ty.yuntaijiaju.cn

#include <stdio.h>
来源：http://bj.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jq.szsharing.cn

[S02] C：变量与格式化输出
来源：http://ba.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://sf.szxytkj.cn

[S03] C：读入整数
来源：http://xa.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://zb.wgjwhj.cn

[S04] C：字符串复制
来源：http://rp.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gg.hnjuh.cn

[S05] C：字符串长度
来源：http://zc.newstarts.cn

strlen(s)
来源：http://vf.shtwfgs.cn

[S06] C：字符串比较
来源：http://hm.huanxung.cn

strcmp(a, b) == 0
来源：http://qq.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://er.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://na.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://am.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cj.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://eo.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vf.9csxet.cn

[S10] C：指针与解引用
来源：http://kb.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://ot.hnjuh.cn

[S11] C：逐行读文件
来源：http://jh.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://pu.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fd.colortex.cn

fclose(f);
来源：http://md.muxihuayi.cn

[S12] C：写文件
来源：http://an.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wn.asd995.cn

[S13] C：宏定义
来源：http://ei.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zn.muxihuayi.cn

[S14] C：枚举
来源：http://xp.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://jc.szsharing.cn

[S15] C：类型转换
来源：http://fh.nszjky.cn

(double) a / b
来源：http://rk.szxytkj.cn

[S16] C：位操作置位
来源：http://pf.shxzukj.cn

x |= (1 << 3);
来源：http://mv.nszjky.cn

[S17] C：安全拼接字符串
来源：http://hr.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gb.asd995.cn

[S18] C：命令行参数
来源：http://mt.colortex.cn

int main(int argc, char **argv)
来源：http://lw.lnxyls.cn

[S19] C：快速排序
来源：http://co.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ti.hahajie.cn

[S20] C：二分查找
来源：http://iu.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wy.521024.cn

[S21] C：字符类别判断
来源：http://mm.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fx.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://fp.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wi.521024.cn

[S23] C：随机数
来源：http://tm.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ty.shxzukj.cn

[S24] C：获取本地时间
来源：http://gn.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nn.panjiajie.cn

[S25] C：内存拷贝
来源：http://iu.shtwfgs.cn

memcpy(dst, src, n);
来源：http://sh.huixiangedu.cn

[S26] C：内存清零
来源：http://ii.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://is.wgjwhj.cn

[S27] C：定义常量
来源：http://rn.muxihuayi.cn

const double PI = 3.14159;
来源：http://bh.newstarts.cn

[S28] C：静态变量
来源：http://ay.haigaiapp.cn

static int counter = 0;
来源：http://dn.lnxyls.cn

[S29] C：变参函数
来源：http://sw.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://su.nszjky.cn

[S30] C：头文件保护
来源：http://bq.nszjky.cn

#ifndef X_H
来源：http://ng.szxytkj.cn

#define X_H
来源：http://km.shxzukj.cn

#endif
来源：http://ux.nicolike.cn

[S31] C++：Hello World
来源：http://da.jctech888.com.cn

#include <iostream>
来源：http://jg.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://gm.wgjwhj.cn

[S32] C++：字符串
来源：http://et.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://nj.wgjwhj.cn

[S33] C++：vector 增删
来源：http://qt.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yw.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://oc.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://dw.panjiajie.cn

[S35] C++：map
来源：http://ou.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ho.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://ui.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ca.szsharing.cn

[S37] C++：set
来源：http://et.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cd.jianghongdianzi.cn

[S38] C++：排序
来源：http://hu.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://dd.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://bl.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mj.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://ll.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iq.shxzskj.cn

[S41] C++：类与构造函数
来源：http://ha.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pg.asd995.cn

[S42] C++：继承与虚函数
来源：http://kh.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://mi.521024.cn

[S43] C++：智能指针
来源：http://xn.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://jf.nszjky.cn

[S44] C++：引用传参
来源：http://hu.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://tl.521024.cn

[S45] C++：lambda
来源：http://dr.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eq.newstarts.cn

[S46] C++：函数模板
来源：http://cu.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lm.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://qe.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mc.9csxet.cn

[S48] C++：逐行读文件
来源：http://sy.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ee.9csxet.cn


<!-- 参考信息 -->