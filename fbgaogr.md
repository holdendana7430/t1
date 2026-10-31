代发 wailian999

R. Bash 专题
来源：http://kz.wgjwhj.cn

================================================================================
来源：http://bm.521024.cn

[R01] shebang 与严格模式
来源：http://ru.yuexingan06.cn

#!/usr/bin/env bash
来源：http://lx.huanxung.cn

set -euo pipefail
来源：http://fk.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://hl.huanxung.cn

name="Tom"; echo "$name"
来源：http://oq.hnjuh.cn

[R03] 只读变量
来源：http://mh.yuexingan06.cn

readonly PI=3.14
来源：http://jg.huanxung.cn

[R04] 位置参数
来源：http://mf.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pd.chemitech.net.cn

[R05] 参数默认值
来源：http://ty.yuntaijiaju.cn

name="${1:-default}"
来源：http://bw.lnxyls.cn

[R06] 判断命令是否存在
来源：http://hs.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zr.panjiajie.cn

[R07] if 判断文件
来源：http://pe.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kj.szsharing.cn

[R08] 数值比较
来源：http://kk.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://io.chemitech.net.cn

[R09] 字符串比较
来源：http://hw.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tb.newstarts.cn

[R10] 正则匹配
来源：http://fg.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zl.huixiangedu.cn

[R11] case 多分支
来源：http://wq.9csxet.cn

case "$1" in
来源：http://om.bjjhwx.cn

start) echo "启动" ;;
来源：http://te.newstarts.cn

stop)  echo "停止" ;;
来源：http://qc.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://qy.haigaiapp.cn

esac
来源：http://vq.newstarts.cn

[R12] for 遍历文件
来源：http://vk.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://fb.huixinmuqiang.cn

[R13] for 计数循环
来源：http://ja.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://tx.huixiangedu.cn

[R14] C 风格 for
来源：http://co.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dn.muxihuayi.cn

[R15] while 逐行读文件
来源：http://cc.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ns.chemitech.net.cn

[R16] until 等待条件
来源：http://sr.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://af.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://kh.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ty.huixiangedu.cn

[R18] 遍历数组
来源：http://rn.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mh.shxzskj.cn

[R19] 数组长度
来源：http://rw.colortex.cn

echo "${#arr[@]}"
来源：http://or.panjiajie.cn

[R20] 关联数组（字典）
来源：http://vw.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bt.jctech888.com.cn

[R21] 字符串长度
来源：http://wx.asd995.cn

echo "${#s}"
来源：http://nf.hahajie.cn

[R22] 截取子串
来源：http://sw.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://ot.huixinmuqiang.cn

[R23] 字符串替换
来源：http://ps.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vn.yuexingan06.cn

[R24] 大小写转换
来源：http://ah.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cz.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://lh.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sm.asd995.cn

[R26] 命令替换
来源：http://ly.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://rx.nicolike.cn

[R27] 算术展开
来源：http://yl.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://al.muxihuayi.cn

[R28] 浮点运算
来源：http://rn.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://ew.gzmigu.cn

[R29] 定义函数
来源：http://oz.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fh.wgjwhj.cn

[R30] 函数返回状态码
来源：http://id.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ym.lnxyls.cn

[R31] 局部变量
来源：http://tq.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://rj.gzmigu.cn

[R32] 参数个数校验
来源：http://ix.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jh.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://hy.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kc.jianghongdianzi.cn

[R34] 退出时清理
来源：http://vn.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ks.chemitech.net.cn

[R35] 后台执行并等待
来源：http://bh.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kg.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://zl.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hx.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://lg.newstarts.cn

files=$(ls -1)
来源：http://iy.panjiajie.cn

[R38] 管道串联
来源：http://oh.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://pa.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://cc.panjiajie.cn

cmd > out.log 2>&1
来源：http://uf.shxzskj.cn

[R40] 追加写日志
来源：http://re.521024.cn

echo "log" >> out.log
来源：http://pf.shxzukj.cn

[R41] 丢弃输出
来源：http://ow.huanxung.cn

cmd >/dev/null 2>&1
来源：http://qr.shxzskj.cn

[R42] 输入重定向
来源：http://ya.9csxet.cn

wc -l < a.txt
来源：http://lp.nicolike.cn

[R43] 按名字查找文件
来源：http://nt.nicolike.cn

find . -name "*.log" -type f
来源：http://la.huixiangedu.cn

[R44] 按修改时间查找
来源：http://ou.haigaiapp.cn

find . -mtime -7 -type f
来源：http://hu.szxytkj.cn

[R45] 批量删除
来源：http://nx.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://se.szsharing.cn

