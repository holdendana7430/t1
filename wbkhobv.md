代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/geetdslna.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gprkpuodf.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gptrfvgsl.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/ghvhkyqrh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gjruixksy.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gweorwydx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/ghlacysbp.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxgmeherk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gtvbufyfs.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gqkwfuomi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gjohiqcqk.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gthwatyrl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gzgyyskwo.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/ggkskippk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gioxybhic.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gyxrhamoi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gnjiuobpt.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gpdtexwbh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gxgiijaut.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gtuifbfeu.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gcbfhoxrh.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gzhqrkenq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/godemcmmw.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gscdxroba.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gnojrxlwd.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gakyuluek.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gqcnqhmmr.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gyyyttecc.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gyghvcmze.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gitteytpp.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gwllsuayw.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/goxdvgovg.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gevvyqrbi.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gblufcvfg.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gqludibpp.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gazpfxnqq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gwawmobyk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gfnotuqzd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gnbcfzogn.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/giamldchp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gaxmsjouy.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gvcoexzwm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfknvcgbh.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gjwtezasq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/giclrmteg.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gxeyicfbb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gcbhxihlc.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gqyjuakpo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gxlkvhchu.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gghhimcsm.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gofitxuxx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gdbvasuvf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gtfyhdvkn.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gomujwpga.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbgfmbivz.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gejrnaqvu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gdgjxemoz.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gangmmzuo.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gowvezhtx.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gwgsmkekw.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gqjbafgco.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/giposqjex.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gbvkjodfe.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/giyuqmlac.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gbsceuysh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gucjvyljw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gqtyjqxuz.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/grpavedii.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/giwejpsml.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/grymjgfjh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gubjpkyda.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gooxeqlrv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/glrotykuc.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/guuhkpeod.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gjibfxifx.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gqdrvvgzu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gckkguaic.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/goyxjpygs.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gysdstxeo.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gscvtmqer.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/ghlmgiipk.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gifkvjkxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gxjlmppxu.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/grbxlieir.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gkxrnbcre.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gqfubpwuy.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gvuajrsso.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/grszoqmmi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gysbvmtoy.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gmmtnpbqm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gggtohfhs.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gxmkogdrk.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gnesdxbvc.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gpdcokdur.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gtwymbshw.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ghrflcids.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gkkwblxer.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gttamycxj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gklwrsrje.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gqutjwmjk.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gbkxheqts.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gnjjhpydz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gmdbhditm.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gdaitkwfi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gbnasjegf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/ghxfiubof.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gkgbtwxan.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gncgrbuaa.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gduuiloaj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gukemmsvd.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gaiguzaxc.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gtqbydmhh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gciqwwzwz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/glltzawmf.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gtxhnunem.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gtwymzbaf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gqifrboxy.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gqkomesnd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gwecyveix.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gpzptfrik.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gvqcpqenh.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gfcfasfsn.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gvyonpzwt.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gqwztuyma.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/grboliouu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gzjtyvjwj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gfkqbjegh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gotrmkkws.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/grouhxbnc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gkudlqvgp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gxocznchy.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gpnowwxdn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gxqneuobo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gkltphnnf.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gljtiiqnz.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gaocnskkt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/glwfurzdt.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gvfufoiwe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gkofdzzzm.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/grohvxgpa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gqwrvhgkj.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/glnfmoakr.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gbhjbdibg.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/geutmwsve.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggdrkhdop.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glbhmxxws.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gvxmelhxw.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gnsbfjmnb.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gnwrlqzyt.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gjulfdlbw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gnrhskprt.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gizcrqosp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gecixxxeo.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gqhcsrawv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gintxbkec.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gwbvunpuz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/giyixzrsm.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gyjwkdzpu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gwkokmdqa.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gfekdkneq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gapzgrxxf.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gcxrumsoz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gjsmtqcjj.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gmkieipiw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gufsjhvgg.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gcvwqfyue.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gtogqiaxa.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/guxaxwyek.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gpdclljhj.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gpckogbxu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/ggofjyewi.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gbvigpcri.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gmkayqqfm.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gnrvwdwea.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gvqsdnqoi.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjgeymiiw.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/geptlrftm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gyllkccul.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gyqklgyxo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gaifmvcej.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gkoppsikj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/ghhmjpfqu.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gvmmjxlvg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gwrirjhcf.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gyoolaodu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gltamzmgr.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/grxsrryvm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gqogoyviq.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gqflzhifg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gpcgawkbl.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/ggrlihjpv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gagmfjyuw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gwkxmfkbu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gekqienrh.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gqblwmfwy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gwntolpaz.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gpmqntqkz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gnwjfaund.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gisfqjiap.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gorviovju.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gkllulmry.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbqdngb.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gbccvmekx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gapgvnxnv.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gmjkhlqsw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gepqdkdsf.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gdvgmahmt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gupimmmbe.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gtjbfzexu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gmewlpowx.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gxwqqkvpf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gmoxcxbzb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gouyethph.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gsbzzfixk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gfwjcuspa.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gthcgigcj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggiffjohz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/ggycnognz.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/guuyiflto.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gcbjxgaza.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gmcrthqcx.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gnfodqhyw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gjnmpnncn.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gtfozubnh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gyhrmgzap.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/grjngntsi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gzjejqmqw.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gqtutjofl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gimuowejd.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gqpmqjrct.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gsapuzxat.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gcfjvmgpo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gwtffznfk.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gixscvfus.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gmbkxcwsi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gkzeobbpw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gnzxygioc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnrfhouhf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gvywrqzdg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdrbjmuhy.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxdmvobcf.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gyrzeaqvt.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gmopvfnec.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gnsuotbxv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gqwwyntcc.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/glfhxmlpi.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gxqqumjtr.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gasraiwmy.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gcapnrhtg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gtfrgeqgi.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gxfisenhr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzxgtqqnq.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gabpqkvqo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/grdczkjak.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/ghpzkpras.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gqssztoge.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gdjdylpcz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/geszzgpfc.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gwonelxzj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gzyiapddh.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gjxxdioky.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gwgbkjwju.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gzoccdpyf.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gabjradlp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gsotenomv.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gexgubugh.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/ggzgcitzr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gnygflqxx.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/goputbums.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gkieoznxp.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gvjdsvogd.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gdypkgikm.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gimefegfd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ghnlpddqv.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/grzxnjwqf.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/guyfmaejb.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gzzjiahbm.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gvikpccsj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gfzfbguca.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gfqdpjzub.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gkyvgrpng.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/ghgzqsrgh.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/grlrvefth.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gcingilue.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gsjmlxboe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gqbjucmkd.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gjzijdczi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnlxrxwql.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gcvnhcmol.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gjskaymyw.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gsylyhqmr.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gryavfkuj.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gebudjgrw.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gciuimeac.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/grulwsqud.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gnsixginr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gzraldncb.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/ghpdabkmj.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gfbgtgnae.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/glzqldgil.sHtML


<!-- 参考信息 -->