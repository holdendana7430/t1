代发 wailian999

[Q86] 读取 JSON 字段
来源：http://xh.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hx.asd995.cn

[Q87] JSON 字段做条件
来源：http://fn.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sp.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://ch.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ab.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fi.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://ot.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qu.huixiangedu.cn

[Q90] 生成序号列
来源：http://fk.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cr.nszjky.cn

================================================================================
来源：http://yt.hahajie.cn

R. Bash 专题
来源：http://xm.huixiangedu.cn

================================================================================
来源：http://bx.szsharing.cn

[R01] shebang 与严格模式
来源：http://ma.shtwfgs.cn

#!/usr/bin/env bash
来源：http://qu.szsharing.cn

set -euo pipefail
来源：http://wm.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://ia.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://kg.lnxyls.cn

[R03] 只读变量
来源：http://ef.jianghongdianzi.cn

readonly PI=3.14
来源：http://yp.hahajie.cn

[R04] 位置参数
来源：http://kc.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rm.muxihuayi.cn

[R05] 参数默认值
来源：http://bl.muxihuayi.cn

name="${1:-default}"
来源：http://zt.gzmigu.cn

[R06] 判断命令是否存在
来源：http://xu.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://et.huanxung.cn

[R07] if 判断文件
来源：http://if.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rx.colortex.cn

[R08] 数值比较
来源：http://yh.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ux.shxzskj.cn

[R09] 字符串比较
来源：http://jv.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://li.nicolike.cn

[R10] 正则匹配
来源：http://xd.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mf.huixiangedu.cn

[R11] case 多分支
来源：http://fy.szsharing.cn

case "$1" in
来源：http://jz.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://fs.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://cd.huanxung.cn

*)     echo "未知命令" ;;
来源：http://pc.huanxung.cn

esac
来源：http://zy.bjjhwx.cn

[R12] for 遍历文件
来源：http://bg.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://nc.haigaiapp.cn

[R13] for 计数循环
来源：http://wr.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://kp.asd995.cn

[R14] C 风格 for
来源：http://mb.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oh.shxzskj.cn

[R15] while 逐行读文件
来源：http://dc.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dz.huixiangedu.cn

[R16] until 等待条件
来源：http://zj.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gn.hahajie.cn

[R17] 数组定义与取值
来源：http://bo.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ns.asd995.cn

[R18] 遍历数组
来源：http://pf.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qd.newstarts.cn

[R19] 数组长度
来源：http://ho.yuexingan06.cn

echo "${#arr[@]}"
来源：http://ka.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://ul.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fc.szsharing.cn

[R21] 字符串长度
来源：http://ry.huixinmuqiang.cn

echo "${#s}"
来源：http://ys.bjjhwx.cn

[R22] 截取子串
来源：http://ke.panjiajie.cn

echo "${s:0:5}"
来源：http://ns.gzmigu.cn

[R23] 字符串替换
来源：http://sf.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qc.szsharing.cn

[R24] 大小写转换
来源：http://ke.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fm.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://ad.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ev.panjiajie.cn

[R26] 命令替换
来源：http://xw.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://xr.jctech888.com.cn

[R27] 算术展开
来源：http://zq.nszjky.cn

echo $((1 + 2 * 3))
来源：http://sk.muxihuayi.cn

[R28] 浮点运算
来源：http://el.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://hx.panjiajie.cn

[R29] 定义函数
来源：http://ww.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yn.wgjwhj.cn

[R30] 函数返回状态码
来源：http://ei.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://ne.yuexingan06.cn

[R31] 局部变量
来源：http://lc.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://ns.muxihuayi.cn

[R32] 参数个数校验
来源：http://bp.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qx.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://wp.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oc.wgjwhj.cn

[R34] 退出时清理
来源：http://ar.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bj.hahajie.cn

[R35] 后台执行并等待
来源：http://vc.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ba.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://fh.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fi.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://go.huixinmuqiang.cn

files=$(ls -1)
来源：http://ye.yuexingan06.cn

[R38] 管道串联
来源：http://ps.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://yn.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://nb.yuexingan06.cn

cmd > out.log 2>&1
来源：http://eh.huanxung.cn

[R40] 追加写日志
来源：http://jn.newstarts.cn

echo "log" >> out.log
来源：http://sd.nszjky.cn

[R41] 丢弃输出
来源：http://aw.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://fl.yuntaijiaju.cn

