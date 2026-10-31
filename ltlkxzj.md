代发 wailian999

[Q86] 读取 JSON 字段
来源：http://gr.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gs.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://lc.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ro.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://vf.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dp.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fd.shxzskj.cn

[Q89] 判断表是否存在
来源：http://sp.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dg.szsharing.cn

[Q90] 生成序号列
来源：http://kd.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hi.shxzukj.cn

================================================================================
来源：http://et.szsharing.cn

R. Bash 专题
来源：http://dh.chemitech.net.cn

================================================================================
来源：http://us.panjiajie.cn

[R01] shebang 与严格模式
来源：http://ul.panjiajie.cn

#!/usr/bin/env bash
来源：http://ev.huixiangedu.cn

set -euo pipefail
来源：http://rh.nszjky.cn

[R02] 变量赋值与使用
来源：http://xv.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://tn.haigaiapp.cn

[R03] 只读变量
来源：http://le.lnxyls.cn

readonly PI=3.14
来源：http://gh.lnxyls.cn

[R04] 位置参数
来源：http://uo.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ox.9csxet.cn

[R05] 参数默认值
来源：http://bf.huixinmuqiang.cn

name="${1:-default}"
来源：http://xt.panjiajie.cn

[R06] 判断命令是否存在
来源：http://hc.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gw.gzmigu.cn

[R07] if 判断文件
来源：http://hd.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nc.lnxyls.cn

[R08] 数值比较
来源：http://df.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qq.521024.cn

[R09] 字符串比较
来源：http://pf.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ld.hahajie.cn

[R10] 正则匹配
来源：http://bx.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zm.hnjuh.cn

[R11] case 多分支
来源：http://bw.lnxyls.cn

case "$1" in
来源：http://fw.haigaiapp.cn

start) echo "启动" ;;
来源：http://rt.nicolike.cn

stop)  echo "停止" ;;
来源：http://wb.521024.cn

*)     echo "未知命令" ;;
来源：http://dg.hnjuh.cn

esac
来源：http://bf.gzmigu.cn

[R12] for 遍历文件
来源：http://jt.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://rt.gzmigu.cn

[R13] for 计数循环
来源：http://db.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://la.colortex.cn

[R14] C 风格 for
来源：http://ye.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rs.chemitech.net.cn

[R15] while 逐行读文件
来源：http://eo.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pb.szxytkj.cn

[R16] until 等待条件
来源：http://or.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ue.hnjuh.cn

[R17] 数组定义与取值
来源：http://zh.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zk.gzmigu.cn

[R18] 遍历数组
来源：http://ae.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wb.nicolike.cn

[R19] 数组长度
来源：http://zw.asd995.cn

echo "${#arr[@]}"
来源：http://vc.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://ma.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jq.lnxyls.cn

[R21] 字符串长度
来源：http://iy.muxihuayi.cn

echo "${#s}"
来源：http://lb.hahajie.cn

[R22] 截取子串
来源：http://gt.bookmarksfly.cn

echo "${s:0:5}"
来源：http://tr.lnxyls.cn

[R23] 字符串替换
来源：http://zh.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gl.asd995.cn

[R24] 大小写转换
来源：http://uv.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://od.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://ue.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uk.shxzukj.cn

[R26] 命令替换
来源：http://ix.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://id.wgjwhj.cn

[R27] 算术展开
来源：http://xy.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://mq.szxytkj.cn

[R28] 浮点运算
来源：http://mv.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://mn.9csxet.cn

[R29] 定义函数
来源：http://wh.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yl.colortex.cn

[R30] 函数返回状态码
来源：http://tn.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://gk.yuntaijiaju.cn

[R31] 局部变量
来源：http://jh.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://xh.shtwfgs.cn

[R32] 参数个数校验
来源：http://vp.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lb.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://cf.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hi.shxzukj.cn

[R34] 退出时清理
来源：http://ci.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nw.yuexingan06.cn

[R35] 后台执行并等待
来源：http://gn.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://es.9csxet.cn

[R36] 并发执行多个任务
来源：http://zd.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pk.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://ml.9csxet.cn

files=$(ls -1)
来源：http://og.colortex.cn

[R38] 管道串联
来源：http://zz.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://yb.colortex.cn

[R39] 重定向标准输出与错误
来源：http://kd.gzmigu.cn

cmd > out.log 2>&1
来源：http://bw.yuexingan06.cn

[R40] 追加写日志
来源：http://sr.yuntaijiaju.cn

