代发 wailian999

[Q82] 字符长度与字节长度
来源：http://pj.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://da.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://fo.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://so.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://iz.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://vi.wgjwhj.cn

[Q85] 数值取整
来源：http://nh.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fl.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://ab.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lj.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://wu.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fc.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://gg.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nz.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bk.panjiajie.cn

[Q89] 判断表是否存在
来源：http://gp.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hn.lnxyls.cn

[Q90] 生成序号列
来源：http://nm.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rt.shxzskj.cn

================================================================================
来源：http://yn.shtwfgs.cn

R. Bash 专题
来源：http://dq.shxzskj.cn

================================================================================
来源：http://tc.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://ve.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://fq.shxzukj.cn

set -euo pipefail
来源：http://nd.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://th.szsharing.cn

name="Tom"; echo "$name"
来源：http://px.haigaiapp.cn

[R03] 只读变量
来源：http://nr.bjjhwx.cn

readonly PI=3.14
来源：http://nj.colortex.cn

[R04] 位置参数
来源：http://aj.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ne.lnxyls.cn

[R05] 参数默认值
来源：http://ho.shtwfgs.cn

name="${1:-default}"
来源：http://ur.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://al.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vv.nszjky.cn

[R07] if 判断文件
来源：http://ga.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ca.asd995.cn

[R08] 数值比较
来源：http://gh.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ne.wgjwhj.cn

[R09] 字符串比较
来源：http://tj.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wi.panjiajie.cn

[R10] 正则匹配
来源：http://xu.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hg.shxzukj.cn

[R11] case 多分支
来源：http://zf.lnxyls.cn

case "$1" in
来源：http://ss.newstarts.cn

start) echo "启动" ;;
来源：http://ph.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://yg.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://kh.szxytkj.cn

esac
来源：http://dp.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://to.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://nb.bookmarksfly.cn

[R13] for 计数循环
来源：http://kt.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://nj.yuexingan06.cn

[R14] C 风格 for
来源：http://lx.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fp.yuexingan06.cn

[R15] while 逐行读文件
来源：http://hx.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yl.colortex.cn

[R16] until 等待条件
来源：http://wd.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pc.nicolike.cn

[R17] 数组定义与取值
来源：http://pg.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ox.hahajie.cn

[R18] 遍历数组
来源：http://dg.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sa.nszjky.cn

[R19] 数组长度
来源：http://dg.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://kr.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://on.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wk.bookmarksfly.cn

[R21] 字符串长度
来源：http://av.bjjhwx.cn

echo "${#s}"
来源：http://tb.9csxet.cn

[R22] 截取子串
来源：http://hf.hahajie.cn

echo "${s:0:5}"
来源：http://uf.gzmigu.cn

[R23] 字符串替换
来源：http://fz.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://da.szsharing.cn

[R24] 大小写转换
来源：http://je.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bn.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://ip.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ip.newstarts.cn

[R26] 命令替换
来源：http://xl.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://jp.yuntaijiaju.cn

[R27] 算术展开
来源：http://xd.521024.cn

echo $((1 + 2 * 3))
来源：http://vy.colortex.cn

[R28] 浮点运算
来源：http://wq.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://uc.huixinmuqiang.cn

[R29] 定义函数
来源：http://ep.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xd.huanxung.cn

[R30] 函数返回状态码
来源：http://uo.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://hg.chemitech.net.cn

[R31] 局部变量
来源：http://ou.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://xe.wgjwhj.cn

[R32] 参数个数校验
来源：http://cd.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ko.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://qm.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://it.huixinmuqiang.cn

[R34] 退出时清理
来源：http://yn.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oa.colortex.cn

[R35] 后台执行并等待
来源：http://bc.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bc.huanxung.cn

[R36] 并发执行多个任务
来源：http://or.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qk.nicolike.cn

[R37] 把输出赋给变量
来源：http://sh.wgjwhj.cn

files=$(ls -1)
来源：http://ma.newstarts.cn

[R38] 管道串联
来源：http://rw.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://gx.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://lk.shxzskj.cn

cmd > out.log 2>&1
来源：http://af.bjjhwx.cn

[R40] 追加写日志
来源：http://cy.521024.cn

