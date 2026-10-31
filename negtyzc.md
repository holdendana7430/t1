代发 wailian999

[Q80] 字符串截取
来源：http://ky.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ys.nszjky.cn

[Q81] 字符串替换
来源：http://vo.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rs.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://pb.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://el.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://bp.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ld.gzmigu.cn

[Q84] 去除首尾空格
来源：http://uu.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://oa.huixiangedu.cn

[Q85] 数值取整
来源：http://zq.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lx.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://tr.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gq.szsharing.cn

[Q87] JSON 字段做条件
来源：http://ec.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sz.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://tf.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nv.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fn.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://th.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ji.wgjwhj.cn

[Q90] 生成序号列
来源：http://lh.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nc.hahajie.cn

================================================================================
来源：http://th.yuexingan06.cn

R. Bash 专题
来源：http://fx.chemitech.net.cn

================================================================================
来源：http://rw.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://gz.bjjhwx.cn

#!/usr/bin/env bash
来源：http://tb.shtwfgs.cn

set -euo pipefail
来源：http://vp.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://zb.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://do.shtwfgs.cn

[R03] 只读变量
来源：http://io.wgjwhj.cn

readonly PI=3.14
来源：http://bk.wgjwhj.cn

[R04] 位置参数
来源：http://yx.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qy.jctech888.com.cn

[R05] 参数默认值
来源：http://eu.bookmarksfly.cn

name="${1:-default}"
来源：http://qp.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://sh.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://un.bookmarksfly.cn

[R07] if 判断文件
来源：http://ea.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lp.521024.cn

[R08] 数值比较
来源：http://ob.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fs.haigaiapp.cn

[R09] 字符串比较
来源：http://ty.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wt.huixiangedu.cn

[R10] 正则匹配
来源：http://no.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ls.huixiangedu.cn

[R11] case 多分支
来源：http://ej.asd995.cn

case "$1" in
来源：http://jv.hahajie.cn

start) echo "启动" ;;
来源：http://fl.shxzukj.cn

stop)  echo "停止" ;;
来源：http://oy.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://gm.newstarts.cn

esac
来源：http://kl.jctech888.com.cn

[R12] for 遍历文件
来源：http://le.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://cq.yuntaijiaju.cn

[R13] for 计数循环
来源：http://tz.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://zi.panjiajie.cn

[R14] C 风格 for
来源：http://gw.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mb.shxzukj.cn

[R15] while 逐行读文件
来源：http://oz.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fo.hahajie.cn

[R16] until 等待条件
来源：http://of.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dr.jctech888.com.cn

[R17] 数组定义与取值
来源：http://ga.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gw.hnjuh.cn

[R18] 遍历数组
来源：http://bb.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ix.szxytkj.cn

[R19] 数组长度
来源：http://gv.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://hm.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://wr.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cv.huanxung.cn

[R21] 字符串长度
来源：http://wq.nszjky.cn

echo "${#s}"
来源：http://ho.huixiangedu.cn

[R22] 截取子串
来源：http://dg.chemitech.net.cn

echo "${s:0:5}"
来源：http://nn.shxzukj.cn

[R23] 字符串替换
来源：http://cw.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aa.huixinmuqiang.cn

[R24] 大小写转换
来源：http://xw.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dl.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://mf.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dh.szsharing.cn

[R26] 命令替换
来源：http://jc.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://qn.bookmarksfly.cn

[R27] 算术展开
来源：http://lq.szsharing.cn

echo $((1 + 2 * 3))
来源：http://ld.shtwfgs.cn

[R28] 浮点运算
来源：http://wb.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://qw.haigaiapp.cn

[R29] 定义函数
来源：http://dj.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lo.chemitech.net.cn

[R30] 函数返回状态码
来源：http://dr.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://rf.nicolike.cn

[R31] 局部变量
来源：http://dq.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://bd.huanxung.cn

[R32] 参数个数校验
来源：http://td.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yp.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://yd.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ev.haigaiapp.cn

[R34] 退出时清理
来源：http://ej.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xr.nicolike.cn

[R35] 后台执行并等待
来源：http://rl.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://eu.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://jj.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cc.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://pm.szxytkj.cn

files=$(ls -1)
来源：http://zf.yuexingan06.cn

