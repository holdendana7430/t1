代发 wailian999

[Q86] 读取 JSON 字段
来源：http://cn.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ek.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://dk.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ww.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://uc.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://du.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jv.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://vn.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vs.hahajie.cn

[Q90] 生成序号列
来源：http://bt.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oi.gzmigu.cn

================================================================================
来源：http://yd.shxzukj.cn

R. Bash 专题
来源：http://mf.newstarts.cn

================================================================================
来源：http://oa.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://nz.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://nt.521024.cn

set -euo pipefail
来源：http://vu.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://lg.nszjky.cn

name="Tom"; echo "$name"
来源：http://sb.newstarts.cn

[R03] 只读变量
来源：http://mz.panjiajie.cn

readonly PI=3.14
来源：http://jx.huixiangedu.cn

[R04] 位置参数
来源：http://ms.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ua.huixiangedu.cn

[R05] 参数默认值
来源：http://iz.bookmarksfly.cn

name="${1:-default}"
来源：http://tn.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://ae.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://um.nicolike.cn

[R07] if 判断文件
来源：http://sa.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ps.gzmigu.cn

[R08] 数值比较
来源：http://ji.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yq.shxzskj.cn

[R09] 字符串比较
来源：http://np.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ps.nszjky.cn

[R10] 正则匹配
来源：http://ii.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ke.hnjuh.cn

[R11] case 多分支
来源：http://cv.yuntaijiaju.cn

case "$1" in
来源：http://bh.newstarts.cn

start) echo "启动" ;;
来源：http://yx.szsharing.cn

stop)  echo "停止" ;;
来源：http://rs.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://vc.huixiangedu.cn

esac
来源：http://oq.asd995.cn

[R12] for 遍历文件
来源：http://ap.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://jj.shxzskj.cn

[R13] for 计数循环
来源：http://wn.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://hv.huixinmuqiang.cn

[R14] C 风格 for
来源：http://mg.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uz.shtwfgs.cn

[R15] while 逐行读文件
来源：http://vf.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hp.chemitech.net.cn

[R16] until 等待条件
来源：http://yg.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dd.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://qa.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cp.colortex.cn

[R18] 遍历数组
来源：http://vq.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jo.huixinmuqiang.cn

[R19] 数组长度
来源：http://kz.nszjky.cn

echo "${#arr[@]}"
来源：http://or.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://dl.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ar.shtwfgs.cn

[R21] 字符串长度
来源：http://ch.jctech888.com.cn

echo "${#s}"
来源：http://it.muxihuayi.cn

[R22] 截取子串
来源：http://md.huanxung.cn

echo "${s:0:5}"
来源：http://ql.szxytkj.cn

[R23] 字符串替换
来源：http://ej.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sp.panjiajie.cn

[R24] 大小写转换
来源：http://or.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vh.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://af.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xv.yuexingan06.cn

[R26] 命令替换
来源：http://xi.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://oj.szsharing.cn

[R27] 算术展开
来源：http://lu.521024.cn

echo $((1 + 2 * 3))
来源：http://ht.shxzskj.cn

[R28] 浮点运算
来源：http://lo.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://xc.szxytkj.cn

[R29] 定义函数
来源：http://xb.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lz.szsharing.cn

[R30] 函数返回状态码
来源：http://dg.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://tj.colortex.cn

[R31] 局部变量
来源：http://ov.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://jz.nicolike.cn

[R32] 参数个数校验
来源：http://rp.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lh.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://tn.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bf.9csxet.cn

[R34] 退出时清理
来源：http://mb.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://by.nszjky.cn

[R35] 后台执行并等待
来源：http://ez.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cq.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://kl.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://je.szsharing.cn

[R37] 把输出赋给变量
来源：http://en.nicolike.cn

files=$(ls -1)
来源：http://po.szxytkj.cn

[R38] 管道串联
来源：http://vq.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://vw.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://ge.wgjwhj.cn

cmd > out.log 2>&1
来源：http://ts.huixiangedu.cn

[R40] 追加写日志
来源：http://sr.9csxet.cn

echo "log" >> out.log
来源：http://ru.jctech888.com.cn

[R41] 丢弃输出
来源：http://id.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://lg.huixinmuqiang.cn

[R42] 输入重定向
来源：http://rt.lnxyls.cn