[R42] 输入重定向
来源：http://wf.newstarts.cn

wc -l < a.txt
来源：http://wj.huixiangedu.cn

[R43] 按名字查找文件
来源：http://sq.colortex.cn

find . -name "*.log" -type f
来源：http://se.521024.cn

[R44] 按修改时间查找
来源：http://qn.lnxyls.cn

find . -mtime -7 -type f
来源：http://ne.nicolike.cn

[R45] 批量删除
来源：http://ib.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://fj.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://hm.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zy.bookmarksfly.cn

[R47] sed 单行替换
来源：http://tv.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ss.muxihuayi.cn

[R48] awk 取指定列
来源：http://mv.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://yz.yuntaijiaju.cn

[R49] awk 带条件
来源：http://jk.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://le.chemitech.net.cn

[R50] awk 求和
来源：http://zw.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nz.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://py.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lg.shxzukj.cn

[R52] 统计行数
来源：http://uu.szxytkj.cn

wc -l a.txt
来源：http://ol.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://ub.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bx.nszjky.cn

[R54] 比较两个文件
来源：http://gg.hahajie.cn

diff a.txt b.txt
来源：http://tj.bookmarksfly.cn

[R55] 压缩与解压
来源：http://us.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yk.szxytkj.cn

[R56] 远程拷贝
来源：http://wf.gzmigu.cn

scp file user@host:/path/
来源：http://wq.shxzskj.cn

[R57] 远程执行命令
来源：http://qr.muxihuayi.cn

ssh user@host 'uptime'
来源：http://ss.huixinmuqiang.cn

[R58] 下载文件
来源：http://gp.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ph.wgjwhj.cn

[R59] 发 POST JSON
来源：http://tw.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://le.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://zq.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vv.yuexingan06.cn

[R61] 磁盘占用
来源：http://kb.haigaiapp.cn

df -h;  du -sh *
来源：http://ui.shxzukj.cn

[R62] 找最占空间的文件
来源：http://yk.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://nj.lnxyls.cn

[R63] 内存与进程
来源：http://ql.colortex.cn

free -h;  ps aux | grep nginx
来源：http://qe.gzmigu.cn

[R64] 结束进程
来源：http://bp.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://jv.gzmigu.cn

[R65] 查看端口占用
来源：http://rg.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gu.jctech888.com.cn

[R66] 定时任务
来源：http://mo.chemitech.net.cn

crontab -e;  crontab -l
来源：http://eo.hahajie.cn

[R67] 生成随机十六进制串
来源：http://hf.huanxung.cn

openssl rand -hex 16
来源：http://wu.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://ls.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rh.yuexingan06.cn

[R69] 生成随机密码
来源：http://wr.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://dn.lnxyls.cn

[R70] 时间戳与互转
来源：http://zg.9csxet.cn

date +%s;  date -d @1700000000
来源：http://uj.yuntaijiaju.cn

[R71] 日期格式化
来源：http://co.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hc.9csxet.cn

[R72] 等待端口就绪
来源：http://rn.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dj.huixiangedu.cn

[R73] 分割大日志
来源：http://tx.szsharing.cn

split -l 1000 big.log part_
来源：http://gd.panjiajie.cn

[R74] 批量重命名
来源：http://ye.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://li.colortex.cn

[R75] 导出环境变量
来源：http://ot.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://ci.jctech888.com.cn

[R76] 使用临时文件
来源：http://ml.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ez.newstarts.cn

[R77] 读取用户输入
来源：http://ye.chemitech.net.cn

read -rp "请输入: " ans
来源：http://uu.hahajie.cn

[R78] 交互式菜单
来源：http://tt.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tk.nicolike.cn

[R79] 解析命令行选项
来源：http://fy.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lv.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://ne.lnxyls.cn

time ./run.sh
来源：http://rt.hahajie.cn

================================================================================
来源：http://jt.yuntaijiaju.cn

S. C / C++ 专题
来源：http://rf.newstarts.cn

================================================================================
来源：http://np.newstarts.cn

[S01] C：Hello World
来源：http://bn.nszjky.cn

#include <stdio.h>
来源：http://fb.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hn.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://xa.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://hq.bjjhwx.cn

[S03] C：读入整数
来源：http://yg.huanxung.cn

int x; scanf("%d", &x);
来源：http://iz.hahajie.cn