echo "log" >> out.log
来源：http://wy.shxzskj.cn

[R41] 丢弃输出
来源：http://ca.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://sb.huanxung.cn

[R42] 输入重定向
来源：http://ck.colortex.cn

wc -l < a.txt
来源：http://ns.haigaiapp.cn

[R43] 按名字查找文件
来源：http://ad.wgjwhj.cn

find . -name "*.log" -type f
来源：http://hf.huixiangedu.cn

[R44] 按修改时间查找
来源：http://zx.szxytkj.cn

find . -mtime -7 -type f
来源：http://jj.jianghongdianzi.cn

[R45] 批量删除
来源：http://jf.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://if.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://wc.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qw.colortex.cn

[R47] sed 单行替换
来源：http://xq.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://co.hahajie.cn

[R48] awk 取指定列
来源：http://st.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://js.jctech888.com.cn

[R49] awk 带条件
来源：http://dh.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xi.9csxet.cn

[R50] awk 求和
来源：http://cd.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://np.szxytkj.cn

[R51] 排序去重取前几
来源：http://fy.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://je.gzmigu.cn

[R52] 统计行数
来源：http://jz.bookmarksfly.cn

wc -l a.txt
来源：http://uo.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://oz.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ow.wgjwhj.cn

[R54] 比较两个文件
来源：http://gc.huixiangedu.cn

diff a.txt b.txt
来源：http://ax.muxihuayi.cn

[R55] 压缩与解压
来源：http://qv.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sb.bookmarksfly.cn

[R56] 远程拷贝
来源：http://vz.wgjwhj.cn

scp file user@host:/path/
来源：http://gt.szsharing.cn

[R57] 远程执行命令
来源：http://rx.521024.cn

ssh user@host 'uptime'
来源：http://sr.nszjky.cn

[R58] 下载文件
来源：http://wm.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ni.nszjky.cn

[R59] 发 POST JSON
来源：http://fs.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xi.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://rf.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xa.haigaiapp.cn

[R61] 磁盘占用
来源：http://zv.hnjuh.cn

df -h;  du -sh *
来源：http://iz.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://nf.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://kr.szxytkj.cn

[R63] 内存与进程
来源：http://xs.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://ee.shtwfgs.cn

[R64] 结束进程
来源：http://fg.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://pg.nicolike.cn

[R65] 查看端口占用
来源：http://xv.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uh.bookmarksfly.cn

[R66] 定时任务
来源：http://ld.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://vx.colortex.cn

[R67] 生成随机十六进制串
来源：http://dr.gzmigu.cn

openssl rand -hex 16
来源：http://ls.shxzskj.cn

[R68] 计算文件校验值
来源：http://ge.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yo.hnjuh.cn

[R69] 生成随机密码
来源：http://ld.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://rx.9csxet.cn

[R70] 时间戳与互转
来源：http://xl.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://qo.huixiangedu.cn

[R71] 日期格式化
来源：http://pb.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ng.hahajie.cn

[R72] 等待端口就绪
来源：http://gp.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ga.newstarts.cn

[R73] 分割大日志
来源：http://ie.yuexingan06.cn

split -l 1000 big.log part_
来源：http://ny.newstarts.cn

[R74] 批量重命名
来源：http://ga.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hn.newstarts.cn

[R75] 导出环境变量
来源：http://uy.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://lv.shxzukj.cn

[R76] 使用临时文件
来源：http://ln.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cn.szsharing.cn

[R77] 读取用户输入
来源：http://hy.hahajie.cn

read -rp "请输入: " ans
来源：http://vs.nicolike.cn

[R78] 交互式菜单
来源：http://iu.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ha.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://tb.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uu.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://vr.bjjhwx.cn

time ./run.sh
来源：http://ou.jianghongdianzi.cn

================================================================================
来源：http://bn.hnjuh.cn

S. C / C++ 专题
来源：http://vc.huixiangedu.cn

================================================================================
来源：http://ry.huanxung.cn

[S01] C：Hello World
来源：http://ya.bookmarksfly.cn

#include <stdio.h>
来源：http://qs.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dl.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://iv.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://rs.jctech888.com.cn

[S03] C：读入整数
来源：http://ub.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://le.newstarts.cn