[R46] 递归替换文件内容
来源：http://lb.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lw.szxytkj.cn

[R47] sed 单行替换
来源：http://rs.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ru.521024.cn

[R48] awk 取指定列
来源：http://vj.521024.cn

awk '{print $1, $3}' a.txt
来源：http://fa.szxytkj.cn

[R49] awk 带条件
来源：http://hz.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ck.521024.cn

[R50] awk 求和
来源：http://sc.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ey.bjjhwx.cn

[R51] 排序去重取前几
来源：http://hw.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vw.haigaiapp.cn

[R52] 统计行数
来源：http://xe.nicolike.cn

wc -l a.txt
来源：http://jl.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://ht.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vh.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://mo.521024.cn

diff a.txt b.txt
来源：http://zo.shtwfgs.cn

[R55] 压缩与解压
来源：http://ha.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://le.521024.cn

[R56] 远程拷贝
来源：http://gl.jianghongdianzi.cn

scp file user@host:/path/
来源：http://jo.huixiangedu.cn

[R57] 远程执行命令
来源：http://ww.gzmigu.cn

ssh user@host 'uptime'
来源：http://xm.521024.cn

[R58] 下载文件
来源：http://rz.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wj.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://qw.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://es.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ki.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yb.hahajie.cn

[R61] 磁盘占用
来源：http://ez.nszjky.cn

df -h;  du -sh *
来源：http://qg.shxzskj.cn

[R62] 找最占空间的文件
来源：http://ni.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://aa.chemitech.net.cn

[R63] 内存与进程
来源：http://fy.asd995.cn

free -h;  ps aux | grep nginx
来源：http://gm.chemitech.net.cn

[R64] 结束进程
来源：http://db.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://tu.panjiajie.cn

[R65] 查看端口占用
来源：http://vp.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://le.huixiangedu.cn

[R66] 定时任务
来源：http://xs.yuexingan06.cn

crontab -e;  crontab -l
来源：http://ec.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://rs.panjiajie.cn

openssl rand -hex 16
来源：http://be.szxytkj.cn

[R68] 计算文件校验值
来源：http://mj.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mz.hahajie.cn

[R69] 生成随机密码
来源：http://rb.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://pv.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://ca.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://da.shxzskj.cn

[R71] 日期格式化
来源：http://cm.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gm.9csxet.cn

[R72] 等待端口就绪
来源：http://ls.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mx.colortex.cn

[R73] 分割大日志
来源：http://li.chemitech.net.cn

split -l 1000 big.log part_
来源：http://ho.asd995.cn

[R74] 批量重命名
来源：http://hx.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dm.nszjky.cn

[R75] 导出环境变量
来源：http://jo.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://uk.jctech888.com.cn

[R76] 使用临时文件
来源：http://hx.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jv.bjjhwx.cn

[R77] 读取用户输入
来源：http://in.muxihuayi.cn

read -rp "请输入: " ans
来源：http://bp.hnjuh.cn

[R78] 交互式菜单
来源：http://xg.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pd.shxzskj.cn

[R79] 解析命令行选项
来源：http://hi.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qx.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://zm.yuntaijiaju.cn

time ./run.sh
来源：http://ob.colortex.cn

================================================================================
来源：http://hp.hahajie.cn

S. C / C++ 专题
来源：http://bg.gzmigu.cn

================================================================================
来源：http://ck.chemitech.net.cn

[S01] C：Hello World
来源：http://jc.muxihuayi.cn

#include <stdio.h>
来源：http://on.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ch.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://ef.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://iv.nicolike.cn

[S03] C：读入整数
来源：http://wv.shxzukj.cn

int x; scanf("%d", &x);
来源：http://ov.hnjuh.cn

[S04] C：字符串复制
来源：http://fc.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bc.bookmarksfly.cn

[S05] C：字符串长度
来源：http://iq.shtwfgs.cn

strlen(s)
来源：http://hz.nicolike.cn

[S06] C：字符串比较
来源：http://hi.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://da.panjiajie.cn

[S07] C：数组遍历求和
来源：http://lj.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kc.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://qo.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cl.colortex.cn

[S09] C：结构体定义与初始化
来源：http://hp.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xt.jctech888.com.cn

[S10] C：指针与解引用
来源：http://bt.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://xc.muxihuayi.cn

[S11] C：逐行读文件
来源：http://oe.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://yc.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qi.yuntaijiaju.cn

fclose(f);
来源：http://su.9csxet.cn

[S12] C：写文件
来源：http://ct.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eo.jianghongdianzi.cn

