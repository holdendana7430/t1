代发 wailian999

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjblbljdx.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gcwtchzfo.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/ghhsdtfio.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrpjhgxe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gubefjnxs.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/geljdrsro.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfdyqbgr.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqlpgpyj.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxzuoqnj.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gupykvcuc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdboezcf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynljxiot.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuwpisgb.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhekvhop.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gclasxcbu.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukcauphk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkejbiobo.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgjumsrd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gkccdthsu.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaupchsh.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnakidok.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gapaupclf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqgqsmzp.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhyhpuzv.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gxckikzlk.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gplxgyuck.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzplnezv.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/ghzjpuwws.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gmgoiwowe.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gslavstaw.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpuxyzyg.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvaobdjwu.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gewxcsrak.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gryndxzwx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypeirvet.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkcppleh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfffavkj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdoeesip.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpigaagc.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcyijizh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhzxopkx.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gjllnzlrc.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjchxdcuh.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtrjgvdh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gjikbxlvk.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/goxgegnxg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/govfcxash.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxtdxmmh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gntttcybu.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gmjsecitl.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxglbfvyk.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gppypqief.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvajdyvgg.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaagbdhk.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwoldvbcm.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ghxodlwmx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiaqonku.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcemlnem.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtetlcqa.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaeqstpe.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnzsohwy.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gekwrauxv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/grppsvjcd.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxdjaecj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsxqfkdr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazosmsqy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggirqwsgz.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxutliip.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gdtcloscn.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gphqccnvb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwvnvyvd.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gyoqwtcsj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gxpdptdfm.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtqpubgd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdcfrquh.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdptmrtuz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjlgvkzv.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxoruahg.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbvebjcr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsdmipvc.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghofzsg.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gscfaxwsy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwzdvdot.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/glvbintmx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrigywym.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqkdefmu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmoupwdl.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gphxqebpo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhgakaif.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/glrcrjajm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybqznqot.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gqfrprxpf.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gocmgbhsu.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gdacnyqnc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggfqchjos.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxipuqfbn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gnqivksyn.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpiebyqcr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gpchqvrey.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gplvuwzwy.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gkjrexwcj.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gqohnbosp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhqjwhzl.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gqupcuzhc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glgmbxsdj.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gxuvingir.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gcflhpmdj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzujkdqj.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfnqivsy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbyuzeene.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckyxggua.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtbucfzc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grafhjfoj.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnsrrpykn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gecmpchhm.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeogvjgy.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/goxkkvkgi.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gufrzzxia.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gzumxvtks.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkabnqqkn.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydwkmmms.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gkjghvgcp.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjvvvmzk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gindigcej.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtaprcwe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/guvjfonvo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gbqnrsopz.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/geftdliba.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gwckwmawg.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gjwfyfoil.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gqbiqifrw.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjvmzenhu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gslwegvxf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gfkwxrril.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsscolsi.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbdgtesq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/girbdvjum.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gnjrpqpho.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeerletf.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnwfvray.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexawykiz.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gglmhshwu.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfeznbxm.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsuhcyob.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvvgveww.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsjtismi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gwrgtnvbm.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtnlmrfs.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepoeidnm.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gscxcumgp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgizkvct.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gwaadvdpe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbvgxiln.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gszzcxtxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgmvduzu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorldzmdv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqalsnpj.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkirmtqgz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmkoxoik.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/goysfimwq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxizeamrx.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmhcrdqzz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnxhrqin.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkctljqmp.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gilafxnob.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gkzkuuomv.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gratwmdli.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwrvvdcj.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/godkuekrh.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmklppzmh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gahfavfal.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gseofutvz.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/giznmqxxl.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gtuydrgqg.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmlhvjyz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknyupyhq.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gahthwoff.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giixrrdof.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gejikmrmh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqudpzkd.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gqsotgjqr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbklquvn.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqpewvyt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyqsiznh.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gosgxpgcu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuobqsda.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvemqkbbh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfjdrakr.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gmpruwwak.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqgnrdqnf.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqqasnxd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gnnadvprt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gptefstkq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gyqgxcpii.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gahggnavk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gesakdqxw.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/grhtgycpj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfzaxrgu.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grabsjvav.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcstwfzgn.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gdomlmbkz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnxrunhl.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/ggrgroefw.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsszkamk.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxtcoaib.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgvreylw.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gjvxxgfuh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgyetoix.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfkgvuvy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gotuasytb.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvbkdqxkl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapigqjkg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/giatfkdyy.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gaggkvtgo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gljngohqu.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gbkkskahn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gnbrnndss.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gyburltkl.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gklqoxidh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnranyib.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghulhpynf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehncmnmf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/galxivwms.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/grqldduwt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gptcbwjcg.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/ginurjxyg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdqboopi.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkxwdceh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjcbmnwrt.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxrnxnzo.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdclhrbfu.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvgwdzes.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmellyum.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gmcdrzzyn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpgkksod.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gscfaqobr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gheslyhom.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/golvraqef.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoxwjepx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwsnaupv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwnrxnpiv.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gjfuknepv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfywrdmhh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gfqbbcjxu.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/grsqluwgz.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gtykcgftt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkowuiul.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/grbehiryx.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbipnbne.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gjdfnbivs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gadcpovog.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcrzctquy.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gdkbzpzar.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynrxnpwg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaujequv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gixpayhdx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeqgsdbu.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gstmfupka.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqmhivjay.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gkqnjgvzi.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gentluhdg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswktrwhb.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gzykgkpyy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gjqtimuka.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gubfsehsa.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcafsoswo.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/givvznceb.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gbytddhjq.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/ghterfvgb.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxqqpoyf.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gitinlayy.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gqzxxagmw.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyqbrafd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtvxjhyc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloualxte.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gbskfrfrw.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/geykoiorw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggstlifgb.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gzozmqjsr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gvvuugdvf.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwfrosea.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gxcfceotb.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqmaytde.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gqddsmkgs.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqhbddcfa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gqtwgtfkl.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/guopfrrdh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvplveczg.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gwcsioohn.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gpeibngay.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gnwfiigbl.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjdgzxdg.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/glgwxwhng.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjczkutst.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gcophrgju.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpwckjrf.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/guaejbapr.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gjbcgyezd.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlsoercd.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/glnbzbtxd.sHtML


<!-- 参考信息 -->