[S04] C：字符串复制
来源：http://gg.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nx.panjiajie.cn

[S05] C：字符串长度
来源：http://gg.szsharing.cn

strlen(s)
来源：http://uy.shxzskj.cn

[S06] C：字符串比较
来源：http://ah.nszjky.cn

strcmp(a, b) == 0
来源：http://nu.9csxet.cn

[S07] C：数组遍历求和
来源：http://ou.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bt.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://im.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jr.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://ix.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://go.huanxung.cn

[S10] C：指针与解引用
来源：http://mq.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://xj.gzmigu.cn

[S11] C：逐行读文件
来源：http://ep.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://yf.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://td.bjjhwx.cn

fclose(f);
来源：http://wh.nicolike.cn

[S12] C：写文件
来源：http://ek.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ig.huanxung.cn

[S13] C：宏定义
来源：http://fw.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zu.bookmarksfly.cn

[S14] C：枚举
来源：http://la.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://ij.yuntaijiaju.cn

[S15] C：类型转换
来源：http://gx.shxzukj.cn

(double) a / b
来源：http://xa.9csxet.cn

[S16] C：位操作置位
来源：http://dj.wgjwhj.cn

x |= (1 << 3);
来源：http://gv.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://rs.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yn.huanxung.cn

[S18] C：命令行参数
来源：http://nv.panjiajie.cn

int main(int argc, char **argv)
来源：http://zf.huanxung.cn

[S19] C：快速排序
来源：http://cy.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ct.muxihuayi.cn

[S20] C：二分查找
来源：http://lw.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://as.szxytkj.cn

[S21] C：字符类别判断
来源：http://kj.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fg.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://gu.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gx.hnjuh.cn

[S23] C：随机数
来源：http://ri.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rt.gzmigu.cn

[S24] C：获取本地时间
来源：http://jq.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fq.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://cc.asd995.cn

memcpy(dst, src, n);
来源：http://wx.yuexingan06.cn

[S26] C：内存清零
来源：http://fx.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://pg.panjiajie.cn

[S27] C：定义常量
来源：http://kl.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://ay.shxzskj.cn

[S28] C：静态变量
来源：http://kp.yuexingan06.cn

static int counter = 0;
来源：http://aa.colortex.cn

[S29] C：变参函数
来源：http://gh.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://da.lnxyls.cn

[S30] C：头文件保护
来源：http://hz.colortex.cn

#ifndef X_H
来源：http://fv.hnjuh.cn

#define X_H
来源：http://zg.bjjhwx.cn

#endif
来源：http://zv.shtwfgs.cn

[S31] C++：Hello World
来源：http://tz.shtwfgs.cn

#include <iostream>
来源：http://uy.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://ko.wgjwhj.cn

[S32] C++：字符串
来源：http://xy.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://oy.shtwfgs.cn

[S33] C++：vector 增删
来源：http://gt.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cz.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://gd.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://ua.shtwfgs.cn

[S35] C++：map
来源：http://zh.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gt.shxzukj.cn

[S36] C++：unordered_map
来源：http://da.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://np.521024.cn

[S37] C++：set
来源：http://dc.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fd.haigaiapp.cn

[S38] C++：排序
来源：http://cu.asd995.cn

std::sort(v.begin(), v.end());
来源：http://wk.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://cx.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tw.bjjhwx.cn

[S40] C++：查找元素
来源：http://hn.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yh.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://qu.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://li.hahajie.cn

[S42] C++：继承与虚函数
来源：http://ui.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://qt.huanxung.cn

[S43] C++：智能指针
来源：http://ac.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://xf.colortex.cn

[S44] C++：引用传参
来源：http://tf.colortex.cn

void inc(int &x) { ++x; }
来源：http://pc.chemitech.net.cn

[S45] C++：lambda
来源：http://rb.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://td.szsharing.cn

[S46] C++：函数模板
来源：http://po.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ac.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://wi.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hj.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://ii.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ak.521024.cn

while (std::getline(in, line)) { }
来源：http://tn.asd995.cn

[S49] C++：写文件
来源：http://ok.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qa.chemitech.net.cn

[S50] C++：格式化数字
来源：http://nz.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vh.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://es.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://mi.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://aa.jctech888.com.cn


<!-- 参考信息 -->