[S13] C：宏定义
来源：http://kq.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ow.gzmigu.cn

[S14] C：枚举
来源：http://mm.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://oa.panjiajie.cn

[S15] C：类型转换
来源：http://eb.shtwfgs.cn

(double) a / b
来源：http://at.shtwfgs.cn

[S16] C：位操作置位
来源：http://sa.panjiajie.cn

x |= (1 << 3);
来源：http://nt.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://bl.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qe.huanxung.cn

[S18] C：命令行参数
来源：http://ta.haigaiapp.cn

int main(int argc, char **argv)
来源：http://nv.yuntaijiaju.cn

[S19] C：快速排序
来源：http://as.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cb.panjiajie.cn

[S20] C：二分查找
来源：http://kw.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gz.gzmigu.cn

[S21] C：字符类别判断
来源：http://ud.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jw.shtwfgs.cn

[S22] C：字符串转数字
来源：http://op.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lh.jianghongdianzi.cn

[S23] C：随机数
来源：http://ta.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jy.nszjky.cn

[S24] C：获取本地时间
来源：http://hh.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kq.huanxung.cn

[S25] C：内存拷贝
来源：http://lj.szxytkj.cn

memcpy(dst, src, n);
来源：http://ny.nicolike.cn

[S26] C：内存清零
来源：http://gh.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://qg.lnxyls.cn

[S27] C：定义常量
来源：http://zg.bookmarksfly.cn

const double PI = 3.14159;
来源：http://xd.yuexingan06.cn

[S28] C：静态变量
来源：http://ma.shxzukj.cn

static int counter = 0;
来源：http://vm.panjiajie.cn

[S29] C：变参函数
来源：http://ut.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://br.colortex.cn

[S30] C：头文件保护
来源：http://fm.panjiajie.cn

#ifndef X_H
来源：http://kd.nszjky.cn

#define X_H
来源：http://fc.wgjwhj.cn

#endif
来源：http://ca.bjjhwx.cn

[S31] C++：Hello World
来源：http://mg.lnxyls.cn

#include <iostream>
来源：http://wr.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://lm.newstarts.cn

[S32] C++：字符串
来源：http://fn.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://hz.gzmigu.cn

[S33] C++：vector 增删
来源：http://ve.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oi.shxzskj.cn

[S34] C++：遍历 vector
来源：http://cd.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ic.szsharing.cn

[S35] C++：map
来源：http://do.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xd.nszjky.cn

[S36] C++：unordered_map
来源：http://wk.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qy.9csxet.cn

[S37] C++：set
来源：http://ot.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ll.huixinmuqiang.cn

[S38] C++：排序
来源：http://au.521024.cn

std::sort(v.begin(), v.end());
来源：http://ev.asd995.cn

[S39] C++：自定义比较器排序
来源：http://md.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xz.nicolike.cn

[S40] C++：查找元素
来源：http://uk.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hf.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://cn.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://em.szsharing.cn

[S42] C++：继承与虚函数
来源：http://eg.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://oe.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://gr.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://jk.gzmigu.cn

[S44] C++：引用传参
来源：http://wo.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://fn.shtwfgs.cn

[S45] C++：lambda
来源：http://zh.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://al.chemitech.net.cn

[S46] C++：函数模板
来源：http://wb.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ic.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://yt.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xa.huanxung.cn

[S48] C++：逐行读文件
来源：http://hc.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yy.huanxung.cn

while (std::getline(in, line)) { }
来源：http://fo.huixinmuqiang.cn

[S49] C++：写文件
来源：http://wu.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uf.szxytkj.cn

[S50] C++：格式化数字
来源：http://qj.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nt.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://xw.bjjhwx.cn

static_cast<double>(a) / b
来源：http://oa.521024.cn

[S52] C++：const 与 noexcept
来源：http://uu.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://fm.huixiangedu.cn

[S53] C++：移动语义
来源：http://ej.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://fp.lnxyls.cn

[S54] C++：异常处理
来源：http://wo.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rp.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://fw.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ui.szsharing.cn

[S56] C++：optional
来源：http://qx.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xl.nicolike.cn

[S57] C++：编译期常量
来源：http://ex.huixinmuqiang.cn

constexpr int N = 10;
来源：http://cq.panjiajie.cn

[S58] C++：命名空间
来源：http://fx.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://uc.hnjuh.cn

[S59] C++：静态断言
来源：http://vf.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ws.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://dd.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gf.szsharing.cn

================================================================================
来源：http://yq.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mb.hahajie.cn

================================================================================
来源：http://zt.yuexingan06.cn


<!-- 参考信息 -->