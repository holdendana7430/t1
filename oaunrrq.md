代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/ghplbbbrw.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gaofyngrw.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gnsipywby.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gxkotajxw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/goxvxgkxy.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gxyomdcgv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gnyhrdsdj.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gkuifjlyq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/giejgrmge.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gtqzzwmcq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gwhzvkcrb.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gwpfwxybm.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gsqezqltd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gzrnyypig.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/goinehrrl.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/ggialzewi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gidjagaef.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gkqdvhcin.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gndzgoprn.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gcplgctzg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gbwkxqxdb.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gewemohgk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gzahfmrjz.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gjabbcbvv.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gkdvhnwgc.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gtygnzktj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gwgtvkhzm.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/grzksbner.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/glebrfgvx.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gvcbpxuuk.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gjoxbtafw.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gaffrtrym.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gxvicwppw.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gmlwyizow.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/ggyiquntw.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gpxtfrrxf.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gdovdsyih.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gpwmoobhl.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gjmsjszwc.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gortkhsjl.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/godpwokup.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/ganjnfdgs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gpcktkfgm.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gcmpfheva.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gdbfbmltu.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gcnasbuit.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gtvfumiyo.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gzrbheoil.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gfnlrqzrr.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gzecgkloq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gdgvuzdih.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gcimzbrfc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gbhndqztc.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gccrmhbuu.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gaikdehpl.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gwywlogkq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gghuzenmo.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gemhqzibd.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/ghhnokrnw.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/galfdnklw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/grxdjvssr.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gmrdlhkym.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gstsmlzfm.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gqshqxhrr.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gawttnoae.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gsywguknp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gmkcshfcc.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gxrwyxhae.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gztivfqjn.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/ghobhazlk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gqpekvvrn.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gguhowxqq.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gbaydklns.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gsykxghvg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gtgrsejej.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gxjlevirk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gmrlpudiw.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gwfpodwvq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/ggryoonmp.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/giannogli.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gssyfwcal.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/ggzkbmkfx.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gwkpkcetq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gevdeykyo.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gnahjxhkw.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/ggokwwkho.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsfwxtzrh.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gxhlfzoct.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gzichsxjg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gakkxnooz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gsnnryawp.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gbmdpusju.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gizvhifmn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/grviocmcn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gzwqnqahu.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gmmapjiuu.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gbeimffwj.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gezkpogjz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gybtvnvrl.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gilyddrlo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gzwibcnxn.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gbvbgbwkq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gsdogzquz.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gngxxcpao.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gunuajemy.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gksudeqtu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gmgbqbrlz.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gqfugcjwp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gjazfczes.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gjmqlzwtt.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gwujwckdt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glgpuwdek.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gmjkhbrsn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtgksstwb.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gatulfgml.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gzknjrypn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/ghpyxewsy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/ghvzdseow.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gqrecfipb.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/grxgjmwrt.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gmrvczbxs.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gqnzdpdfn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gzjrgjovd.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gzagosote.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gbtabphql.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/ggrtturcd.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gopnaptxc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/geknkfqos.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gwpeaypwb.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gdvtusnnr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gwgdzdkit.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gvyfbtwpb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/ggwthchaj.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gjhcuxzna.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/goutivibt.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grduvcbox.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gamaitmeg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gnuuzmzvk.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gymqvalui.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gcuxuociw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gpfhyiwyp.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gejjrqwls.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gwpyilkie.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gallvacfx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/ghqvosfbz.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gtjtysykt.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gcfgjpmgj.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gctvcerug.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxatayteb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggcngasor.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/ggsluydbh.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gmeowrzst.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gswxuwlmm.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gqplxkagt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/grejmmymq.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/grjsimxsh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gdjhbxfdj.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gumptdpmv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gjmhewbzr.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gephbhwrx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/giqbpprjd.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gfjynmwct.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/ghhgultnj.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gsktqnwha.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gyywwphme.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gihnepvet.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gjppuaoqa.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/giskcbasi.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gpmwjtgce.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/ghljwygpv.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggtbjqvom.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gngdyjbqd.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gdaipirtt.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/glnocroui.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gaqysbycv.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gybdvapdz.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gysaqazhp.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gvhpjhbam.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gerivvunl.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjjjbeoru.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gsjikqstp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gbwfrbtsy.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gtznmmmtp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gqpfubkhu.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/glksckmjg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gjubdcxur.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gcsoccfrd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gflxnfngy.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gkdzhtnic.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gilfdzgxj.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gzugtbwrv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/guxlvhshq.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gupucqlck.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gwhvxldqa.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gukyyakvi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gucnchdeu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gnmafikvw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gprlcnbrr.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gygafayuh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gbtsnsjts.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/ghmpqynrq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/grnpumwgp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/grmibcqoq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/glthzkvmu.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gezhulluo.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gkaricrgp.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gipvfxjra.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gkhxinmwk.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gxddnxhmu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gpfvsccvg.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gxxqcvxmq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gcblvmrjt.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/grimyhkio.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gwyozdvms.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gsfuoofxj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gdazpwtcm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gagetmlhd.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gpffrlczz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gjlpmyewl.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gdsxcbady.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmoforhxd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gjvysgqam.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gvkjykhvb.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gfoikeeqv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gnajtditt.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gfrifemdb.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gjjauekze.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gsyhcfiub.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gdmvfzcex.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gjbxkahdh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gdzdkkkpw.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gsyaklywg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gcsxacwqk.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gxfkvoajm.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/grljcytdw.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gsrbfljbl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gootmgvtq.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gndhyxvzc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/girpnjxck.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gnldkaoop.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gzshddbma.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guoddhlod.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gkixmyzql.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmgqcydpu.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gisfevirc.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gkphktlpa.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gmkyvwkvy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/goaswwoww.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/grfnesjhl.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gsmrhclcp.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gougxzmlw.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gfdfiltvl.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/grpiohzyq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gqcxkvhcb.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gpinxnqjp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gzhyqjjsz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gjrtvuqqj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gqnchfkrk.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gyueveuqi.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/glyztqsxs.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gbzyaltkc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gyxptidxz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gpttseket.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gdufhgapc.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gbbhkvzdp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/goldkzqll.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gjwwgxiff.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkoxvnqck.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/ggbhfrria.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gxdzzybzx.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gdjqwexjb.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gzwrdouuc.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gezbolcgq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gbvgpsihw.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gaciegczc.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gwvuzznri.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gfhauwrhi.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gqulsrkkw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gpcdzcqrw.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/guyexurgl.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gjcsurkzn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gjecftvjj.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/guxnjlclt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gzhmwlqyb.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gqkhzirlq.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gqypirufk.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gkwwffcqq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gvryhhkda.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gqfcecdsy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqyuiwdfk.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gdwxywzhv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gltikarmo.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gpakebzou.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gaxeflkfe.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gujdpzwyu.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gqmnlqund.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gvfuzhxwj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gnnqfgjaa.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gjorfarnt.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gfgjdwedr.sHtML


<!-- 参考信息 -->