[S04] C：字符串复制
来源：http://ik.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://we.nszjky.cn

[S05] C：字符串长度
来源：http://bp.muxihuayi.cn

strlen(s)
来源：http://wj.yuexingan06.cn

[S06] C：字符串比较
来源：http://dl.newstarts.cn

strcmp(a, b) == 0
来源：http://vx.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://yk.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qo.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://hc.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xd.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://vw.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kw.asd995.cn

[S10] C：指针与解引用
来源：http://jt.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://qi.asd995.cn

[S11] C：逐行读文件
来源：http://vs.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://ci.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xx.wgjwhj.cn

fclose(f);
来源：http://uz.colortex.cn

[S12] C：写文件
来源：http://vk.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ma.9csxet.cn

[S13] C：宏定义
来源：http://lp.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eq.asd995.cn

[S14] C：枚举
来源：http://xq.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://mz.nszjky.cn

[S15] C：类型转换
来源：http://ct.jctech888.com.cn

(double) a / b
来源：http://sn.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ts.colortex.cn

x |= (1 << 3);
来源：http://bh.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://gg.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nw.hahajie.cn

[S18] C：命令行参数
来源：http://uq.haigaiapp.cn

int main(int argc, char **argv)
来源：http://ar.jctech888.com.cn

[S19] C：快速排序
来源：http://nw.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ge.shxzskj.cn

[S20] C：二分查找
来源：http://oq.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ia.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://nm.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ee.huixiangedu.cn

[S22] C：字符串转数字
来源：http://nk.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://md.hahajie.cn

[S23] C：随机数
来源：http://kn.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zn.nszjky.cn

[S24] C：获取本地时间
来源：http://gh.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://th.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://ak.wgjwhj.cn

memcpy(dst, src, n);
来源：http://nq.bookmarksfly.cn

[S26] C：内存清零
来源：http://re.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://wz.colortex.cn

[S27] C：定义常量
来源：http://cz.newstarts.cn

const double PI = 3.14159;
来源：http://oz.521024.cn

[S28] C：静态变量
来源：http://va.9csxet.cn

static int counter = 0;
来源：http://wm.jianghongdianzi.cn

[S29] C：变参函数
来源：http://lg.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wp.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://vg.muxihuayi.cn

#ifndef X_H
来源：http://dn.chemitech.net.cn

#define X_H
来源：http://ob.bookmarksfly.cn

#endif
来源：http://na.bjjhwx.cn

[S31] C++：Hello World
来源：http://yr.shxzskj.cn

#include <iostream>
来源：http://md.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://he.jianghongdianzi.cn

[S32] C++：字符串
来源：http://tz.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://dh.panjiajie.cn

[S33] C++：vector 增删
来源：http://uo.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zz.hnjuh.cn

[S34] C++：遍历 vector
来源：http://dv.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://xe.9csxet.cn

[S35] C++：map
来源：http://dn.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mk.shxzukj.cn

[S36] C++：unordered_map
来源：http://ue.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xg.panjiajie.cn

[S37] C++：set
来源：http://rm.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://to.panjiajie.cn

[S38] C++：排序
来源：http://tj.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://xb.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://hi.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fd.wgjwhj.cn

[S40] C++：查找元素
来源：http://cw.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tk.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://nf.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tk.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://lu.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://wz.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://aj.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://cr.hahajie.cn

[S44] C++：引用传参
来源：http://pu.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://zj.huixinmuqiang.cn

[S45] C++：lambda
来源：http://qy.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dm.nszjky.cn

[S46] C++：函数模板
来源：http://cy.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sx.521024.cn

[S47] C++：结构化绑定遍历
来源：http://nz.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hx.521024.cn

[S48] C++：逐行读文件
来源：http://ab.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ix.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://qm.jctech888.com.cn

[S49] C++：写文件
来源：http://is.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wd.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://je.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vq.asd995.cn

[S51] C++：显式类型转换
来源：http://er.hahajie.cn

static_cast<double>(a) / b
来源：http://do.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://nc.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://yx.jctech888.com.cn

[S53] C++：移动语义
来源：http://ab.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://wr.panjiajie.cn

[S54] C++：异常处理
来源：http://da.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fp.hnjuh.cn

[S55] C++：结构化绑定
来源：http://es.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xg.huixiangedu.cn

[S56] C++：optional
来源：http://ms.colortex.cn


<!-- 参考信息 -->