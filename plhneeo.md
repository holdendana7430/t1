代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpjlcdqx.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbauisvi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfqzvekn.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gylzqwqdi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbycsinnh.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gilbwzqep.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/grtqkxlvp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gvezeifer.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gjholonzi.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gsmsochnq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gkchthdrw.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gowfmvhfs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gsljzikos.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkvwlaac.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcwwfxkf.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmugskiba.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbiblhyw.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhcozzoa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gepamtsgu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwluuwuhz.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gydmhjpdw.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhrehhmh.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gscawuijd.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/godlnzhsm.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gtrwxefuz.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcuvdaqj.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpconoigg.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gherazqjn.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgtmhyvz.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfezwwhqn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguscciis.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/grgqfqeql.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrbudvoe.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gapwhpqxu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gepybswif.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gifsqozqc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnqhyily.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkjurdnz.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grflmctrt.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/glaaxuhwd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/grqjwuhrq.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpborizi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmldbqjq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfczfeerm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gitpfclvz.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gqmknitaz.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqzqneugz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbwkzqov.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvawvgiq.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghlbmvqbv.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyqtoxsrh.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/ggzecwkny.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gicuvenkh.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/galxebhov.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/grubqlqff.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqzuilot.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gcmpufhku.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbznileq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/grrohdoww.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gqifgujid.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqjlmzfs.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gynxcagku.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkgoauzp.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gkkidssgp.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gdnfgsmzy.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcycacmjw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gldiaaica.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygkmjwih.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/glejygozk.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/grmzefdeu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gtnrtshnt.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gedpeeexc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gjnonlpgw.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrcjbvvc.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfmlqzbq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gytjyojjb.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/ggopsxjrz.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gepuipgri.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfculrlb.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/glvwjkfoh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gckphjptg.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmmnpzct.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gyekujicy.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gwisntobl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgcottly.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqbzaney.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsmntvbnn.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxumcsbkr.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhnoqkce.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gcfagrxgw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuzzhtcp.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggpdokeyh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gesevhuet.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyrrfpyy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gguqpqlst.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpjegwjc.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gjxcramsq.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlxebjpd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggusgwpfd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmybbdgvo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvgpqmuzm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcumnhlw.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gfjwjyoyf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbaboupxw.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrrwquxd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdclxekmt.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/getptwhuh.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gqzkdtbll.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghonqllmh.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gjmlddkyo.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/ggocmqxwa.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqnqhypu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvhaqnwp.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzxhgtge.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/giymbuwhx.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwavusiob.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/grtcyqkol.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gvpnycyjc.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gdtewcffd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvspsjvvi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhxybcaw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwebkvqo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gvbbidfry.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuoyhtqn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gviitrgen.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatzjjgxg.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjhoerbe.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/grdsawjmz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoconveg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/getkqjuwu.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gkxccalib.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/grhvjnsbx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdmmfthm.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ghodsulqt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvrwbcal.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gbbcecrhb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpmzpmrb.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/glzxngsga.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvclkurje.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyrxjmjk.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/guxkwribl.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/girtvdiym.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gmffqfrrq.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghprauytu.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/giczhvojt.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywzmyrbw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gatsxqpjx.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gldvhpvri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gwliypjzo.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ghejktwnj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjbalhss.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgcnbwvq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geejtddta.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/glqmutdte.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gysksefgc.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxmzkswb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveisukhh.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ggympuvsq.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gpuwbiyuo.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvudahkv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/goksoqebc.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/glbgakims.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzmsanob.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonmmgsdr.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxmgltze.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmahlmskq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmnwimje.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gacuzsuxo.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gcoszghux.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gcmjhcqtv.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gvushoead.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gslzxvvrf.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gymxuinou.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcgmevsq.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmjjrlpq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbthvzwd.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gujhdwdpr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqnhwwbmj.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gmpnmzbxs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoggibty.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gegtkezeq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyvvkuht.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqgoektp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcerdxex.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gbprvyoqo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgvnlxxs.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gswpktevo.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gxaxianwc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/giznanewh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/ginfbrstm.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/goxojlawd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbtkdzlit.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtnaegfll.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gebdinhag.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjefvgelj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gbsjdjivr.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthjxzyrz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvchpqfff.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/giqpgvpjz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgkjenjl.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gprnrymln.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdghllrv.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gojrmuhwu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guqtnplch.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/glqbftgqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfnyqkbc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcouxnouj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrydgvsu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gchxmrcje.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gquszibnn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gsttwbawm.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzyhlmmt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gegfsyraf.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ggfdvcknc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmrfqwmy.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/glfgwhbsn.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gktzyqtwu.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzofxjxt.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/grqedmdlv.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gtqaakieq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrfpvoql.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gidafegpk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gxnftrgcc.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/ghjlbogcz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqrtijoex.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gynnyjolb.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gszkmppjr.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrtwoyqt.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/guwlrzmhj.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gxxjuaksx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghezbojnk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvlegedu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gocmijsyl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gordeznvg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/giirohqsu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbkortvok.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gifdoknto.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdvlpsje.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gggpeczzn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gsotybnit.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gdgumimcv.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzdspihg.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadjxcyoj.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkqtcmta.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gmlwsvrwz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gwhlfbcjy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gdgcndmzd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfyjcezk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnbwstyi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfiehoeh.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gqohntnpr.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gyrbdyfgv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gajsjfkbp.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvefmjqb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gflczvznu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbcbbpfp.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjobqzwwj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/glhbxxdhx.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzdwclsq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/goqotrfke.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvhrkzri.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbdsoacz.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdmccsso.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gcejwzhov.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoygrqtg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdczjpflr.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkfywzjnw.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcvrtdsf.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gydiyntmm.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkvndnrx.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gobzcdltq.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwstrmzal.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gayctmwfg.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtfnrupp.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyzuulel.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjvlnpry.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gveexomqm.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gqyvmonuc.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gxhgmlolh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzogtsfuo.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghwjqnisj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/goqsznlro.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gmkctxivl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxogmcibf.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpviyynq.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gutcvtqyt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlnvhcjh.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomyzndns.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/grfvkrslg.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gbvaghftk.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gevgkfhyg.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkegwzpzk.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gbqvvucns.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqvkkmfk.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gcfjxphoj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gwycpnybx.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfzjnnbrn.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gazrgxmcs.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdwdfgzt.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfqpmdwp.sHtML


<!-- 参考信息 -->