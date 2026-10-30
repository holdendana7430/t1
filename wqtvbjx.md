代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitnaijph.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgmslapd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggisjlfau.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/geigtcdjp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gywzojsqi.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghenekkvo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlnigcmr.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gvwqoeqxt.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gwhsuwzpt.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gklrrqddc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gmeqzgnrw.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvbnxetu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gwghtkczt.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gbletyvtn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbtvftgw.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbwasfcz.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzrjinpxk.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejxyixxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcqrkrhx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gvcpfesna.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtpvmlyy.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/ggblnjpfq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gffeegrrn.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gyjxqqftq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gbiqwvxde.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gmnxoppem.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggehtazgs.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvlxumos.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkeiqulm.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjdlmehgk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gjlqoxpvv.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/glzitxnhu.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gjfjccpji.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvbfmhkq.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gsmplswko.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/giatzwsry.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzjoqoga.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbaejsxo.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxcazhjy.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzggjhxpy.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzrudtql.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gmbjoyjmr.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gsuetxssk.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkrzjisq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gungmpzqq.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gazfotgfj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/givdzppyi.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyxbkvird.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwbwpgqta.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/ganmzdozc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyaoolez.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnmmhliz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gdygsocbz.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpmajmzk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdawwnfi.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsjzvjny.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gybyjjnja.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpdbgchx.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpipvktp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/glycewsvg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/geyvfnssp.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcncoxjbb.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaifyelw.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gvxqikkkv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gnotesukr.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaueutgf.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/geoqshltz.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gnmxvlbxx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucyjezud.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grelojmcj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqxnjdcv.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gwflmpaum.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gkybldhxj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhdkfcwa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfairdqml.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcwackig.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gjzghulym.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggusgbjsu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gikmqpyla.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqvoymwh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gsegrjovo.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gnmjnntoo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzqsjcmo.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gxzhmhdtk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gapixnfow.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gezzabbim.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicxiatyz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkurefeh.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gorsngfyv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwqlvxrz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggxyuarpp.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmaproza.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpcneyiw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giykyjhlb.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gtftdnqfj.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gdkolvqqp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/geznworta.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspuwmkoy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwhrdkpwq.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/grhxgjpic.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gjghscofc.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gbqsngmpj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdodchvti.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcioxebog.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/guvzirnsi.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gicifehmn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrqwwjdk.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/garrayaxr.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/givjjpkid.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/guhivtmvu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrzzagfv.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvroofoo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/grljkveze.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgspgkyc.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gtawqytdx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfgpahbes.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomydsjvm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnwswmarh.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmypxbyiz.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqsdhdle.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohxegumj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gfsbwvgmo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/grotvmjaw.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gtlcidwdh.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcxtnoxh.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymkeuohm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkixqgha.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gwuztvgqn.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfghwyzzr.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grzqqafxp.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ghpasszkf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvltrjvk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/glmxtacri.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmggayil.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gexyxhcta.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gfsgrdlux.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gskrhktyd.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpetrzgu.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqtlicaq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnkajpnh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbmhneqo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiobjqqk.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyntassq.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhqpefkf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gcobbjabx.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gcjhyyprn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gkfkalmbb.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gexopmqpn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gcmbifqso.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpuwxfes.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbomxwwef.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gaasuhsol.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gtzpwdyss.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gghdivvac.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gokcsvofo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpjbursc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsosxsqd.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohqtfswg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtxekmfr.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gxigvwzuu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gelzfknhx.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/goiilpuxg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gmejwbevs.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtsktfoh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsskaehhn.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gshjgdnom.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlklhuxi.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/guhydbqai.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gnwnoecmp.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvmjnnmj.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/geqglbuho.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/grobtnizz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gjlhckbja.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gbkovjsny.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ghqvtjfiz.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gadjvmqde.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gysyleqrc.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gusgxvnen.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gqmtdsrbg.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvwujooh.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gumrtjkgb.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/ggbtffewu.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkppscrm.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlffoyxv.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbirzgbv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqjreaqeg.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gipfnisly.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmmqtgib.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gtjbxdenl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gnmrxiava.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlouoggj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfugpitz.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ggbgjwmfu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnrsyvrp.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskoppkmx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqafsbfzc.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gzbxmgvan.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdarlymdq.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgpjttiw.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtyvlhgb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gekejackx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/glilqzfih.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepsyytyl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gpmonwazv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjioyceo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtamhhpup.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheowcpbb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gnckfbxnx.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gxmupcffj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqjuhjae.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkwzfgeb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlumgtgw.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gfvxcijxb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfacdytel.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrnoieow.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjxhrvtd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gbrasosjf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwitwwosz.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvvdwuux.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gffxypcer.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gyyotoded.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhyisebx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gbqnbgxtv.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwpqkshvf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpupmpra.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqoadund.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/griilikyl.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gfjazowvv.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grvgdzkmg.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gkyhkrmgp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkytliphv.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/ggzehacsk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grqifzwvx.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gcmkqptal.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrpnetvf.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/grrecbenv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/givzuozkp.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqxfsmyu.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gbonmcewg.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gotlribgk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gqtuqtrct.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gdeitkfbo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/giiwkecma.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gvqdvulwb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gbginyeef.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurkvhepp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gdgaawwbh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guvhmkbog.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbtjdvtf.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/glamhzkyd.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfriekczm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gcykkuctz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxglmdpss.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/goaiwanws.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/geocveuhu.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gxlxbvmie.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gjcefdrqm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gdftcuinc.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjyhhvcc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypddrtxa.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gfghnazwj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gsfapqcrs.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gklmqngnr.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrzcyjzk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecapbadv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gefllmxrs.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpduzwgud.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gsqotzwyx.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gwuiqbfkp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/ghczgjxsv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gcofvzbaw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gotnjqjvy.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/ghgcvaqyx.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzvoxlygf.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqlskwoxn.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpyxdpxi.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmauwfgx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gogfsjmwr.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfkfroek.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gvrocvkso.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gisfyifgl.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gknpdhzen.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gjvbzhggl.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gajdauajt.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuzttqgn.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsiokkng.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgbvkcxr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtjoguhg.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/guygjjuvo.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gxxgzakyk.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gwgoavngp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjribbpqv.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzlcujgs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gzhlhuwul.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gcglyywtj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvafvzkat.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gzhgrtidg.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/geadvcjnc.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gapingxey.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gppqjokix.sHtML


<!-- 参考信息 -->