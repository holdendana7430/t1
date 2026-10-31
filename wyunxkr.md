代发 wailian999

[Q80] 字符串截取
来源：http://av.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sb.haigaiapp.cn

[Q81] 字符串替换
来源：http://up.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tb.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://ss.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ur.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://eg.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jv.shxzukj.cn

[Q84] 去除首尾空格
来源：http://xd.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://vc.9csxet.cn

[Q85] 数值取整
来源：http://ot.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eb.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://el.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eh.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://np.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ur.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://us.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ki.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gl.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://rh.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pr.shtwfgs.cn

[Q90] 生成序号列
来源：http://kq.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jg.panjiajie.cn

================================================================================
来源：http://pf.wgjwhj.cn

R. Bash 专题
来源：http://aq.9csxet.cn

================================================================================
来源：http://qh.shxzukj.cn

[R01] shebang 与严格模式
来源：http://lz.asd995.cn

#!/usr/bin/env bash
来源：http://wc.gzmigu.cn

set -euo pipefail
来源：http://ag.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://qu.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://ya.huanxung.cn

[R03] 只读变量
来源：http://de.szsharing.cn

readonly PI=3.14
来源：http://av.hahajie.cn

[R04] 位置参数
来源：http://wt.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://he.wgjwhj.cn

[R05] 参数默认值
来源：http://ye.shxzskj.cn

name="${1:-default}"
来源：http://ys.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://kx.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yc.asd995.cn

[R07] if 判断文件
来源：http://gj.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oc.haigaiapp.cn

[R08] 数值比较
来源：http://nm.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vj.huixinmuqiang.cn

[R09] 字符串比较
来源：http://kc.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pb.hnjuh.cn

[R10] 正则匹配
来源：http://ky.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ki.wgjwhj.cn

[R11] case 多分支
来源：http://od.colortex.cn

case "$1" in
来源：http://qc.asd995.cn

start) echo "启动" ;;
来源：http://oj.colortex.cn

stop)  echo "停止" ;;
来源：http://ge.colortex.cn

*)     echo "未知命令" ;;
来源：http://qm.bjjhwx.cn

esac
来源：http://ss.gzmigu.cn

[R12] for 遍历文件
来源：http://me.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://lt.shxzskj.cn

[R13] for 计数循环
来源：http://ds.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://kj.521024.cn

[R14] C 风格 for
来源：http://nf.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ty.panjiajie.cn

[R15] while 逐行读文件
来源：http://xg.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rz.chemitech.net.cn

[R16] until 等待条件
来源：http://dz.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lz.muxihuayi.cn

[R17] 数组定义与取值
来源：http://iw.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ct.newstarts.cn

[R18] 遍历数组
来源：http://id.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dg.lnxyls.cn

[R19] 数组长度
来源：http://pl.bjjhwx.cn

echo "${#arr[@]}"
来源：http://ml.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://xb.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://by.9csxet.cn

[R21] 字符串长度
来源：http://xt.shxzskj.cn

echo "${#s}"
来源：http://qb.colortex.cn

[R22] 截取子串
来源：http://ui.shxzukj.cn

echo "${s:0:5}"
来源：http://cw.jianghongdianzi.cn

[R23] 字符串替换
来源：http://hn.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mt.jctech888.com.cn

[R24] 大小写转换
来源：http://ln.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ch.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://gy.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://og.colortex.cn

[R26] 命令替换
来源：http://qp.521024.cn

now=$(date +%F); echo "$now"
来源：http://jr.lnxyls.cn

[R27] 算术展开
来源：http://nv.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://ul.yuexingan06.cn

[R28] 浮点运算
来源：http://mq.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://be.nszjky.cn

[R29] 定义函数
来源：http://os.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qq.hnjuh.cn

[R30] 函数返回状态码
来源：http://qw.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://hf.huixinmuqiang.cn

[R31] 局部变量
来源：http://no.521024.cn

f() { local x=1; echo "$x"; }
来源：http://ox.huixiangedu.cn

[R32] 参数个数校验
来源：http://kr.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xq.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://mb.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://la.huixiangedu.cn

[R34] 退出时清理
来源：http://cl.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vr.panjiajie.cn

[R35] 后台执行并等待
来源：http://gv.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://if.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://ar.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ay.hahajie.cn

[R37] 把输出赋给变量
来源：http://hu.9csxet.cn

