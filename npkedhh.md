代发 wailian999

[Q82] 字符长度与字节长度
来源：http://vv.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lq.huanxung.cn

[Q83] 大小写转换
来源：http://fr.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jw.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://bj.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://qh.nicolike.cn

[Q85] 数值取整
来源：http://bo.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bh.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://io.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ck.szsharing.cn

[Q87] JSON 字段做条件
来源：http://ui.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kg.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://cu.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wy.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qc.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://jd.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gb.panjiajie.cn

[Q90] 生成序号列
来源：http://ox.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eb.bookmarksfly.cn

================================================================================
来源：http://md.muxihuayi.cn

R. Bash 专题
来源：http://xv.bjjhwx.cn

================================================================================
来源：http://sz.newstarts.cn

[R01] shebang 与严格模式
来源：http://mc.yuexingan06.cn

#!/usr/bin/env bash
来源：http://sg.shxzskj.cn

set -euo pipefail
来源：http://eg.hnjuh.cn

[R02] 变量赋值与使用
来源：http://nv.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://yu.hnjuh.cn

[R03] 只读变量
来源：http://is.szxytkj.cn

readonly PI=3.14
来源：http://kw.yuexingan06.cn

[R04] 位置参数
来源：http://rd.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wf.szxytkj.cn

[R05] 参数默认值
来源：http://tp.shtwfgs.cn

name="${1:-default}"
来源：http://fg.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://zx.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ab.huanxung.cn

[R07] if 判断文件
来源：http://ld.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dt.bookmarksfly.cn

[R08] 数值比较
来源：http://ig.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xa.szsharing.cn

[R09] 字符串比较
来源：http://qe.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cy.huanxung.cn

[R10] 正则匹配
来源：http://by.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kw.gzmigu.cn

[R11] case 多分支
来源：http://kr.bookmarksfly.cn

case "$1" in
来源：http://hb.shxzukj.cn

start) echo "启动" ;;
来源：http://ss.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://jb.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://mu.nicolike.cn

esac
来源：http://jf.nszjky.cn

[R12] for 遍历文件
来源：http://iz.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://ds.shtwfgs.cn

[R13] for 计数循环
来源：http://ly.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://gp.bookmarksfly.cn

[R14] C 风格 for
来源：http://ja.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ob.colortex.cn

[R15] while 逐行读文件
来源：http://ba.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uj.nicolike.cn

[R16] until 等待条件
来源：http://fo.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nk.jctech888.com.cn

[R17] 数组定义与取值
来源：http://fo.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ai.bjjhwx.cn

[R18] 遍历数组
来源：http://ek.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sk.yuexingan06.cn

[R19] 数组长度
来源：http://iq.9csxet.cn

echo "${#arr[@]}"
来源：http://wz.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://zs.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jq.chemitech.net.cn

[R21] 字符串长度
来源：http://cr.szsharing.cn

echo "${#s}"
来源：http://uz.asd995.cn

[R22] 截取子串
来源：http://yg.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://da.szsharing.cn

[R23] 字符串替换
来源：http://jh.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jp.asd995.cn

[R24] 大小写转换
来源：http://bq.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vz.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://qx.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qu.muxihuayi.cn

[R26] 命令替换
来源：http://cy.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://jd.haigaiapp.cn

[R27] 算术展开
来源：http://hy.huanxung.cn

echo $((1 + 2 * 3))
来源：http://nf.asd995.cn

[R28] 浮点运算
来源：http://bb.521024.cn

echo "scale=2; 10/3" | bc
来源：http://xe.asd995.cn

[R29] 定义函数
来源：http://cf.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ve.gzmigu.cn

[R30] 函数返回状态码
来源：http://yx.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://vc.muxihuayi.cn

[R31] 局部变量
来源：http://fs.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://sh.hahajie.cn

[R32] 参数个数校验
来源：http://ap.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uo.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://es.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tt.shtwfgs.cn

[R34] 退出时清理
来源：http://qw.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mo.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://uj.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kn.hahajie.cn

[R36] 并发执行多个任务
来源：http://ux.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://su.9csxet.cn

[R37] 把输出赋给变量
来源：http://ut.wgjwhj.cn

files=$(ls -1)
来源：http://md.9csxet.cn

[R38] 管道串联
来源：http://qf.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://mh.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://ow.muxihuayi.cn

cmd > out.log 2>&1
来源：http://fm.haigaiapp.cn