[R38] 管道串联
来源：http://xo.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://dn.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://kp.muxihuayi.cn

cmd > out.log 2>&1
来源：http://jb.asd995.cn

[R40] 追加写日志
来源：http://cq.haigaiapp.cn

echo "log" >> out.log
来源：http://ae.colortex.cn

[R41] 丢弃输出
来源：http://ad.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://ak.wgjwhj.cn

[R42] 输入重定向
来源：http://bi.colortex.cn

wc -l < a.txt
来源：http://cg.panjiajie.cn

[R43] 按名字查找文件
来源：http://or.9csxet.cn

find . -name "*.log" -type f
来源：http://uc.hahajie.cn

[R44] 按修改时间查找
来源：http://bo.shtwfgs.cn

find . -mtime -7 -type f
来源：http://uo.huixiangedu.cn

[R45] 批量删除
来源：http://so.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://gm.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://kz.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fx.hnjuh.cn

[R47] sed 单行替换
来源：http://or.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xu.yuexingan06.cn

[R48] awk 取指定列
来源：http://ia.521024.cn

awk '{print $1, $3}' a.txt
来源：http://dj.newstarts.cn

[R49] awk 带条件
来源：http://xy.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xc.haigaiapp.cn

[R50] awk 求和
来源：http://st.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lz.521024.cn

[R51] 排序去重取前几
来源：http://lm.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://au.jianghongdianzi.cn

[R52] 统计行数
来源：http://dd.gzmigu.cn

wc -l a.txt
来源：http://aq.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://to.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ir.hahajie.cn

[R54] 比较两个文件
来源：http://ie.521024.cn

diff a.txt b.txt
来源：http://ly.chemitech.net.cn

[R55] 压缩与解压
来源：http://og.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ix.chemitech.net.cn

[R56] 远程拷贝
来源：http://gf.huanxung.cn

scp file user@host:/path/
来源：http://ap.haigaiapp.cn

[R57] 远程执行命令
来源：http://yk.huanxung.cn

ssh user@host 'uptime'
来源：http://nw.chemitech.net.cn

[R58] 下载文件
来源：http://nw.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://um.lnxyls.cn

[R59] 发 POST JSON
来源：http://fs.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ht.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://jp.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xn.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://ji.huixiangedu.cn

df -h;  du -sh *
来源：http://xt.hnjuh.cn

[R62] 找最占空间的文件
来源：http://iq.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://nu.yuntaijiaju.cn

[R63] 内存与进程
来源：http://hw.asd995.cn

free -h;  ps aux | grep nginx
来源：http://vl.hahajie.cn

[R64] 结束进程
来源：http://gv.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://ne.lnxyls.cn

[R65] 查看端口占用
来源：http://rz.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vp.yuexingan06.cn

[R66] 定时任务
来源：http://vn.521024.cn

crontab -e;  crontab -l
来源：http://ny.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://ib.hnjuh.cn

openssl rand -hex 16
来源：http://wg.521024.cn

[R68] 计算文件校验值
来源：http://yn.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lk.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://pd.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://ck.szsharing.cn

[R70] 时间戳与互转
来源：http://dt.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://ck.nszjky.cn

[R71] 日期格式化
来源：http://ag.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hy.521024.cn

[R72] 等待端口就绪
来源：http://mg.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ok.asd995.cn

[R73] 分割大日志
来源：http://qx.newstarts.cn

split -l 1000 big.log part_
来源：http://an.521024.cn

[R74] 批量重命名
来源：http://ci.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rt.wgjwhj.cn

[R75] 导出环境变量
来源：http://wp.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://ob.haigaiapp.cn

[R76] 使用临时文件
来源：http://pn.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xx.szxytkj.cn

[R77] 读取用户输入
来源：http://nh.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://yy.9csxet.cn

[R78] 交互式菜单
来源：http://cb.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://un.chemitech.net.cn

[R79] 解析命令行选项
来源：http://oq.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pc.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://ew.wgjwhj.cn

time ./run.sh
来源：http://qg.huanxung.cn

================================================================================
来源：http://zy.wgjwhj.cn

S. C / C++ 专题
来源：http://re.chemitech.net.cn

================================================================================
来源：http://hf.wgjwhj.cn