wc -l < a.txt
来源：http://hz.nicolike.cn

[R43] 按名字查找文件
来源：http://yz.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://kj.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://gs.521024.cn

find . -mtime -7 -type f
来源：http://vg.nszjky.cn

[R45] 批量删除
来源：http://km.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://bh.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://oq.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bm.szxytkj.cn

[R47] sed 单行替换
来源：http://ia.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://on.nszjky.cn

[R48] awk 取指定列
来源：http://ma.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://bv.shtwfgs.cn

[R49] awk 带条件
来源：http://fg.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nd.huixiangedu.cn

[R50] awk 求和
来源：http://ou.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gl.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://ls.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yf.bjjhwx.cn

[R52] 统计行数
来源：http://iw.gzmigu.cn

wc -l a.txt
来源：http://nk.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://ow.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ea.colortex.cn

[R54] 比较两个文件
来源：http://wh.asd995.cn

diff a.txt b.txt
来源：http://ro.shxzukj.cn

[R55] 压缩与解压
来源：http://am.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jo.nszjky.cn

[R56] 远程拷贝
来源：http://qq.wgjwhj.cn

scp file user@host:/path/
来源：http://od.panjiajie.cn

[R57] 远程执行命令
来源：http://ps.szxytkj.cn

ssh user@host 'uptime'
来源：http://of.jianghongdianzi.cn

[R58] 下载文件
来源：http://wc.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://el.szsharing.cn

[R59] 发 POST JSON
来源：http://jd.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wx.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://mw.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cd.9csxet.cn

[R61] 磁盘占用
来源：http://hd.521024.cn

df -h;  du -sh *
来源：http://bg.nicolike.cn

[R62] 找最占空间的文件
来源：http://se.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://cg.bookmarksfly.cn

[R63] 内存与进程
来源：http://qn.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://zw.huanxung.cn

[R64] 结束进程
来源：http://wc.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://az.haigaiapp.cn

[R65] 查看端口占用
来源：http://mh.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rr.jctech888.com.cn

[R66] 定时任务
来源：http://sj.huixiangedu.cn

crontab -e;  crontab -l
来源：http://ys.nszjky.cn

[R67] 生成随机十六进制串
来源：http://ws.shxzukj.cn

openssl rand -hex 16
来源：http://ts.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://lc.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cq.shxzskj.cn

[R69] 生成随机密码
来源：http://kb.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://tv.szsharing.cn

[R70] 时间戳与互转
来源：http://eg.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://sc.lnxyls.cn

[R71] 日期格式化
来源：http://fr.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vg.521024.cn

[R72] 等待端口就绪
来源：http://iu.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ul.wgjwhj.cn

[R73] 分割大日志
来源：http://jd.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://cs.521024.cn

[R74] 批量重命名
来源：http://an.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vd.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://je.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://or.colortex.cn

[R76] 使用临时文件
来源：http://rq.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fk.yuexingan06.cn

[R77] 读取用户输入
来源：http://wo.asd995.cn

read -rp "请输入: " ans
来源：http://tu.szxytkj.cn

[R78] 交互式菜单
来源：http://wx.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sm.nicolike.cn

[R79] 解析命令行选项
来源：http://ms.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jw.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://ie.shxzukj.cn

time ./run.sh
来源：http://af.jctech888.com.cn

================================================================================
来源：http://pu.muxihuayi.cn

S. C / C++ 专题
来源：http://lc.hahajie.cn

================================================================================
来源：http://lk.jctech888.com.cn

[S01] C：Hello World
来源：http://zs.yuntaijiaju.cn

#include <stdio.h>
来源：http://dh.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wx.nicolike.cn

[S02] C：变量与格式化输出
来源：http://bt.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://up.newstarts.cn

[S03] C：读入整数
来源：http://cx.shxzukj.cn

int x; scanf("%d", &x);
来源：http://pt.huixiangedu.cn

[S04] C：字符串复制
来源：http://vf.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ri.nicolike.cn

[S05] C：字符串长度
来源：http://du.bjjhwx.cn

strlen(s)
来源：http://bi.hnjuh.cn

[S06] C：字符串比较
来源：http://iq.hahajie.cn

strcmp(a, b) == 0
来源：http://od.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://je.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cq.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://dp.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xp.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://zn.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hs.shtwfgs.cn

[S10] C：指针与解引用
来源：http://iu.colortex.cn