[R40] 追加写日志
来源：http://aa.jianghongdianzi.cn

echo "log" >> out.log
来源：http://cs.hahajie.cn

[R41] 丢弃输出
来源：http://qk.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://gz.yuexingan06.cn

[R42] 输入重定向
来源：http://op.muxihuayi.cn

wc -l < a.txt
来源：http://ha.newstarts.cn

[R43] 按名字查找文件
来源：http://gb.colortex.cn

find . -name "*.log" -type f
来源：http://qr.shtwfgs.cn

[R44] 按修改时间查找
来源：http://tb.shxzskj.cn

find . -mtime -7 -type f
来源：http://vl.huixiangedu.cn

[R45] 批量删除
来源：http://rd.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://yt.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://qg.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gx.9csxet.cn

[R47] sed 单行替换
来源：http://vd.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hi.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://qz.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://dz.asd995.cn

[R49] awk 带条件
来源：http://ny.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cy.asd995.cn

[R50] awk 求和
来源：http://rh.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fc.shxzskj.cn

[R51] 排序去重取前几
来源：http://wu.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ec.jianghongdianzi.cn

[R52] 统计行数
来源：http://ho.jctech888.com.cn

wc -l a.txt
来源：http://jw.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://jw.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yv.gzmigu.cn

[R54] 比较两个文件
来源：http://it.bjjhwx.cn

diff a.txt b.txt
来源：http://at.muxihuayi.cn

[R55] 压缩与解压
来源：http://dg.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bj.521024.cn

[R56] 远程拷贝
来源：http://sy.hahajie.cn

scp file user@host:/path/
来源：http://qv.nszjky.cn

[R57] 远程执行命令
来源：http://wx.9csxet.cn

ssh user@host 'uptime'
来源：http://nc.yuexingan06.cn

[R58] 下载文件
来源：http://oq.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xo.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://aj.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mv.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://ky.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bi.nszjky.cn

[R61] 磁盘占用
来源：http://db.bjjhwx.cn

df -h;  du -sh *
来源：http://jc.nicolike.cn

[R62] 找最占空间的文件
来源：http://fq.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://yp.shxzskj.cn

[R63] 内存与进程
来源：http://iz.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://oc.bookmarksfly.cn

[R64] 结束进程
来源：http://gv.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://ej.colortex.cn

[R65] 查看端口占用
来源：http://iy.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ly.chemitech.net.cn

[R66] 定时任务
来源：http://wj.hahajie.cn

crontab -e;  crontab -l
来源：http://oo.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://wx.panjiajie.cn

openssl rand -hex 16
来源：http://ak.chemitech.net.cn

[R68] 计算文件校验值
来源：http://zs.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fc.shtwfgs.cn

[R69] 生成随机密码
来源：http://or.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://dc.newstarts.cn

[R70] 时间戳与互转
来源：http://no.521024.cn

date +%s;  date -d @1700000000
来源：http://dh.jctech888.com.cn

[R71] 日期格式化
来源：http://ma.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://er.hahajie.cn

[R72] 等待端口就绪
来源：http://et.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dr.asd995.cn

[R73] 分割大日志
来源：http://io.haigaiapp.cn

split -l 1000 big.log part_
来源：http://fw.yuntaijiaju.cn

[R74] 批量重命名
来源：http://bo.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bz.hahajie.cn

[R75] 导出环境变量
来源：http://sf.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://tm.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://tt.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mf.asd995.cn

[R77] 读取用户输入
来源：http://na.bjjhwx.cn

read -rp "请输入: " ans
来源：http://ql.shxzukj.cn

[R78] 交互式菜单
来源：http://fo.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fz.shxzukj.cn

[R79] 解析命令行选项
来源：http://kn.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://or.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://ub.haigaiapp.cn

time ./run.sh
来源：http://br.panjiajie.cn

================================================================================
来源：http://gz.hnjuh.cn

S. C / C++ 专题
来源：http://zx.yuexingan06.cn

================================================================================
来源：http://cp.szxytkj.cn

[S01] C：Hello World
来源：http://gk.nszjky.cn

#include <stdio.h>
来源：http://yg.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://br.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://wk.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://jq.yuntaijiaju.cn

[S03] C：读入整数
来源：http://tr.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://mx.chemitech.net.cn

[S04] C：字符串复制
来源：http://wr.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dh.lnxyls.cn

