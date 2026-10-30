代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaiuftxe.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhgfusbt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gunqyvmwy.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdssabox.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwnzycgs.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxhytagv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gylhliaxv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/glhljlubl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gcnkucsba.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnutzcwn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxapauyjt.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoqafpio.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gufnlteih.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstywriwy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gttdpjhsk.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnrcrlli.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxhkxvatn.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohywbqem.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghunjksdz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfejblkwb.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gwnzygnpx.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhwcnuhj.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/guwfsyfqm.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqkzsdaj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpumtotl.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhwvpkbi.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghqzjynti.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gufdzagvy.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gmcqehhxb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycwnqoog.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpnjkccl.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/guivmvvvz.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfryzokx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gkalmwnuz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gmjxgnasb.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grmhbkvsq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtdafcuyn.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfhvuimw.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gepbhvpyi.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfzsgwgb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gfltblvtn.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycpxdneh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/geiqjzhpp.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjnnuphp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gcboyvper.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gvhgxlpis.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmcfghmr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgnzpzmc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gryvfprvj.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggornetbd.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqtargmia.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gozsdtaha.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gvcornpri.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjazkmig.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gvxirznqa.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjticuwyu.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gfjthfbup.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gldcnause.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrgmotyy.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gjocdzxrs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxizqxdy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/glwjlutcq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgmawlkw.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/ghpolodwi.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gmkblffda.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guvqjblvd.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxgygybm.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gyauvpcxl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoevtaru.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfazwvcqw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpafuyfkw.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsihbyyh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gqsidnvwz.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnfoktmx.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gremvoodi.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gcthjxejl.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gtjlwtqjt.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gltlsbkha.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gklixksbs.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gjcwufvbg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdhyaust.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gtswjbujz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gczdunfza.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glntjpbbv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwdwnizk.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcgsleti.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxvwhelu.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbhyomze.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gwqildssa.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gtqddwajb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwnvkgyy.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtzomuqbm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioivqzqo.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiujaxmi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/guqfeeals.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gnvbgiqrf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpangvrer.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gatowlymb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsgvjirmf.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gntfcovdd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvpbkehbq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/grfymzxjy.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gsnrkogdh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjurtpji.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmehcosv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdxbiofus.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsjhgjxg.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gyfftyqon.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqetfhjd.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrszmhzt.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcqpqkrq.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gvoqiikjz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoobrnmk.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvtauaqf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnxldpqx.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/goyplwxze.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzeybtjq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnjlnfis.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpyisfnx.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvtahmno.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwuoctja.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpnklvxv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggesybdzk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/ghwozsexs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxlijhxm.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgkrhyvv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gsbpnyhux.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gflnddynl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxpymmtd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrnxpdln.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/grsyxtcgm.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyqwbmsq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatmmebkz.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjdskrhn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/goxlkehij.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoeupuvd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbepruxg.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrwmmizq.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ghdleqxmz.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/goanbxwkv.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gclidiukm.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdbuyuba.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gkrcptkdl.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwtzvshhz.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gbigxwsvb.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvhnqsqv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfaotgft.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gyxjfcnrd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwmkcunw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumkjfcjd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgzyjgiw.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiofwtis.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfdaesue.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gtjkprcxu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdlqevru.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/grpgzferd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmthdgao.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gdvyruimp.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gytvhiqis.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gfdzisauf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghriukdxa.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxsmyipj.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gbqvyefbs.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdpuxfmi.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyswvjdre.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/glwsacugp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gdjbemjmp.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gyoemvkat.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gdwsligrj.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhvyklpt.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzijuswy.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/giuwsmjkc.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpurgoex.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcjwfhoyf.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gilrfuqnb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghudbdwnp.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzyrqfkr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gddvehrzz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguxnwibh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbliwatvo.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/ghacswlhg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscalcqdo.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/ghnbegomp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbzcjwntx.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gvcnysknp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqosynju.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gicesfkee.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyiaegwq.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvmkxomma.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gcjavvsdq.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdmppgiz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwznhjsm.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gptqbtfuj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmjnulif.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgvplvqp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/glclqgygm.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqhbgqpp.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgmhyllx.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gjmrcqlnd.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giyptndjt.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnzbctvl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxlodqpe.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/grrvybvwu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjlviuvla.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggcibpdzl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfdpfkvx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goknptvfn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcswgbysj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyacclljq.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/grmtyarrx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gdfcmacat.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwzqxicw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gxwetbpov.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhmlzdlc.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgukmqlu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjsjeooc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggkfnizoh.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/giiwxclwh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gboalnkyl.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gxmoknfsd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glilyvtbq.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gwxgfcrda.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gwjopernb.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxxlghrb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjmodify.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gkzbcbzoj.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcywljppr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpcvrdqq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcjbiitf.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/grwirhkir.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/geaesizxh.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsldwquh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/giwjnuaui.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzzhmpzi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhkmeyjp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gacucfxti.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlogrsgo.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqpkubeq.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gztwvhcgy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gqktrpmzg.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gaftsmplv.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqwuujge.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gksmpkeln.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxwbziry.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gautislun.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gkszovkiy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/geyxvxdyu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/geqaokmmq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzdeyslw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gokqqqbos.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzycyecw.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoolwbrp.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxrqslrrs.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/glnlgsjsd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gcmifbtsn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gdlmwfzkb.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsoaoowq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqukqpubc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqhgcwfv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grxiwkemv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmhcsmhd.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdcpwnfx.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfvrrbxw.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gfdjxnmra.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gxdtxzgrx.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gpkticaqs.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvytlgbco.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdhhkqrjr.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgtumujm.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbtpdpxym.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gjawucnxe.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomswpcul.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/grnmzocfc.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcltwbasb.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxrvjwej.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjifxjjr.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjakesexc.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuugrfxt.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoxloghq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/grrilzoku.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmxfopzk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/govpduegv.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtgrhhqz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndhfkivf.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrsaxfpj.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvupxonxn.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlsgzamo.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gobddepwh.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gubfxeltx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gibmrhjnt.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehpzwoiy.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjsibdou.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gljhhaqst.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/ghljkmryq.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsotkajy.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmswtqaep.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwndjrktv.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgphgpbr.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqousdeot.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gerxhtdba.sHtML


<!-- 参考信息 -->