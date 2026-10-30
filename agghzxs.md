代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/goguxymct.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gopttjnqc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/giztlqjry.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/grpmlvknl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwmxwtxz.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmavvoqvh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpavcfdld.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gqsyklurw.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/genkpwprb.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gzgnucail.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdqllgtp.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyvccozj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghcpxbkvz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdenaiant.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnyosifp.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggibzumpg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gflvffimx.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/grlqrhpzg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnsnpauvp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gposviqvq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsfpflxu.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gvqlmpegz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdknngpvx.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/ggzdgdwof.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gzyxqsexe.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdttnxce.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlpukkvn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfrnqqlg.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gufmtvbmn.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/geyxxjejo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gbifgignb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gltvdlwnp.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfmsklmv.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gllcmrkiu.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpkrsofh.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzyuhqxg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpihwxojd.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwytkefw.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmzqarvl.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbmwenit.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvplqecu.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwndhqwrn.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gnpfrrtrw.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkjpqdfn.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gngwtmnto.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gnvqmcrzw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjkjyyoa.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gddpjzbhs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpznnvgam.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqdvhjof.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfntkjjof.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuwsbfak.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/grwtqbxbv.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gcufuglex.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glrlebmzm.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/grenacmpw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/glokkqxnf.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzwsrfin.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goesonqih.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvysxfhhx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/guiqyzqnt.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpxkqxgt.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glibawydv.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ghvvunzdx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/govtelqkd.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdthnuxl.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbjthtwh.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/ggivneuwm.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxxvrqmb.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibmnpfuw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlkcayrx.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/grblxpulk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaknksplw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszxbmyse.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnsrnldy.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gocmuwojx.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gsrasuchv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdasjegp.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gpyqnzbyg.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomnkkdbo.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gnlkogxxl.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwkojcga.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwedfckl.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gitljpant.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbqrbrpo.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgacfkwn.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwxppklv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkwafddh.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/goikbytxr.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpqjkltf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gptleuuev.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/grxfkgldl.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkdkdbjz.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/guapkbbsq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gxwiqimsi.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gelodoxhy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/grkqmppsy.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnewfefl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/giicaslke.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpvmxrcq.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gkqeyxxss.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gqbmnkijz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpntuwgof.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/giighlali.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gkvakhqiv.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghxzgutjo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gfzizfuch.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfbejnlr.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/glvpqlkuk.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gqarcwpfj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/glvxinvhe.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaapfqpbm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvihxiitx.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcecwbmgn.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewfaqqms.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggzqngfks.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gsesqgonw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizkzzidp.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxvwxlbvf.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzehstqh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzvrfcbi.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/ggzxwtsor.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gunktxzwv.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gwlcwcvrr.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gauffbreq.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gciiezetj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/glmgywwub.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjqbgpla.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqassrguq.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzssppoaq.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxuzogov.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwzgbnsx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gisojwkky.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gssxmmnoj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpixxfhg.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gymmtptib.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzndpxmv.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/glvvnbidu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgaafzts.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmtzvkwzx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/glzcivrrn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqvixzjp.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvaykimi.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gksrehmxk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gceivujxx.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiqxaqco.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuijtejh.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttllgnfv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gfndjptja.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/goftxocyr.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtgwlexd.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/ggcyhrwml.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gonwvojlc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyznwxib.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gltwufzxg.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmvptbmp.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gzpxyvkxc.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gyentxosn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/grqfqzdyl.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqvjmcbj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkogywylj.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gmpqbmlij.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/guruyscsb.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpgldecb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnouejix.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ggzsuzgah.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gpmxrzkha.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gjghizcei.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gtdmzghlh.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/givzzwmnt.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gmcvkjwap.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrweokku.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyncogpk.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvupyupi.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gqckhebvp.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giqottmqp.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gwspocqoq.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrmjfmgv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhzcgvng.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakrxsbaj.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdwggvsp.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/glebukdsf.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gensncdfd.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvknokvik.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/grvglmjfb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiaeoluk.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grkoaebum.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gxaobnfxv.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gniucvfqh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ghiltewyh.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlfohdav.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsndjoxp.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gydnlakvr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthnoljta.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/goeqnqren.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvunbdlpv.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzfusjak.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrjmjhie.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gdosofwco.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnizwnhik.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjugujdh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gkxugwddc.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gxgfptxzs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvmyobdl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfpeoxve.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gaodpogeo.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydbgfgst.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/grtyluapu.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gasjjigef.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/ghbzvxarn.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbazsvquz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuiegqal.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlrsqqpu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gvgxvlrjj.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrfmpfle.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzkgveenv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjlqhjuk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuuovooi.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxhsuhuo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuyijoud.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gxebpupie.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwiunudr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggthmhfht.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzrrsltc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdjbwxkj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gymfpdduq.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gqksbjxpc.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gvqgqrkxq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyjgcmbrx.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhvywjgs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjfmsifa.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrwwtvqn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gkymbucro.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gahkygryy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gembgwspd.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplucsyzf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxzehdfa.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdauecdcp.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjrxbejw.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihgefbjg.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gzyvirirl.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpbssvwc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtcziilx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyguwqbe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmompqoty.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxpvtksxy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/geoqfotow.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghakqlqmg.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhgojrje.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzvronmv.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/goduqoxvf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvkcvmvh.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/ghnqmigla.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gksslogfm.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gitljghyj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzqtnccf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gryztizwr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiqboqgz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/ggrsmkgfx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqdeomfd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gyponaatc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmwrhnfi.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkaojbcb.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqedlrnfn.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glaoxhwtw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwisvfxs.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwculngs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gsozarblk.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/goedfdocy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqprpxkv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gieuxysoe.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmcqyfsvx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gjuxbykvz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvbwsonwj.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/grwgxeldf.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gegtjhlps.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gtupvreko.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpptlsplh.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grmpwfivg.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/glqlzmbav.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gzmydyiqt.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszikenbr.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcbjeifv.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/goxqarzgg.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbkfqzti.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuswvgth.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gmlksqtgk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzgdeaxw.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gafrotrcd.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gylehwuxo.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guewaddgp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhjvsgid.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacktbxwa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuuxptyz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadcgrkte.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsgvmffx.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjeazobk.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnvdnnyf.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtboxpym.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpnwbjvy.sHtML


<!-- 参考信息 -->