echo "log" >> out.log
来源：http://ws.szxytkj.cn

[R41] 丢弃输出
来源：http://vt.9csxet.cn

cmd >/dev/null 2>&1
来源：http://mx.jctech888.com.cn

[R42] 输入重定向
来源：http://ma.muxihuayi.cn

wc -l < a.txt
来源：http://kn.jctech888.com.cn

[R43] 按名字查找文件
来源：http://na.asd995.cn

find . -name "*.log" -type f
来源：http://tn.szsharing.cn

[R44] 按修改时间查找
来源：http://ys.huixiangedu.cn

find . -mtime -7 -type f
来源：http://ty.szsharing.cn

[R45] 批量删除
来源：http://uy.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://dt.hnjuh.cn

[R46] 递归替换文件内容
来源：http://mn.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gn.bjjhwx.cn

[R47] sed 单行替换
来源：http://ck.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ht.asd995.cn

[R48] awk 取指定列
来源：http://ad.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://gh.521024.cn

[R49] awk 带条件
来源：http://fu.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zr.asd995.cn

[R50] awk 求和
来源：http://ou.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://te.521024.cn

[R51] 排序去重取前几
来源：http://ns.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xb.haigaiapp.cn

[R52] 统计行数
来源：http://ti.muxihuayi.cn

wc -l a.txt
来源：http://aq.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://rg.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mm.panjiajie.cn

[R54] 比较两个文件
来源：http://uo.szsharing.cn

diff a.txt b.txt
来源：http://yo.hahajie.cn

[R55] 压缩与解压
来源：http://ma.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wv.shtwfgs.cn

[R56] 远程拷贝
来源：http://iv.yuexingan06.cn

scp file user@host:/path/
来源：http://dq.nicolike.cn

[R57] 远程执行命令
来源：http://cb.huixiangedu.cn

ssh user@host 'uptime'
来源：http://zi.gzmigu.cn

[R58] 下载文件
来源：http://ww.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gt.nszjky.cn

[R59] 发 POST JSON
来源：http://ym.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xh.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://sr.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gi.lnxyls.cn

[R61] 磁盘占用
来源：http://fz.jianghongdianzi.cn

df -h;  du -sh *
来源：http://wo.szxytkj.cn

[R62] 找最占空间的文件
来源：http://wg.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://qo.szsharing.cn

[R63] 内存与进程
来源：http://cg.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://jo.521024.cn

[R64] 结束进程
来源：http://me.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://jp.hnjuh.cn

[R65] 查看端口占用
来源：http://pp.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fn.huanxung.cn

[R66] 定时任务
来源：http://pw.huixiangedu.cn

crontab -e;  crontab -l
来源：http://ww.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://mw.haigaiapp.cn

openssl rand -hex 16
来源：http://hc.huanxung.cn

[R68] 计算文件校验值
来源：http://ej.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rg.shxzskj.cn

[R69] 生成随机密码
来源：http://hz.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://lh.bjjhwx.cn

[R70] 时间戳与互转
来源：http://tb.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://dk.panjiajie.cn

[R71] 日期格式化
来源：http://jb.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xn.nszjky.cn

[R72] 等待端口就绪
来源：http://oq.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ue.huixiangedu.cn

[R73] 分割大日志
来源：http://eo.jctech888.com.cn

split -l 1000 big.log part_
来源：http://ge.lnxyls.cn

[R74] 批量重命名
来源：http://zw.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sv.newstarts.cn

[R75] 导出环境变量
来源：http://yt.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://md.nicolike.cn

[R76] 使用临时文件
来源：http://mp.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zb.9csxet.cn

[R77] 读取用户输入
来源：http://og.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://ii.hnjuh.cn

[R78] 交互式菜单
来源：http://do.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zx.muxihuayi.cn

[R79] 解析命令行选项
来源：http://ko.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ft.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://fj.huanxung.cn

time ./run.sh
来源：http://um.shtwfgs.cn

================================================================================
来源：http://xg.9csxet.cn

S. C / C++ 专题
来源：http://fb.lnxyls.cn

================================================================================
来源：http://pc.colortex.cn

[S01] C：Hello World
来源：http://yb.huixiangedu.cn

#include <stdio.h>
来源：http://co.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uf.nicolike.cn

[S02] C：变量与格式化输出
来源：http://ks.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://ec.lnxyls.cn

[S03] C：读入整数
来源：http://nv.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://ss.muxihuayi.cn

