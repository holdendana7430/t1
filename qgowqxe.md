代发 wailian999

[Q78] 当前时间
来源：http://ir.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://go.lnxyls.cn

[Q79] 字符串拼接
来源：http://wt.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cr.nszjky.cn

[Q80] 字符串截取
来源：http://hn.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ai.9csxet.cn

[Q81] 字符串替换
来源：http://bj.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ef.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://ju.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bo.muxihuayi.cn

[Q83] 大小写转换
来源：http://bm.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fr.nszjky.cn

[Q84] 去除首尾空格
来源：http://kr.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://tf.newstarts.cn

[Q85] 数值取整
来源：http://vf.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nb.asd995.cn

[Q86] 读取 JSON 字段
来源：http://zg.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yv.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://hb.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sv.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://gj.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bo.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://el.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://oy.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yy.shxzskj.cn

[Q90] 生成序号列
来源：http://hw.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tv.szsharing.cn

================================================================================
来源：http://yn.bjjhwx.cn

R. Bash 专题
来源：http://xg.jctech888.com.cn

================================================================================
来源：http://kj.shxzskj.cn

[R01] shebang 与严格模式
来源：http://hs.asd995.cn

#!/usr/bin/env bash
来源：http://qq.9csxet.cn

set -euo pipefail
来源：http://ke.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://ew.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://wc.yuntaijiaju.cn

[R03] 只读变量
来源：http://nd.bookmarksfly.cn

readonly PI=3.14
来源：http://yx.bookmarksfly.cn

[R04] 位置参数
来源：http://jh.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sg.gzmigu.cn

[R05] 参数默认值
来源：http://fs.muxihuayi.cn

name="${1:-default}"
来源：http://ae.asd995.cn

[R06] 判断命令是否存在
来源：http://bk.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cd.yuexingan06.cn

[R07] if 判断文件
来源：http://kz.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fx.szsharing.cn

[R08] 数值比较
来源：http://rl.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qi.szxytkj.cn

[R09] 字符串比较
来源：http://ig.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bx.hahajie.cn

[R10] 正则匹配
来源：http://rn.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wq.shtwfgs.cn

[R11] case 多分支
来源：http://hs.lnxyls.cn

case "$1" in
来源：http://hn.yuexingan06.cn

start) echo "启动" ;;
来源：http://pr.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://yu.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://aj.shtwfgs.cn

esac
来源：http://nv.szsharing.cn

[R12] for 遍历文件
来源：http://vp.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://jm.szxytkj.cn

[R13] for 计数循环
来源：http://zg.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://zb.hnjuh.cn

[R14] C 风格 for
来源：http://yr.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mo.szsharing.cn

[R15] while 逐行读文件
来源：http://hx.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hu.wgjwhj.cn

[R16] until 等待条件
来源：http://xv.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tq.shxzskj.cn

[R17] 数组定义与取值
来源：http://kj.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yi.yuexingan06.cn

[R18] 遍历数组
来源：http://wr.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://az.asd995.cn

[R19] 数组长度
来源：http://px.huixiangedu.cn

echo "${#arr[@]}"
来源：http://tc.newstarts.cn

[R20] 关联数组（字典）
来源：http://jf.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bb.asd995.cn

[R21] 字符串长度
来源：http://af.chemitech.net.cn

echo "${#s}"
来源：http://pg.panjiajie.cn

[R22] 截取子串
来源：http://sy.hahajie.cn

echo "${s:0:5}"
来源：http://ir.muxihuayi.cn

[R23] 字符串替换
来源：http://rs.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nt.colortex.cn

[R24] 大小写转换
来源：http://op.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xn.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://aw.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://up.colortex.cn

[R26] 命令替换
来源：http://tq.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://iw.asd995.cn

[R27] 算术展开
来源：http://cz.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://we.huixiangedu.cn

[R28] 浮点运算
来源：http://rl.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://yb.521024.cn

[R29] 定义函数
来源：http://hc.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kt.bjjhwx.cn

[R30] 函数返回状态码
来源：http://au.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://gc.wgjwhj.cn

[R31] 局部变量
来源：http://np.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://ty.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://ut.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ud.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://ng.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sw.9csxet.cn

[R34] 退出时清理
来源：http://du.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yi.521024.cn

[R35] 后台执行并等待
来源：http://xr.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ro.shxzskj.cn

[R36] 并发执行多个任务
来源：http://bv.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mg.panjiajie.cn