[S05] C：字符串长度
来源：http://fp.huixinmuqiang.cn

strlen(s)
来源：http://hn.bjjhwx.cn

[S06] C：字符串比较
来源：http://nz.gzmigu.cn

strcmp(a, b) == 0
来源：http://uz.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://dx.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rh.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://lx.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bo.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://mg.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qm.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://ws.szsharing.cn

int *p = &a;  *p = 5;
来源：http://cm.wgjwhj.cn

[S11] C：逐行读文件
来源：http://wm.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://ll.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zq.wgjwhj.cn

fclose(f);
来源：http://yn.shtwfgs.cn

[S12] C：写文件
来源：http://su.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wi.bjjhwx.cn

[S13] C：宏定义
来源：http://lr.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://km.shxzskj.cn

[S14] C：枚举
来源：http://dm.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://pl.huixiangedu.cn

[S15] C：类型转换
来源：http://pc.huixiangedu.cn

(double) a / b
来源：http://aa.huanxung.cn

[S16] C：位操作置位
来源：http://ek.muxihuayi.cn

x |= (1 << 3);
来源：http://el.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://be.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tf.shxzukj.cn

[S18] C：命令行参数
来源：http://kf.shxzskj.cn

int main(int argc, char **argv)
来源：http://ig.lnxyls.cn

[S19] C：快速排序
来源：http://vo.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://on.huanxung.cn

[S20] C：二分查找
来源：http://gm.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ty.bjjhwx.cn

[S21] C：字符类别判断
来源：http://bh.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ou.szxytkj.cn

[S22] C：字符串转数字
来源：http://um.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tu.haigaiapp.cn

[S23] C：随机数
来源：http://xw.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iw.shxzukj.cn

[S24] C：获取本地时间
来源：http://oo.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hf.shxzukj.cn

[S25] C：内存拷贝
来源：http://ti.nszjky.cn

memcpy(dst, src, n);
来源：http://ph.shxzskj.cn

[S26] C：内存清零
来源：http://ep.nicolike.cn

memset(a, 0, sizeof a);
来源：http://xi.bookmarksfly.cn

[S27] C：定义常量
来源：http://gu.chemitech.net.cn

const double PI = 3.14159;
来源：http://pw.lnxyls.cn

[S28] C：静态变量
来源：http://vo.szxytkj.cn

static int counter = 0;
来源：http://db.shtwfgs.cn

[S29] C：变参函数
来源：http://dg.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lc.gzmigu.cn

[S30] C：头文件保护
来源：http://mf.jianghongdianzi.cn

#ifndef X_H
来源：http://dq.9csxet.cn

#define X_H
来源：http://vu.szxytkj.cn

#endif
来源：http://yz.asd995.cn

[S31] C++：Hello World
来源：http://cj.gzmigu.cn

#include <iostream>
来源：http://gd.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://hl.panjiajie.cn

[S32] C++：字符串
来源：http://mg.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://vl.chemitech.net.cn

[S33] C++：vector 增删
来源：http://an.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yv.shxzskj.cn

[S34] C++：遍历 vector
来源：http://bp.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wi.bjjhwx.cn

[S35] C++：map
来源：http://yb.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aw.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://li.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pz.asd995.cn

[S37] C++：set
来源：http://ft.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ot.yuntaijiaju.cn

[S38] C++：排序
来源：http://vh.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://kc.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://kj.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://it.muxihuayi.cn

[S40] C++：查找元素
来源：http://sk.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ps.gzmigu.cn

[S41] C++：类与构造函数
来源：http://zd.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rp.newstarts.cn

[S42] C++：继承与虚函数
来源：http://ap.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://wf.szxytkj.cn

[S43] C++：智能指针
来源：http://wn.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://an.shxzukj.cn

[S44] C++：引用传参
来源：http://nj.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://lq.hnjuh.cn

[S45] C++：lambda
来源：http://ry.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eq.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://mn.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vw.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://bp.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rb.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://lw.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yh.hahajie.cn

while (std::getline(in, line)) { }
来源：http://vv.colortex.cn

[S49] C++：写文件
来源：http://xg.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yj.nicolike.cn

[S50] C++：格式化数字
来源：http://ps.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wf.panjiajie.cn

[S51] C++：显式类型转换
来源：http://sl.bjjhwx.cn

static_cast<double>(a) / b
来源：http://da.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://cf.nicolike.cn


<!-- 参考信息 -->