files=$(ls -1)
来源：http://zn.gzmigu.cn

[R38] 管道串联
来源：http://gr.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://ov.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://ja.huixiangedu.cn

cmd > out.log 2>&1
来源：http://eu.szsharing.cn

[R40] 追加写日志
来源：http://dh.gzmigu.cn

echo "log" >> out.log
来源：http://er.hahajie.cn

[R41] 丢弃输出
来源：http://jd.9csxet.cn

cmd >/dev/null 2>&1
来源：http://li.hnjuh.cn

[R42] 输入重定向
来源：http://kj.9csxet.cn

wc -l < a.txt
来源：http://ky.wgjwhj.cn

[R43] 按名字查找文件
来源：http://ks.yuexingan06.cn

find . -name "*.log" -type f
来源：http://ch.bjjhwx.cn

[R44] 按修改时间查找
来源：http://gc.wgjwhj.cn

find . -mtime -7 -type f
来源：http://qg.jctech888.com.cn

[R45] 批量删除
来源：http://rp.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://gr.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://ap.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ig.wgjwhj.cn

[R47] sed 单行替换
来源：http://gf.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gi.chemitech.net.cn

[R48] awk 取指定列
来源：http://nm.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://lk.szxytkj.cn

[R49] awk 带条件
来源：http://hm.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pq.nicolike.cn

[R50] awk 求和
来源：http://mm.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wn.newstarts.cn

[R51] 排序去重取前几
来源：http://iu.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dh.shtwfgs.cn

[R52] 统计行数
来源：http://tz.bookmarksfly.cn

wc -l a.txt
来源：http://eu.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://gh.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wx.jctech888.com.cn

[R54] 比较两个文件
来源：http://wi.huixinmuqiang.cn

diff a.txt b.txt
来源：http://py.9csxet.cn

[R55] 压缩与解压
来源：http://le.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hp.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://se.nszjky.cn

scp file user@host:/path/
来源：http://nr.9csxet.cn

[R57] 远程执行命令
来源：http://te.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ge.gzmigu.cn

[R58] 下载文件
来源：http://os.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mc.shxzskj.cn

[R59] 发 POST JSON
来源：http://kz.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://af.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://oj.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zb.szxytkj.cn

[R61] 磁盘占用
来源：http://oq.szxytkj.cn

df -h;  du -sh *
来源：http://eq.9csxet.cn

[R62] 找最占空间的文件
来源：http://tb.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://uy.szxytkj.cn

[R63] 内存与进程
来源：http://mv.colortex.cn

free -h;  ps aux | grep nginx
来源：http://nn.nicolike.cn

[R64] 结束进程
来源：http://tx.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://wh.nszjky.cn

[R65] 查看端口占用
来源：http://ax.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jp.shxzskj.cn

[R66] 定时任务
来源：http://wx.hnjuh.cn

crontab -e;  crontab -l
来源：http://nd.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://ue.wgjwhj.cn

openssl rand -hex 16
来源：http://md.9csxet.cn

[R68] 计算文件校验值
来源：http://ka.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gp.bjjhwx.cn

[R69] 生成随机密码
来源：http://me.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://ax.wgjwhj.cn

[R70] 时间戳与互转
来源：http://jx.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://yt.bookmarksfly.cn

[R71] 日期格式化
来源：http://ja.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ly.shtwfgs.cn

[R72] 等待端口就绪
来源：http://uo.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vd.huanxung.cn

[R73] 分割大日志
来源：http://ob.bjjhwx.cn

split -l 1000 big.log part_
来源：http://di.shxzukj.cn

[R74] 批量重命名
来源：http://ub.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nx.huanxung.cn

[R75] 导出环境变量
来源：http://vn.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://uy.huixiangedu.cn

[R76] 使用临时文件
来源：http://by.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ge.hahajie.cn

[R77] 读取用户输入
来源：http://uh.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://zk.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://tr.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rg.colortex.cn

[R79] 解析命令行选项
来源：http://ix.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vh.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://er.szsharing.cn

time ./run.sh
来源：http://tz.yuexingan06.cn

================================================================================
来源：http://co.gzmigu.cn

S. C / C++ 专题
来源：http://vm.521024.cn

================================================================================
来源：http://qr.chemitech.net.cn

[S01] C：Hello World
来源：http://po.hnjuh.cn

