代发 wailian999

[Q80] 字符串截取
来源：http://wc.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ru.hnjuh.cn

[Q81] 字符串替换
来源：http://xl.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rn.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://aa.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gj.yuexingan06.cn

[Q83] 大小写转换
来源：http://nk.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hs.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://hc.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://hd.bookmarksfly.cn

[Q85] 数值取整
来源：http://pp.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ad.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://on.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jq.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://cq.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cy.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://wc.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wc.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fu.newstarts.cn

[Q89] 判断表是否存在
来源：http://vy.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pr.nicolike.cn

[Q90] 生成序号列
来源：http://ul.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sh.huixinmuqiang.cn

================================================================================
来源：http://sb.chemitech.net.cn

R. Bash 专题
来源：http://og.yuexingan06.cn

================================================================================
来源：http://mu.hahajie.cn

[R01] shebang 与严格模式
来源：http://ot.asd995.cn

#!/usr/bin/env bash
来源：http://sw.lnxyls.cn

set -euo pipefail
来源：http://dn.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://dr.colortex.cn

name="Tom"; echo "$name"
来源：http://js.gzmigu.cn

[R03] 只读变量
来源：http://bx.szsharing.cn

readonly PI=3.14
来源：http://jm.521024.cn

[R04] 位置参数
来源：http://ks.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lg.bookmarksfly.cn

[R05] 参数默认值
来源：http://dy.shxzskj.cn

name="${1:-default}"
来源：http://aw.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://fz.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wo.shxzskj.cn

[R07] if 判断文件
来源：http://su.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qv.wgjwhj.cn

[R08] 数值比较
来源：http://ff.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vp.szxytkj.cn

[R09] 字符串比较
来源：http://kl.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kq.chemitech.net.cn

[R10] 正则匹配
来源：http://pf.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fd.newstarts.cn

[R11] case 多分支
来源：http://dd.shxzukj.cn

case "$1" in
来源：http://il.huixiangedu.cn

start) echo "启动" ;;
来源：http://ql.nicolike.cn

stop)  echo "停止" ;;
来源：http://kf.521024.cn

*)     echo "未知命令" ;;
来源：http://zm.521024.cn

esac
来源：http://gz.yuexingan06.cn

[R12] for 遍历文件
来源：http://ep.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://uf.lnxyls.cn

[R13] for 计数循环
来源：http://et.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://tg.bjjhwx.cn

[R14] C 风格 for
来源：http://ur.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sk.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://fx.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nw.bjjhwx.cn

[R16] until 等待条件
来源：http://zk.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pk.panjiajie.cn

[R17] 数组定义与取值
来源：http://br.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fy.szsharing.cn

[R18] 遍历数组
来源：http://hn.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://er.colortex.cn

[R19] 数组长度
来源：http://zp.lnxyls.cn

echo "${#arr[@]}"
来源：http://ny.shxzukj.cn

[R20] 关联数组（字典）
来源：http://dg.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eu.yuntaijiaju.cn

[R21] 字符串长度
来源：http://aa.chemitech.net.cn

echo "${#s}"
来源：http://ww.szsharing.cn

[R22] 截取子串
来源：http://ql.asd995.cn

echo "${s:0:5}"
来源：http://cx.huixiangedu.cn

[R23] 字符串替换
来源：http://vo.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jj.9csxet.cn

[R24] 大小写转换
来源：http://sw.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vf.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://vo.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uv.jianghongdianzi.cn

[R26] 命令替换
来源：http://nn.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://yb.521024.cn

[R27] 算术展开
来源：http://oh.asd995.cn

echo $((1 + 2 * 3))
来源：http://ng.haigaiapp.cn

[R28] 浮点运算
来源：http://lp.521024.cn

echo "scale=2; 10/3" | bc
来源：http://in.newstarts.cn

[R29] 定义函数
来源：http://xd.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mf.lnxyls.cn

[R30] 函数返回状态码
来源：http://ek.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://we.wgjwhj.cn

[R31] 局部变量
来源：http://sf.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://rl.bookmarksfly.cn

[R32] 参数个数校验
来源：http://go.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ff.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://va.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jq.bookmarksfly.cn

[R34] 退出时清理
来源：http://nx.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ec.9csxet.cn

[R35] 后台执行并等待
来源：http://xo.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xl.shxzskj.cn

[R36] 并发执行多个任务
来源：http://te.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kb.lnxyls.cn