[R37] 把输出赋给变量
来源：http://xh.szxytkj.cn

files=$(ls -1)
来源：http://zu.nszjky.cn

[R38] 管道串联
来源：http://gl.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://oa.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://jc.hnjuh.cn

cmd > out.log 2>&1
来源：http://ao.newstarts.cn

[R40] 追加写日志
来源：http://dv.huixinmuqiang.cn

echo "log" >> out.log
来源：http://bp.jctech888.com.cn

[R41] 丢弃输出
来源：http://dz.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://lz.nszjky.cn

[R42] 输入重定向
来源：http://fw.bjjhwx.cn

wc -l < a.txt
来源：http://xj.szsharing.cn

[R43] 按名字查找文件
来源：http://zg.asd995.cn

find . -name "*.log" -type f
来源：http://bu.newstarts.cn

[R44] 按修改时间查找
来源：http://bg.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://sn.nszjky.cn

[R45] 批量删除
来源：http://qm.asd995.cn

find . -name "*.tmp" -delete
来源：http://oo.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://ol.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vk.hnjuh.cn

[R47] sed 单行替换
来源：http://rz.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ac.muxihuayi.cn

[R48] awk 取指定列
来源：http://lc.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://tt.yuntaijiaju.cn

[R49] awk 带条件
来源：http://bk.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qj.jctech888.com.cn

[R50] awk 求和
来源：http://mz.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xh.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://yh.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ov.panjiajie.cn

[R52] 统计行数
来源：http://ks.lnxyls.cn

wc -l a.txt
来源：http://nw.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://gj.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ix.wgjwhj.cn

[R54] 比较两个文件
来源：http://on.nicolike.cn

diff a.txt b.txt
来源：http://mt.gzmigu.cn

[R55] 压缩与解压
来源：http://xv.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kr.nszjky.cn

[R56] 远程拷贝
来源：http://gr.muxihuayi.cn

scp file user@host:/path/
来源：http://rw.szxytkj.cn

[R57] 远程执行命令
来源：http://zp.9csxet.cn

ssh user@host 'uptime'
来源：http://gb.bookmarksfly.cn

[R58] 下载文件
来源：http://yu.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eo.bjjhwx.cn

[R59] 发 POST JSON
来源：http://vn.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qq.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://ng.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vu.colortex.cn

[R61] 磁盘占用
来源：http://yg.jctech888.com.cn

df -h;  du -sh *
来源：http://qe.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://vl.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ch.chemitech.net.cn

[R63] 内存与进程
来源：http://bi.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://sz.jctech888.com.cn

[R64] 结束进程
来源：http://mh.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://mz.shxzskj.cn

[R65] 查看端口占用
来源：http://oj.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ss.521024.cn

[R66] 定时任务
来源：http://xj.muxihuayi.cn

crontab -e;  crontab -l
来源：http://kt.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://yr.jianghongdianzi.cn

openssl rand -hex 16
来源：http://jh.szsharing.cn

[R68] 计算文件校验值
来源：http://hr.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wk.lnxyls.cn

[R69] 生成随机密码
来源：http://dx.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://rh.muxihuayi.cn

[R70] 时间戳与互转
来源：http://oz.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://mj.szxytkj.cn

[R71] 日期格式化
来源：http://gk.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uh.shtwfgs.cn

[R72] 等待端口就绪
来源：http://fo.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bp.nszjky.cn

[R73] 分割大日志
来源：http://qp.shxzskj.cn

split -l 1000 big.log part_
来源：http://mf.shxzukj.cn

[R74] 批量重命名
来源：http://sf.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rv.haigaiapp.cn

[R75] 导出环境变量
来源：http://in.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://wu.szsharing.cn

[R76] 使用临时文件
来源：http://xg.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vb.newstarts.cn

[R77] 读取用户输入
来源：http://sc.hnjuh.cn

read -rp "请输入: " ans
来源：http://fq.chemitech.net.cn

[R78] 交互式菜单
来源：http://fa.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mt.yuexingan06.cn

[R79] 解析命令行选项
来源：http://yc.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zx.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://uc.bookmarksfly.cn

time ./run.sh
来源：http://as.521024.cn

================================================================================
来源：http://rs.colortex.cn

S. C / C++ 专题
来源：http://fp.chemitech.net.cn

================================================================================
来源：http://wc.521024.cn

