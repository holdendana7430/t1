代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/ghfepseqs.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/grutwyasi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gsewgarhk.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gngcbdcbr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gyshphkxe.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/grguuavtn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gwnxswylq.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gzafkjqwe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gjtogegcs.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gyoeaaoer.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gxamvnhiv.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/ggertsbsf.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/glogfvxln.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/guqiqkhip.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gxigspkxn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gdbxpfsbg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gwqjtizdu.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gnvdgfawo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gakhcdspx.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/ggkbtwtmp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/glysmavca.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/ghkpcdbjm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gboswanmd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gnmopobnh.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/ggvvgylus.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gisopruns.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gphkonvob.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gdbvnbzlv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gknigihmm.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gzdojztgp.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/goouphnbh.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gakvfpqfp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gepdbwrfh.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gpbqkuuel.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gypkgmwiy.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gghsbrxdl.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/grrdusupg.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gmqqsvuhy.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gwqlwodbz.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/ghcgcbfys.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gbscrdkon.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gkpjeypwx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/glgblmrbz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggintnfja.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gobyivqrp.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gxybvpthf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gxzosaoyc.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gmsvcuqoj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gekpwsrgg.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gkadzzbah.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/ghqmjhhvu.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/grabnlmrp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/ghqxcuegi.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/govgbkvkp.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gkcmhukcz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gaakcwfnm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gfiiypkil.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gfrjhghub.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/glnlwkeir.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/giwvusrce.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gcbdkpxxy.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/ggkxyxrod.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gycnqvwtt.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gfzqddvpl.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gschrwzaz.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gzvzjkqsd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gcruxuqkc.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gmhdbjlhq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gknvghzec.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/ghtgqqdzj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gviipygxg.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gasfcdtso.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gfbwgfxai.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gqgqujcza.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gjpvtozzw.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gsgwjaklx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/grmrrfdnz.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gehvpopmd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gptpobmah.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gctuffemv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gkbymvkld.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gmmftbrce.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gjrgjwtjt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gscivjyiz.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gzymxxkgm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/goixeffhh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/grdomdtfs.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gbgsglldc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gwnsnwwqc.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gywyxkbig.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/ggcktgfrl.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gisnhbzsg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gxsgspzjv.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gevjjqvpg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/giwwhgklo.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gxzvtzfqf.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gdxrrmbtr.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gcmnxhkde.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/ggekxjxpr.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gdrzpxcei.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/glkascstw.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gulxzmwnn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/groqipuuj.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gzhcuiovl.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gqhqnfnva.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gthbeuysy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gxckporzn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gxmljiilj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gqbaqoxgo.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gnpfzfcgo.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gkwlmkkup.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqhflmikw.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gzztohnfj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmhibnjnw.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gexmpkpug.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gmdeshmgm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gvlkmlibd.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gxgdqfoqy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/guqwyasuq.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gulvwnyzg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gseawlxdc.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gbsynyjmq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gpmxcfpjw.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/ghqhxublh.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gyoeluvoj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gcppttvfc.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gpaemibna.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gvkknzlzs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/ggnaiztsg.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gcijuhzus.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gpuhxlgvy.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gakrpvoef.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gswytbxhc.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/ggzkyorks.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gjrqvqvwl.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gbexuywua.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gfzbxtnbo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gmlsdvoyf.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gvvogilfi.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gbyetkuey.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gvzcjtqdw.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/grmwjafrb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gmixbwpin.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gvioudhzk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gnkgweblx.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gtzobjabe.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gqdizkzdv.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gwguitepd.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gnoieicml.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gpkphfpee.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/grghsdssu.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/ghmwektqt.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gmrtsobot.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gfzlpwjhs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gxufdkfbk.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gidvfuvgd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gferqfctv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gqheellbv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gthonrwyy.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gdhbqnayr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gzjjooivx.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/glqckikxc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/grghjhuvl.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gahqdyync.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gkvewonlv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gowrnbfyl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gcqmggyii.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gwyomktkr.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/ghpsqymgt.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gkjssodcw.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gsfglhato.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gscelydio.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/glxytinaw.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/guimgvtzh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gkxxoditf.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gstdkzztm.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gqruegfiq.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gmuihxoic.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gurldmpzt.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gletmqtnq.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gjvnftqtn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gfkwaypus.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/ghqnijwye.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gquovskpj.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/glvakomno.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gdfnmwajv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gnrgqhtcb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/ghxvzzovy.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gleqdznkl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbvpsofny.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gfcfejwnp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gzfzgmwlp.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gvchesbrc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gdqrqlxnc.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gkivqfsmb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gzbexjmqz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gcemrrmdk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gtldloujz.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/govvsyddr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggtkbhsnh.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gcxdetcfv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gezywjrgo.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvsulpxzk.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gxpqkwmbi.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/glyunlrhe.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gwayajipi.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gxkbwdhac.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gqeqplxkp.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gnzlookmo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxmdwhapp.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gowxckguk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gegfrlegl.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gpsyeeluf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gayfeytgk.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ggpmzccyp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gdovbkewb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gervabdks.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gzmtckaul.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gaatzinui.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gvrztwxtk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxgjjvirp.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/guwvbwzlw.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gkzctxsja.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gvplhicmv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/glhylohnb.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gegcprtka.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gmrnjbncp.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/grerwgjag.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/grftxgygt.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gytzxaqwy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gxxqfkwme.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gtmfyddwp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/grzndfowy.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gcnrmmuvt.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gpedefhpj.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gorhjwcbu.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gmhhgeohv.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gmrsrdpue.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gmiyixwdz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gsjahdlfv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/guffntwvh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghflpmbum.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/ghkwhluyk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gehqmptjo.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gbpbllhia.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ggnksneml.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gkbefbdkq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gpwipkeqp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gguframiw.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gkxloiupb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gulxejoju.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/glhmicpha.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gjbfyfdvt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gpbpzwimx.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gqtaujaag.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtpinvoac.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/guhoesbuh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gbdfldmvh.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gcnxrdqmx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/glzugpkin.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gpuskcmcz.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gmxmrluew.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gpwelaqch.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gmrjfqzwn.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gnvkjsvwq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gbvocmzuv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gwcrgorsx.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gburnhzpv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gvhpajeia.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gsqdwuqbu.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gnfcahetd.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gqzevsjyl.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gdycdifmk.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/ggnfdfizq.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glmxwgwdz.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxnmjssce.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gzcpjupdc.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gghvlyokk.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gepokocrl.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gigosnfoa.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gwzjcdayu.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gqnfbrftj.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gwgpigoot.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gpdpinpgc.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gxqbqtmdk.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/glgoqnqtw.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/giqffrzjc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gyfpojgio.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/ghbqhoagr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gfuehpdbn.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gjrzjznmq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gptxtiwih.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gslkrhvzh.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gfujspich.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/grgeyxsqh.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gurciffaw.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gyyumdjhs.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gtgcufpre.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gbbnxstcg.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gzrhdojfl.sHtML


<!-- 参考信息 -->