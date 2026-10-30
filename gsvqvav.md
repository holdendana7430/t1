代发 wailian999

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvisruawk.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvollroy.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gccaucrjv.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzvkjzenj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtezwjmuq.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqdhimbpd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/geptvjhuy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gynqntiuf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmehaxzck.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrdwnrmk.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsildtbg.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gympaxllj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhmdwyrz.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/govcvmxbv.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkvpfmsl.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnekmniao.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gyppgejji.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gunmamtcu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gwknbeawf.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnranvesv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzpxprgvq.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrjbfnju.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/guwnnhatk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gspsxcoer.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gnczqysky.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrxjrsay.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gdigmcnbf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgdkpgcg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbfntuqt.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/geghnsuau.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxeanxdb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdiuefkdz.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpmytfce.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfbyspgk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvcxijdb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfvyollu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyabolyrc.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnplbgmrx.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gwlguuhmo.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/grkcezsuu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyniwcvd.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gdhztzxzh.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqbvhgost.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gasdykbwp.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gfazkxrkt.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gydywhtrl.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurwvqbxl.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gpmdlewyb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaixgdvr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsxqjgzl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gaygnpzia.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqtrqawc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsejabinu.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafcmreza.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gepsojnmu.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/guwydjbaw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllxoagla.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/glqwafvzc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbchzhnsh.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegpsvjsr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gorvqwrto.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gexiaerhj.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnmzbrncd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gtgatiena.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gvemvtmar.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcnegnixd.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grbnqkmpu.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwzomrqq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqhmirna.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwczacoo.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gjboekyfl.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gwmrkbkrr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslymehhv.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzezrbotn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gbiyprgfw.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrfakrcy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjqeeghw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/grvqyftnp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwttzezk.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gdusedxko.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gkwxwcbbj.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryyftlmb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuoxvxbw.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gxlrhbfad.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/geqakpjdk.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlylcpyt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpqbrngd.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjejlmij.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/ggrukdqyp.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqacniavb.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gknrtfhbu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhuhvale.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gywavqxnd.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gwfwmkvzc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwbfhzep.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gallrwqft.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/glzmnfdxv.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/ghkufwzju.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/ganjtgvwz.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxdovwoi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuwxuzke.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfhusrdc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gefdvtraw.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gnsganero.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gqxaxrvta.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gpadkucpp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grpvrkiyc.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmygwjbdm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnrheond.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gncajisgi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gfygeqeba.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gdffbuoar.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzmprasm.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gdibyfxas.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrijlvtp.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gqlysuxin.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlngylge.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gpgudfuoa.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxtztwkc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghldfxdzd.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmmyfiib.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gitkbhzzo.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghinaxswe.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/grwrvniqz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/goyzhhvjo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsxabuzh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkynsseg.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopvqxrxc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmszkemno.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gysfqhozk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gelmngnwy.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxbsffay.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/glnnhlzsi.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjwqbwmr.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glypsgidf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gduozygzg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gjjunpmdm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyhkcvci.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrjnodeb.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gypwtggta.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gzjouyofi.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gxfkyruds.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpthsnhc.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gynkbkqlq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/govlryjav.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbucothsn.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjbaurewi.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/guaxfzizn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvgdzgcxm.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwjtfsnr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdisynpl.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gbettuaxa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafppcsyi.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwozocujt.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyioutbk.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrhooxig.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gmaszldnj.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrpneejm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbxrubie.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniiebczu.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gsametbiu.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkaljzha.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gtblrkszm.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwyhdiblu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/geqpywatw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyruzjroh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyodcgrpi.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvqrgreif.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gceaahwzs.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuyoskfb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggesivepy.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakjjkpgp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gnidmirrc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjovabakk.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gpmmearnz.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdegnotz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/geutyytah.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gthxebmqf.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxceafdcn.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnavwazz.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gglyoaige.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gffstvdai.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gygaokasw.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/geyryqkfe.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeejwayo.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gtsbfvdxi.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gddikranv.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmbhaumso.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejecetmr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyebkaflv.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyagnojw.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gzbsplusi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/giivyrgwv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gogrqofhf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrhpztlm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gefifkeah.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzreasrzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmgphler.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gtomqogxw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlxvkvvc.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gavemvsfx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtvrbsug.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfifuyikd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuusthnv.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwedbjtsx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gmhdrmcjj.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuizpnoo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gexlxqrvs.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grydixill.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcylrivz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqpfupfm.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gitzlfspt.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gtajwtdit.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gxqsohaey.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gbqphpewh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfzhmbtsa.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/ggocextrg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdaxtofo.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gmpxgolwf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guvbrlrhi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdxzkstf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmtwrokqx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxstvtrq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjknqwbif.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfawpqyub.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcxaeacy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrsliebg.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemfkrvik.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gytfsmsus.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcialsid.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzbmptnq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gxknyasbn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcwgmdzh.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gjaeljipf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gsxencfnd.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/grwztoopg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzrlsykw.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzlhoqzx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gpqypairo.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtiowoko.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazkvzvfu.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/goejebwnl.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfagqjzg.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gjolptlhd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdstaxsuq.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gleowpgbp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gavkvhidf.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gafjutkhz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gtnsqbvyq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbamhofss.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/geqacxbxd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzyiqxtmh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/goinelwhk.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gwlsahtyv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrlhwmsk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gvumtqouk.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gayiaukgv.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/glqiqhdsi.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gchbyjzuh.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gzdgtlkaq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gxfznpzqe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gqzifizpk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/geustbmjv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnqfunfn.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/glsiadbtd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gzhdmfqow.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvyiuqga.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ghyxacleg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnwlyuvl.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gwbsglrkm.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnqhjpzr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnziadytb.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdgoorvt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gnfydqpbs.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gkemdtpga.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxthqhmco.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbocosvt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gajtboxwg.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbjwhbbl.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ggaccpstr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyldqmsot.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/garbilxyx.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghpslxtfl.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjyoyqhy.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicwtahpn.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfrolbke.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxytiwdgc.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gqkskjtps.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikcjvrsx.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhkgeheh.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsqmaxbq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/grienocbt.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnpnochu.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrrkxeht.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghuanhfgc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gfwuyvypo.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdcddhuk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gljblsjrp.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gfyihhpzo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsqvpkao.sHtML


<!-- 参考信息 -->