[R37] 把输出赋给变量
来源：http://mk.shxzukj.cn

files=$(ls -1)
来源：http://rx.nszjky.cn

[R38] 管道串联
来源：http://ky.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://vk.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://bj.colortex.cn

cmd > out.log 2>&1
来源：http://pq.hahajie.cn

[R40] 追加写日志
来源：http://vh.jctech888.com.cn

echo "log" >> out.log
来源：http://zt.jctech888.com.cn

[R41] 丢弃输出
来源：http://oo.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://my.yuntaijiaju.cn

[R42] 输入重定向
来源：http://pb.lnxyls.cn

wc -l < a.txt
来源：http://uk.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://zy.nicolike.cn

find . -name "*.log" -type f
来源：http://bo.szsharing.cn

[R44] 按修改时间查找
来源：http://te.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://fy.jctech888.com.cn

[R45] 批量删除
来源：http://ae.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://yv.asd995.cn

[R46] 递归替换文件内容
来源：http://wd.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mw.9csxet.cn

[R47] sed 单行替换
来源：http://fn.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ua.bjjhwx.cn

[R48] awk 取指定列
来源：http://xl.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://ud.shxzukj.cn

[R49] awk 带条件
来源：http://zb.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cb.wgjwhj.cn

[R50] awk 求和
来源：http://ab.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xf.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://zl.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://db.nicolike.cn

[R52] 统计行数
来源：http://rp.panjiajie.cn

wc -l a.txt
来源：http://po.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://pm.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mz.muxihuayi.cn

[R54] 比较两个文件
来源：http://fg.panjiajie.cn

diff a.txt b.txt
来源：http://iy.chemitech.net.cn

[R55] 压缩与解压
来源：http://cv.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rk.hahajie.cn

[R56] 远程拷贝
来源：http://ld.haigaiapp.cn

scp file user@host:/path/
来源：http://pg.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://em.newstarts.cn

ssh user@host 'uptime'
来源：http://bt.nszjky.cn

[R58] 下载文件
来源：http://nr.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dx.9csxet.cn

[R59] 发 POST JSON
来源：http://ok.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rv.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://ag.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jh.lnxyls.cn

[R61] 磁盘占用
来源：http://vq.muxihuayi.cn

df -h;  du -sh *
来源：http://hp.panjiajie.cn

[R62] 找最占空间的文件
来源：http://cd.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://zp.521024.cn

[R63] 内存与进程
来源：http://oq.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://cf.jianghongdianzi.cn

[R64] 结束进程
来源：http://lw.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://gm.colortex.cn

[R65] 查看端口占用
来源：http://sj.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://di.bjjhwx.cn

[R66] 定时任务
来源：http://yn.shxzukj.cn

crontab -e;  crontab -l
来源：http://kn.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://wi.colortex.cn

openssl rand -hex 16
来源：http://zz.nicolike.cn

[R68] 计算文件校验值
来源：http://tp.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qe.hahajie.cn

[R69] 生成随机密码
来源：http://gm.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://ml.lnxyls.cn

[R70] 时间戳与互转
来源：http://ag.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://ot.bookmarksfly.cn

[R71] 日期格式化
来源：http://ed.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wr.hnjuh.cn

[R72] 等待端口就绪
来源：http://nd.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yc.chemitech.net.cn

[R73] 分割大日志
来源：http://hp.colortex.cn

split -l 1000 big.log part_
来源：http://vj.huixinmuqiang.cn

[R74] 批量重命名
来源：http://ti.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mu.9csxet.cn

[R75] 导出环境变量
来源：http://xa.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://mt.9csxet.cn

[R76] 使用临时文件
来源：http://vu.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tl.szsharing.cn

[R77] 读取用户输入
来源：http://yi.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://fc.hnjuh.cn

[R78] 交互式菜单
来源：http://oi.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kv.panjiajie.cn

[R79] 解析命令行选项
来源：http://wu.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://np.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://aq.yuntaijiaju.cn

time ./run.sh
来源：http://ua.bookmarksfly.cn

================================================================================
来源：http://kh.asd995.cn

S. C / C++ 专题
来源：http://eu.szxytkj.cn

================================================================================
来源：http://km.asd995.cn

[S01] C：Hello World
来源：http://kc.521024.cn

#include <stdio.h>
来源：http://yn.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vf.hahajie.cn

[S02] C：变量与格式化输出
来源：http://ex.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://es.shtwfgs.cn

[S03] C：读入整数
来源：http://qt.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://rk.szxytkj.cn

