代发 wailian999

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkkvyuzp.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/goohbftwv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwixxuugi.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqvzwpwnz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtekpbnqb.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/grfmhoxol.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gxsfgpdfk.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtypdpklr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gceciarqi.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gtfuyphfp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnkalkhl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbyfhcjj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gkluqnwbg.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdxspbuc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gddbucmrs.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gqkmtxqpa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfyysgng.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfgevwjm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gvtqnlksk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsojnbuc.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwoqneef.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gnxxcisje.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gurxbexjf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbmswkyo.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gbsehabmp.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzfjasjzf.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqujttri.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ggbwlhrgb.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gebzbzbso.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/guchpixjo.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gaebpvbfc.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzwipghw.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/grmmmpcjl.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gjrybopra.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ggatsneba.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/grapslmze.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gwjqphnvb.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gjoosvkgo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/giorrtxwb.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gggccoseb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gytfdgllm.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gvjbswoxk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbstqbmk.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkvypfna.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gallirllg.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnxvcoxkz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpupedsyd.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gzleqzfpa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/glbjaulon.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gcyedatao.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvzlihyul.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvejzpnmc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagfutqus.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gikhhzclv.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkcvbpysi.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gusvuylbq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gwjvjdlin.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmhyieqq.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/guqbnfcei.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gcszwotqq.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gytkxeelx.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjgcnecz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/geliaqest.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnxnrdcg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieulideo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaezbqin.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gfqlewqiu.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfdkywsu.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/grfjleewd.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsnwtxfif.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gdqpaeujh.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxcihyoe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzovyfby.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfffwdcm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcttwdccu.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofpipcue.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/grzumpjmt.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsvkijmj.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gnufumred.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknusggiq.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gdagnpfjz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrwjisrq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrwqtqxy.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gyufbkrgf.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gipvpdcok.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gchhqrjbh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gvcztgtpf.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/grukpuhkw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gmkfbgsjx.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gieovrvic.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grzjiiflj.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgaptzke.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gyihrzmyl.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gwngieihu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghjdrssey.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgjbnihd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqeaopcb.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gualhkmhc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gjdohoaei.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhlveoqb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadjrxidp.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbgtesqo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grfvodcib.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gxiyzpbti.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvbkxzkh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gacfsxdhx.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjnldjtk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutzourvx.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gkvtqluvq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/graxdufhc.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzpxyzjw.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gapdiubog.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/guewghfdo.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnddccvae.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnprwhlbn.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdswslbz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfdbzsla.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsdqoryo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzidctcx.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/grvevrulj.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrvjehfq.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/goekyimea.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/ghnxczuuw.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gocgcylqy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzehcxcrv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuzzxymk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gejsnhufb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwclpljk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gmyrmsywe.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gdzyrzhnz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmubocexo.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrbpwwgv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gpokjblaj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvbqjmhlk.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbhdrflh.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzhdnommf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gfgknjxwz.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gopaxgzis.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gerpdzlox.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvpywwst.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gggpadvno.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmybmciad.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtqagjoc.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdrhreug.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtagjckvs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbklhyazo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqhncwoj.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcinijxb.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnntnxvp.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluovtini.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewfmjcau.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gziuwcdbm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gtytnnlut.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/giwnctnew.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gyanexmge.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gbsctckzm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gflfkmqxx.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrnczjsw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gijwjrenv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcjzrczk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeaqvhig.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gosqrdgsl.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/giqprqcld.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gqmewfsev.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gppxtwgbo.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/guaahybdt.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfocgrbxw.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdwexezh.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghklnxwas.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvygzbabj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmenujco.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnfobkty.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gkgozxpdh.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsexlnyz.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gvgsoiems.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjogzcxcz.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gckzllznq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gifkewylh.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glglwykoi.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqmtzwol.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/golzneblv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gylettzjk.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gviqrrydu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gylfthgpi.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gbqilfmng.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfmgwzyy.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gyquvljot.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ggxfitbfj.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihlenqqc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebiwsorn.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gacjseyuq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gtekiwsek.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/goggdqxuh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/glokbkfdp.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gpqysgrpg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpetqzjl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzsjxyen.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gviazbgdo.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyjagfsvd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtiunelm.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/giarlgodf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/govllwsnd.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaelkcgdr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjtxqoet.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsfswomt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/ghalmgvrd.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoazjinx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqnufiwg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzyrfevk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdplqiins.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwcmxhpba.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpryxngl.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gojeddelk.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxkzmhtj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gitzvmbgq.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpafkmxw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyikalzk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppiuktnt.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/geyhbyojv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gfmkhmkrj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyvxsozv.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gazgxpywe.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpgbtlro.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gtozoujwj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmijqpzva.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gkdoesfax.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gfrrgnpow.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gzkqcjbai.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhjuyjmf.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdogkxwml.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gzelqvuae.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjdpbkyy.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gehhccyor.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdjvccfu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gwcwtcjtw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gkosxyrsi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ghbotplsv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grikzbjrj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/giuyebxyj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjlskaebb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjgtbzdl.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gmutmzxwq.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gszdaaiwd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gkopxvsdn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gteftdfky.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdydudrpi.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/giluqtxlk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshoanmze.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ghuunxjqn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiavvdvn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsgidoqz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuzpmdlm.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gnkudnxqs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkwqaybs.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gszormdwv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjneoopco.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuwzcdlo.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gpemgxpnh.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxtibpidc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeeaxjnx.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyicpusz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gjrcsxgmq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gavajhyfs.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gozctckyp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/grmtczloz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gydxafciq.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gynkwnokn.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfoedrec.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gxozldcen.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmmfebci.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggchmalyo.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/goljcrnum.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmsszegc.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grzliyzpb.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbopuqnnc.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlbzelci.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gxojkisio.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/genkletot.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/guttqvaih.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlxnfhzt.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/grpwedzlz.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gwnqmhjkm.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/grqvflspr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdombvjvf.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gofohjupb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxeqnkfs.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/ganjjoyuq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxlqnock.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gijxcboda.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzofzmai.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gcaruqajr.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsptmickj.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfjxgvoj.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnlrszvg.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikniinsn.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gngbkamgg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwlaczgt.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpexmxng.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfnltmgr.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gkpnwlvxv.sHtML


<!-- 参考信息 -->