[S01] C：Hello World
来源：http://sk.huixiangedu.cn

#include <stdio.h>
来源：http://ns.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://my.asd995.cn

[S02] C：变量与格式化输出
来源：http://pc.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://ol.bjjhwx.cn

[S03] C：读入整数
来源：http://mp.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://qe.gzmigu.cn

[S04] C：字符串复制
来源：http://fp.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fw.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://ie.shxzskj.cn

strlen(s)
来源：http://qd.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://oc.hnjuh.cn

strcmp(a, b) == 0
来源：http://dv.huanxung.cn

[S07] C：数组遍历求和
来源：http://ss.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qe.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://eq.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wx.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://lu.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ji.521024.cn

[S10] C：指针与解引用
来源：http://vw.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://wu.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://nm.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://av.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vt.colortex.cn

fclose(f);
来源：http://pn.shxzukj.cn

[S12] C：写文件
来源：http://tu.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oh.wgjwhj.cn

[S13] C：宏定义
来源：http://tx.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sg.muxihuayi.cn

[S14] C：枚举
来源：http://gm.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ro.chemitech.net.cn

[S15] C：类型转换
来源：http://fm.jctech888.com.cn

(double) a / b
来源：http://lm.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://zc.bjjhwx.cn

x |= (1 << 3);
来源：http://lu.521024.cn

[S17] C：安全拼接字符串
来源：http://yx.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qw.muxihuayi.cn

[S18] C：命令行参数
来源：http://qq.newstarts.cn

int main(int argc, char **argv)
来源：http://wd.yuexingan06.cn

[S19] C：快速排序
来源：http://bo.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xc.huanxung.cn

[S20] C：二分查找
来源：http://rq.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hu.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://bk.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tw.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://uy.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://br.asd995.cn

[S23] C：随机数
来源：http://xm.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cj.chemitech.net.cn

[S24] C：获取本地时间
来源：http://us.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://no.szxytkj.cn

[S25] C：内存拷贝
来源：http://dr.szsharing.cn

memcpy(dst, src, n);
来源：http://qs.hnjuh.cn

[S26] C：内存清零
来源：http://av.9csxet.cn

memset(a, 0, sizeof a);
来源：http://lm.asd995.cn

[S27] C：定义常量
来源：http://ua.bookmarksfly.cn

const double PI = 3.14159;
来源：http://jb.chemitech.net.cn

[S28] C：静态变量
来源：http://li.yuexingan06.cn

static int counter = 0;
来源：http://aq.nicolike.cn

[S29] C：变参函数
来源：http://hv.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gs.shtwfgs.cn

[S30] C：头文件保护
来源：http://ts.colortex.cn

#ifndef X_H
来源：http://lm.lnxyls.cn

#define X_H
来源：http://hj.shxzskj.cn

#endif
来源：http://tc.asd995.cn

[S31] C++：Hello World
来源：http://ek.yuexingan06.cn

#include <iostream>
来源：http://hb.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://ml.szsharing.cn

[S32] C++：字符串
来源：http://ad.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://cv.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://fl.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qf.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://jq.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://bl.huanxung.cn

[S35] C++：map
来源：http://ox.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zi.lnxyls.cn

[S36] C++：unordered_map
来源：http://pf.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ud.jianghongdianzi.cn

[S37] C++：set
来源：http://an.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gu.muxihuayi.cn

[S38] C++：排序
来源：http://eq.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://rk.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://xn.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://td.wgjwhj.cn

[S40] C++：查找元素
来源：http://vi.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fs.shxzukj.cn

[S41] C++：类与构造函数
来源：http://ik.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nt.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://te.521024.cn

class B : public Base { public: void f() override {} };
来源：http://di.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://zn.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://eu.521024.cn

[S44] C++：引用传参
来源：http://ad.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://nw.nicolike.cn

[S45] C++：lambda
来源：http://an.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pk.huixiangedu.cn

[S46] C++：函数模板
来源：http://yl.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uc.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://zi.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zr.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://lv.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fj.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://vj.asd995.cn

[S49] C++：写文件
来源：http://gc.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ow.huixiangedu.cn

[S50] C++：格式化数字
来源：http://qe.huixiangedu.cn


<!-- 参考信息 -->