#include <stdio.h>
来源：http://le.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://il.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://wc.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://uu.jctech888.com.cn

[S03] C：读入整数
来源：http://mf.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://yj.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://zc.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rl.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://pi.shtwfgs.cn

strlen(s)
来源：http://km.9csxet.cn

[S06] C：字符串比较
来源：http://mj.panjiajie.cn

strcmp(a, b) == 0
来源：http://yr.521024.cn

[S07] C：数组遍历求和
来源：http://bw.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yu.colortex.cn

[S08] C：动态内存分配与释放
来源：http://qj.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://us.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://qa.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dh.huanxung.cn

[S10] C：指针与解引用
来源：http://lb.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://cg.gzmigu.cn

[S11] C：逐行读文件
来源：http://sv.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://qu.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sz.huixinmuqiang.cn

fclose(f);
来源：http://xt.huanxung.cn

[S12] C：写文件
来源：http://er.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xs.yuexingan06.cn

[S13] C：宏定义
来源：http://lk.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yr.huixiangedu.cn

[S14] C：枚举
来源：http://ox.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://tz.bjjhwx.cn

[S15] C：类型转换
来源：http://bb.huixiangedu.cn

(double) a / b
来源：http://rq.gzmigu.cn

[S16] C：位操作置位
来源：http://bt.shtwfgs.cn

x |= (1 << 3);
来源：http://na.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://bu.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rf.shtwfgs.cn

[S18] C：命令行参数
来源：http://xf.shxzskj.cn

int main(int argc, char **argv)
来源：http://yb.lnxyls.cn

[S19] C：快速排序
来源：http://zo.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hg.wgjwhj.cn

[S20] C：二分查找
来源：http://zt.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shxzukj.cn

[S21] C：字符类别判断
来源：http://gf.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://il.hahajie.cn

[S22] C：字符串转数字
来源：http://dq.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://me.jianghongdianzi.cn

[S23] C：随机数
来源：http://bl.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vv.colortex.cn

[S24] C：获取本地时间
来源：http://sd.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gr.muxihuayi.cn

[S25] C：内存拷贝
来源：http://am.huanxung.cn

memcpy(dst, src, n);
来源：http://kp.jianghongdianzi.cn

[S26] C：内存清零
来源：http://hq.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://vn.szsharing.cn

[S27] C：定义常量
来源：http://jg.gzmigu.cn

const double PI = 3.14159;
来源：http://qy.shtwfgs.cn

[S28] C：静态变量
来源：http://wh.hnjuh.cn

static int counter = 0;
来源：http://on.nicolike.cn

[S29] C：变参函数
来源：http://wp.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ou.muxihuayi.cn

[S30] C：头文件保护
来源：http://tw.huixiangedu.cn

#ifndef X_H
来源：http://cp.shtwfgs.cn

#define X_H
来源：http://nm.haigaiapp.cn

#endif
来源：http://do.yuexingan06.cn

[S31] C++：Hello World
来源：http://hh.huixiangedu.cn

#include <iostream>
来源：http://hf.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://xr.muxihuayi.cn

[S32] C++：字符串
来源：http://du.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://jh.9csxet.cn

[S33] C++：vector 增删
来源：http://zh.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yo.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://om.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://ij.yuntaijiaju.cn

[S35] C++：map
来源：http://wq.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://au.9csxet.cn

[S36] C++：unordered_map
来源：http://ao.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ha.huixinmuqiang.cn

[S37] C++：set
来源：http://fr.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://co.haigaiapp.cn

[S38] C++：排序
来源：http://rm.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://lq.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://xk.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vm.gzmigu.cn

[S40] C++：查找元素
来源：http://to.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kl.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://nk.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ql.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://ok.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://me.shxzukj.cn

[S43] C++：智能指针
来源：http://wg.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://jk.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://kd.hahajie.cn

void inc(int &x) { ++x; }
来源：http://du.szsharing.cn

[S45] C++：lambda
来源：http://az.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ci.colortex.cn

[S46] C++：函数模板
来源：http://mh.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ha.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://uj.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fk.colortex.cn

[S48] C++：逐行读文件
来源：http://au.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nt.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://ka.jianghongdianzi.cn

[S49] C++：写文件
来源：http://vr.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://na.asd995.cn

[S50] C++：格式化数字
来源：http://nj.521024.cn


<!-- 参考信息 -->