[S04] C：字符串复制
来源：http://ui.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fj.yuexingan06.cn

[S05] C：字符串长度
来源：http://ds.nicolike.cn

strlen(s)
来源：http://li.muxihuayi.cn

[S06] C：字符串比较
来源：http://xl.asd995.cn

strcmp(a, b) == 0
来源：http://hd.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://hn.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ul.asd995.cn

[S08] C：动态内存分配与释放
来源：http://yf.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zt.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://qh.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xc.lnxyls.cn

[S10] C：指针与解引用
来源：http://nk.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://dr.yuexingan06.cn

[S11] C：逐行读文件
来源：http://gc.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://dl.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mm.521024.cn

fclose(f);
来源：http://oh.yuntaijiaju.cn

[S12] C：写文件
来源：http://ln.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sh.gzmigu.cn

[S13] C：宏定义
来源：http://nc.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xz.jctech888.com.cn

[S14] C：枚举
来源：http://dk.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://yl.panjiajie.cn

[S15] C：类型转换
来源：http://zk.chemitech.net.cn

(double) a / b
来源：http://ud.panjiajie.cn

[S16] C：位操作置位
来源：http://rt.shxzukj.cn

x |= (1 << 3);
来源：http://sj.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://ff.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sa.nicolike.cn

[S18] C：命令行参数
来源：http://zt.szsharing.cn

int main(int argc, char **argv)
来源：http://qo.shxzskj.cn

[S19] C：快速排序
来源：http://cw.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xl.panjiajie.cn

[S20] C：二分查找
来源：http://mc.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lx.9csxet.cn

[S21] C：字符类别判断
来源：http://zf.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dr.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://zg.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xh.newstarts.cn

[S23] C：随机数
来源：http://uy.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://he.gzmigu.cn

[S24] C：获取本地时间
来源：http://qq.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://id.newstarts.cn

[S25] C：内存拷贝
来源：http://em.asd995.cn

memcpy(dst, src, n);
来源：http://ht.shxzskj.cn

[S26] C：内存清零
来源：http://fe.huanxung.cn

memset(a, 0, sizeof a);
来源：http://ol.muxihuayi.cn

[S27] C：定义常量
来源：http://bn.muxihuayi.cn

const double PI = 3.14159;
来源：http://mg.hnjuh.cn

[S28] C：静态变量
来源：http://tr.shxzskj.cn

static int counter = 0;
来源：http://qe.newstarts.cn

[S29] C：变参函数
来源：http://ot.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://an.jctech888.com.cn

[S30] C：头文件保护
来源：http://co.huixinmuqiang.cn

#ifndef X_H
来源：http://lc.hahajie.cn

#define X_H
来源：http://cq.shtwfgs.cn

#endif
来源：http://hf.shxzukj.cn

[S31] C++：Hello World
来源：http://vc.hahajie.cn

#include <iostream>
来源：http://xg.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://nw.yuntaijiaju.cn

[S32] C++：字符串
来源：http://pb.521024.cn

std::string s = "hi";  s += "!";
来源：http://zh.muxihuayi.cn

[S33] C++：vector 增删
来源：http://qc.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nd.colortex.cn

[S34] C++：遍历 vector
来源：http://vb.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://ck.yuntaijiaju.cn

[S35] C++：map
来源：http://mr.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ds.colortex.cn

[S36] C++：unordered_map
来源：http://gx.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nf.bjjhwx.cn

[S37] C++：set
来源：http://gk.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wp.521024.cn

[S38] C++：排序
来源：http://mu.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://rc.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://nu.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dy.szxytkj.cn

[S40] C++：查找元素
来源：http://vs.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://be.521024.cn

[S41] C++：类与构造函数
来源：http://rj.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cr.szsharing.cn

[S42] C++：继承与虚函数
来源：http://um.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://kv.haigaiapp.cn

[S43] C++：智能指针
来源：http://ic.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://qf.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://sf.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://dj.colortex.cn

[S45] C++：lambda
来源：http://xz.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://is.huanxung.cn

[S46] C++：函数模板
来源：http://sg.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pk.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://ee.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oc.colortex.cn

[S48] C++：逐行读文件
来源：http://wn.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vb.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://ju.szxytkj.cn

[S49] C++：写文件
来源：http://wg.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jv.haigaiapp.cn

[S50] C++：格式化数字
来源：http://ss.haigaiapp.cn


<!-- 参考信息 -->