[S01] C：Hello World
来源：http://un.hahajie.cn

#include <stdio.h>
来源：http://dp.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gb.huanxung.cn

[S02] C：变量与格式化输出
来源：http://sz.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://ui.nicolike.cn

[S03] C：读入整数
来源：http://jh.asd995.cn

int x; scanf("%d", &x);
来源：http://kc.huanxung.cn

[S04] C：字符串复制
来源：http://gw.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eh.wgjwhj.cn

[S05] C：字符串长度
来源：http://eu.huanxung.cn

strlen(s)
来源：http://lo.colortex.cn

[S06] C：字符串比较
来源：http://xo.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://bp.szxytkj.cn

[S07] C：数组遍历求和
来源：http://cd.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rc.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://vi.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zo.521024.cn

[S09] C：结构体定义与初始化
来源：http://wx.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fs.shxzskj.cn

[S10] C：指针与解引用
来源：http://uu.szsharing.cn

int *p = &a;  *p = 5;
来源：http://rg.hahajie.cn

[S11] C：逐行读文件
来源：http://pd.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://sf.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ni.huixinmuqiang.cn

fclose(f);
来源：http://sl.colortex.cn

[S12] C：写文件
来源：http://wi.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rd.9csxet.cn

[S13] C：宏定义
来源：http://zy.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ud.szxytkj.cn

[S14] C：枚举
来源：http://ee.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://zh.bjjhwx.cn

[S15] C：类型转换
来源：http://zd.huixinmuqiang.cn

(double) a / b
来源：http://ve.lnxyls.cn

[S16] C：位操作置位
来源：http://mj.lnxyls.cn

x |= (1 << 3);
来源：http://zh.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://ex.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ys.nszjky.cn

[S18] C：命令行参数
来源：http://nn.asd995.cn

int main(int argc, char **argv)
来源：http://xc.9csxet.cn

[S19] C：快速排序
来源：http://yj.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://py.szxytkj.cn

[S20] C：二分查找
来源：http://ze.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oi.chemitech.net.cn

[S21] C：字符类别判断
来源：http://xf.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vc.lnxyls.cn

[S22] C：字符串转数字
来源：http://oi.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mi.wgjwhj.cn

[S23] C：随机数
来源：http://tr.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qw.gzmigu.cn

[S24] C：获取本地时间
来源：http://tk.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yo.shxzskj.cn

[S25] C：内存拷贝
来源：http://hf.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://gi.colortex.cn

[S26] C：内存清零
来源：http://pi.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://ds.hahajie.cn

[S27] C：定义常量
来源：http://yk.szsharing.cn

const double PI = 3.14159;
来源：http://zr.szsharing.cn

[S28] C：静态变量
来源：http://vk.yuexingan06.cn

static int counter = 0;
来源：http://pn.nicolike.cn

[S29] C：变参函数
来源：http://vg.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ht.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://yv.yuexingan06.cn

#ifndef X_H
来源：http://dc.jianghongdianzi.cn

#define X_H
来源：http://np.huixinmuqiang.cn

#endif
来源：http://fo.asd995.cn

[S31] C++：Hello World
来源：http://yc.9csxet.cn

#include <iostream>
来源：http://it.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ie.shxzskj.cn

[S32] C++：字符串
来源：http://zh.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://dw.muxihuayi.cn

[S33] C++：vector 增删
来源：http://xt.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://po.shxzskj.cn

[S34] C++：遍历 vector
来源：http://ib.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://en.colortex.cn

[S35] C++：map
来源：http://ht.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gy.newstarts.cn

[S36] C++：unordered_map
来源：http://ec.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nr.shxzskj.cn

[S37] C++：set
来源：http://by.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qr.szsharing.cn

[S38] C++：排序
来源：http://tr.521024.cn

std::sort(v.begin(), v.end());
来源：http://jv.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://wv.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zx.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://im.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lx.hnjuh.cn

[S41] C++：类与构造函数
来源：http://bo.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bh.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://mz.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://ri.shxzukj.cn

[S43] C++：智能指针
来源：http://lh.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://sb.chemitech.net.cn

[S44] C++：引用传参
来源：http://ir.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://gq.jctech888.com.cn

[S45] C++：lambda
来源：http://ou.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ue.panjiajie.cn

[S46] C++：函数模板
来源：http://eg.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ni.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://bs.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rq.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://ol.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lo.shxzukj.cn


<!-- 参考信息 -->