int *p = &a;  *p = 5;
来源：http://nh.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://ib.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://or.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ra.szsharing.cn

fclose(f);
来源：http://ox.chemitech.net.cn

[S12] C：写文件
来源：http://ek.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jl.asd995.cn

[S13] C：宏定义
来源：http://vz.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tz.colortex.cn

[S14] C：枚举
来源：http://pq.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://uq.bookmarksfly.cn

[S15] C：类型转换
来源：http://cz.521024.cn

(double) a / b
来源：http://lg.lnxyls.cn

[S16] C：位操作置位
来源：http://xw.shxzskj.cn

x |= (1 << 3);
来源：http://ay.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://kp.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gx.nszjky.cn

[S18] C：命令行参数
来源：http://cv.bjjhwx.cn

int main(int argc, char **argv)
来源：http://gi.asd995.cn

[S19] C：快速排序
来源：http://wt.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xv.szxytkj.cn

[S20] C：二分查找
来源：http://cs.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kr.shtwfgs.cn

[S21] C：字符类别判断
来源：http://tt.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tb.huixiangedu.cn

[S22] C：字符串转数字
来源：http://op.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cj.panjiajie.cn

[S23] C：随机数
来源：http://at.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ls.bjjhwx.cn

[S24] C：获取本地时间
来源：http://yl.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cm.yuexingan06.cn

[S25] C：内存拷贝
来源：http://my.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://ro.szxytkj.cn

[S26] C：内存清零
来源：http://ls.asd995.cn

memset(a, 0, sizeof a);
来源：http://rh.haigaiapp.cn

[S27] C：定义常量
来源：http://sw.yuexingan06.cn

const double PI = 3.14159;
来源：http://gw.yuntaijiaju.cn

[S28] C：静态变量
来源：http://wx.huixinmuqiang.cn

static int counter = 0;
来源：http://ot.gzmigu.cn

[S29] C：变参函数
来源：http://wl.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fv.lnxyls.cn

[S30] C：头文件保护
来源：http://wr.asd995.cn

#ifndef X_H
来源：http://ja.yuexingan06.cn

#define X_H
来源：http://el.bookmarksfly.cn

#endif
来源：http://cm.colortex.cn

[S31] C++：Hello World
来源：http://nn.521024.cn

#include <iostream>
来源：http://nc.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://qn.yuntaijiaju.cn

[S32] C++：字符串
来源：http://cp.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://bn.muxihuayi.cn

[S33] C++：vector 增删
来源：http://rp.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ed.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ye.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://da.hnjuh.cn

[S35] C++：map
来源：http://lb.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cd.colortex.cn

[S36] C++：unordered_map
来源：http://sc.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rq.huixiangedu.cn

[S37] C++：set
来源：http://yj.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ur.chemitech.net.cn

[S38] C++：排序
来源：http://fd.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://ud.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://hh.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ln.gzmigu.cn

[S40] C++：查找元素
来源：http://ko.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fq.shxzskj.cn

[S41] C++：类与构造函数
来源：http://zb.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://in.huanxung.cn

[S42] C++：继承与虚函数
来源：http://jl.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://cc.bookmarksfly.cn

[S43] C++：智能指针
来源：http://bi.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://cn.haigaiapp.cn

[S44] C++：引用传参
来源：http://ai.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://jk.hahajie.cn

[S45] C++：lambda
来源：http://zt.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cc.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://br.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vw.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://db.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dt.nicolike.cn

[S48] C++：逐行读文件
来源：http://mg.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qg.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://og.nicolike.cn

[S49] C++：写文件
来源：http://zc.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ep.521024.cn

[S50] C++：格式化数字
来源：http://ee.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ht.huanxung.cn

[S51] C++：显式类型转换
来源：http://fh.huanxung.cn

static_cast<double>(a) / b
来源：http://ew.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://gl.hahajie.cn

int size() const noexcept { return n_; }
来源：http://rn.bjjhwx.cn

[S53] C++：移动语义
来源：http://ao.asd995.cn

std::vector<int> w = std::move(v);
来源：http://vk.nicolike.cn

[S54] C++：异常处理
来源：http://aa.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aj.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://ji.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tz.bookmarksfly.cn

[S56] C++：optional
来源：http://cm.asd995.cn


<!-- 参考信息 -->