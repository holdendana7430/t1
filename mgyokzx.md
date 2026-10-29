代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gupwfhnkh.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gtcciwsbm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gmcpfuujw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gtypojzse.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gxboqoatu.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/glvxqulax.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gcukodjiw.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/glhcvdpve.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gjycrfzzj.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gwjihyekl.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gmwmeghqn.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzrquvobm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gsxulovwa.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gbwwqvzjn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gvxxdjozc.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gfpsetbua.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gyqmwhmzd.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gyxecnmjy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gbvjnvbgh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gtcrvtpgn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/geearrwun.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gnjtmpkyd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/glmkpxnpu.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gkyszfiwv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gpyjzmavk.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/geewykxps.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/ggflmxzsb.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gpvlyivzk.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gdsgyxegu.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gusaexksf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gsqufqnfh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/ggucoarqw.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gaigzdsus.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/guwjjbfbh.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gujsipoor.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gistmeneo.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/goojuhemo.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gizqgjnks.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/givnjnoug.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/grbytojuc.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gnyhajuzr.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gdbsygdvt.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gpyjnockh.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gwoalpdif.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gjtvahgsv.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gomhqkelj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/goemdbnow.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gzhwhcoji.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gdqgrdzsq.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gtabfmhel.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/ganjfbpof.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gokgjefiu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gycgdbhyb.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gljcizryy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/ghlxyfgkv.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gzwonraok.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gbzkfchpm.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gmennluoq.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/garljoacn.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/grmmebftc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gorggewrq.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/geilwbevu.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/glnyhqwfu.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gdjncktrr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gzkdqtajw.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gwgxvyvdi.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gotchxglg.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/ggjphxnad.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gnofoqhuq.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gxzztlglr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/grnovttlt.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gmbnvcare.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gtxsnaunc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gdwdgvekd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gneladsow.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gxxxjsshk.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gmczmenco.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gicpkosdt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gztsvntzb.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gdajyzlue.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gmnupravs.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gcsegheof.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gplzbyzyo.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gijcjdgbz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gjvdanpzx.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gwmztxrwy.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/grmhckwmg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gwdlpedsr.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/glflfrmzy.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gmjrlarza.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxabqlmfj.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gcslfywpc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gzxbjodan.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/geibfpofw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gkvzbtidf.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gjpsganpp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gjdelfbvs.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gvccttvwp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gmrpsdwhg.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gymooebcp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gqegwivrp.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gcdzrambl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gnropfcpb.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gxcppiztz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gbzxktere.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gpwmzsaua.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gxcpayxwx.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gtnsdjlvh.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/ghtibbdjc.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gxepfoipg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gsxlnwhsr.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gyltqqsmj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gnqoiuuis.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/ghntkhdrz.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gmsfwjdmw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpigayrsu.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gjodamoxx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfxkxotql.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gbllgblxf.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gblseaufm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/grkwyfmse.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gmvwuuakh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gbqkgdneo.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gvxyvegkd.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gepngalcg.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gqwphvvsc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/guqrthlkg.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gpvbyjfqe.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gpxkgkhty.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/grlcejfwn.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gkcmxiztr.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gpxbwgtcf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gviunbfpe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gevchkzpb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/ghexyqafq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gylrxxihu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/ggpxvukzb.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/geqsjvskc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gwtpgbouh.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/guyodvvqd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gpvnqdoso.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gowexrtym.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/goxqfvmmh.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gaqidnolv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/guhdtlnam.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gnowwsoax.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gmmavzizb.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gzjhqlocl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/goskowpys.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gvjsvwbhs.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gwkmszijq.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gamygonlp.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/grjvjmwrj.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gdnaayqkc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/givsoxocw.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gsitsdafr.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gcuuothkf.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/ggxbvjedl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gwhjavsok.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gijuqhffw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gouqjgqrb.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gspcsvwle.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gbazhvgls.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gegyotkyf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gqcbvmixa.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gsigcfyxm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gokurolmh.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gbxbszior.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gwzartxal.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gicyneiyc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gyiyfkqza.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gizysjyfk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gwzybsrtu.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/ghhdktpqc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfogjowja.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gebtlzuro.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gqlumdjuy.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gpwnmjpqy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/giltlcyeo.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gdnczyndh.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gwetblirk.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/grtdglpws.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gvpkvrmdp.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbkgsslpn.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gnwglynmf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gnfnrycwp.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gxlclrozx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gftnqmwqx.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gxlwmksza.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gcawqdjtq.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gwxvdveor.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghbpbedup.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gopwncweg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gfqypqtbc.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gxsplnuwo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gklqppkzs.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gemgsejjr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/ggyskwnhk.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/guztcdntx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gzmyvtgsm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gskgjsoqa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gvbixdwzi.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gsabjymyq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gbyooquiu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gnftqytha.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gybgtqiuz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gceppmvpf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/ghgvprsup.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gvgbnqpmc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gsscvskuu.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gkkrgabrg.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gmtdulmcd.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gzzkwxoen.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gdlizxebo.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gnhziqpgu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gvkcqxful.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gakmfmdcz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gvdofuvok.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/giwlyuhfb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gkahjkbon.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gmbjcksce.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/glruixtcm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gdnbuwobp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtjxanfwn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gzeydqfnm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/giuqohlzl.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gbwgdslwy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gioiskvkm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gnamkxwdm.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gdtbfcicl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gdqwtftew.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/grbcmiour.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gnakmhwve.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gldibnbaa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gmecxjpbr.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/ghvviwivk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/grxehersp.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqilssele.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gkoygozbl.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gqizfpwdz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gzhzjtpnu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/ghudskdda.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/geqaqsxfm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gwmqbwita.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gzfnuiybr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkysxvpfb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gpimbgixw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsqqdlbxb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/guyhsmfav.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gnybmgqvs.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gmgjvlktd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gexwipoza.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/ghhtqefuw.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gcinwcwjw.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/glfwsqjmi.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gfrmtbgcq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gezbostya.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/grlkeencx.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/glubwaghz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gpvkibdyb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/glahxculw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gtopdolcj.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/guvmwwvdd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gjbsxvgpb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gnvqrlqkt.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gvdiobvbl.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gwwvzqqrm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/ghtzdxpwa.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/geqfhktgw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gorvbvlga.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gfoxuuqxy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxpjkyabe.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gcuomizkq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/ghtkbnvzi.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gsguesgce.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gmxmdykfp.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gbxmjvxmf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/geqodjtro.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gqmnruwud.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gswrluvcg.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gyxrxhyoh.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gchzitbwu.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gucdyidix.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/glcrkmrxq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gtiqkvnho.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gwuehkwqu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gbgolnmdq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gxsxrsdrz.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gfrgxuhai.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gauszyvyt.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gbwtxsdfk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gooqungpu.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gmqwsmlny.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gocfmxtmd.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gczuqdqjc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gantyhjmb.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/ghudyrkff.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/guvskuhim.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gukaeaspf.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/ggjgqfmbp.sHtML


<!-- 参考信息 -->