[S04] C：字符串复制
来源：http://jv.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iz.newstarts.cn

[S05] C：字符串长度
来源：http://nt.yuntaijiaju.cn

strlen(s)
来源：http://pk.szxytkj.cn

[S06] C：字符串比较
来源：http://vt.newstarts.cn

strcmp(a, b) == 0
来源：http://av.newstarts.cn

[S07] C：数组遍历求和
来源：http://do.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hj.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://dd.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xd.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://sw.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dv.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://mq.asd995.cn

int *p = &a;  *p = 5;
来源：http://rm.asd995.cn

[S11] C：逐行读文件
来源：http://vf.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://kt.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ac.szxytkj.cn

fclose(f);
来源：http://qb.huixinmuqiang.cn

[S12] C：写文件
来源：http://jj.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uv.9csxet.cn

[S13] C：宏定义
来源：http://hr.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hf.huixinmuqiang.cn

[S14] C：枚举
来源：http://yj.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://uo.haigaiapp.cn

[S15] C：类型转换
来源：http://pw.panjiajie.cn

(double) a / b
来源：http://nl.bookmarksfly.cn

[S16] C：位操作置位
来源：http://xr.wgjwhj.cn

x |= (1 << 3);
来源：http://ba.huanxung.cn

[S17] C：安全拼接字符串
来源：http://sm.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fl.hahajie.cn

[S18] C：命令行参数
来源：http://la.huixiangedu.cn

int main(int argc, char **argv)
来源：http://ky.panjiajie.cn

[S19] C：快速排序
来源：http://kh.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fh.yuexingan06.cn

[S20] C：二分查找
来源：http://ei.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://my.shxzukj.cn

[S21] C：字符类别判断
来源：http://zp.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.asd995.cn

[S22] C：字符串转数字
来源：http://mj.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oo.lnxyls.cn

[S23] C：随机数
来源：http://oi.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ss.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://qs.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jh.szxytkj.cn

[S25] C：内存拷贝
来源：http://ki.szxytkj.cn

memcpy(dst, src, n);
来源：http://ka.haigaiapp.cn

[S26] C：内存清零
来源：http://dr.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://sf.wgjwhj.cn

[S27] C：定义常量
来源：http://ps.newstarts.cn

const double PI = 3.14159;
来源：http://uf.bookmarksfly.cn

[S28] C：静态变量
来源：http://fp.chemitech.net.cn

static int counter = 0;
来源：http://tp.huixinmuqiang.cn

[S29] C：变参函数
来源：http://go.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fg.colortex.cn

[S30] C：头文件保护
来源：http://ra.jianghongdianzi.cn

#ifndef X_H
来源：http://ae.bookmarksfly.cn

#define X_H
来源：http://zq.szsharing.cn

#endif
来源：http://yy.shxzskj.cn

[S31] C++：Hello World
来源：http://ca.newstarts.cn

#include <iostream>
来源：http://qz.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://qy.colortex.cn

[S32] C++：字符串
来源：http://ya.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://ar.lnxyls.cn

[S33] C++：vector 增删
来源：http://ow.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ri.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://me.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://iv.panjiajie.cn

[S35] C++：map
来源：http://vv.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yb.521024.cn

[S36] C++：unordered_map
来源：http://af.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cl.colortex.cn

[S37] C++：set
来源：http://nu.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jh.huixiangedu.cn

[S38] C++：排序
来源：http://yl.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://gy.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://jt.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ya.szsharing.cn

[S40] C++：查找元素
来源：http://jk.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eo.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://ee.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pt.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://kk.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://pd.bookmarksfly.cn

[S43] C++：智能指针
来源：http://cb.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://wq.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://pl.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://ht.9csxet.cn

[S45] C++：lambda
来源：http://hr.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nx.asd995.cn

[S46] C++：函数模板
来源：http://wm.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hv.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://oy.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ak.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://wz.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ko.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://cq.bookmarksfly.cn

[S49] C++：写文件
来源：http://jy.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qm.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://qq.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://om.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://gy.nszjky.cn

static_cast<double>(a) / b
来源：http://cv.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://xl.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://rv.szxytkj.cn

[S53] C++：移动语义
来源：http://en.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://ht.haigaiapp.cn

[S54] C++：异常处理
来源：http://ja.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ev.shxzukj.cn

[S55] C++：结构化绑定
来源：http://wi.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pl.hahajie.cn

[S56] C++：optional
来源：http://iy.yuntaijiaju.cn


<!-- 参考信息 -->