代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gtlyzxhhe.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfduofstr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gpfwkzzdb.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guzpyqcvl.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzvxqevj.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbutdxzc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gchukvulx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gguwfhmgb.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrtqspcd.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdcqxksd.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/goybisklq.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gqqjyeeqc.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsnqpqqd.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gjllkqxaq.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnrnfmedp.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuoonyvi.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gerfhvvft.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gnnwrsmyp.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gzmcvxkxd.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrkbbtdt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gjbunzfae.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskjwdvoe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gxpnybsan.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggqvrmhmw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzptymcmi.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/ginfbqene.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdltjonfn.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcuvvmbo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrdhhdjx.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gadxfrtzv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjqnuqyx.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpwobuya.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymifcsum.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/ghetticuf.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogsnmgjt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/glhhbnqbm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gsgghgbig.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkcqvwwv.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gghqwbpwd.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gtksfhuwo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/grlovltpo.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ggajhdrwk.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/giqqkemnw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplnbapyj.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/grnkdjlxp.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gochmdhlf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlzpxevy.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gwmtubtjk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/goudfguuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/giytsgekt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gmeekjtps.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkztnlkys.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gcezwubem.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuqimpub.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gworxcuzi.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjwylhkm.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrovjccg.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/galqgykij.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpvvrcdc.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/ggccqsfpf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gflrfgpfn.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/guojtqyib.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gfjklgflw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gseoykuuh.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwvdcnus.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geecuclgj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrczzesf.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkkygrfg.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/goxjjuhlp.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gnamhfher.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gzbeqcpmd.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgtlyycd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gdbjbeago.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/glnaoflbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gufysojmw.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpaxhkxp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizevnmsj.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaumakva.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoamysnr.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gewfdqolb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzafpelh.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiakyoyf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gijydkzbt.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgpldhkw.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gwcdcrvyh.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/goneopira.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkcfyqsb.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gyrtkonlm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvudojhp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyywvdke.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtlfwkth.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghiqhogup.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscbwuakb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geztlljkm.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggicnirkh.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gikpghhwg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gffloqvas.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gkokkbnha.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilsumbut.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gnvnnfebq.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/goaionkpc.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/giuvaysmr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdjcymsb.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glcayaomx.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gshaknraa.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqbdasxx.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gklskwgxb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gehjsnptr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/goryqywwd.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gwsflzqlk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikxecaig.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzqjyxjp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gmladpfdi.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gjeavvixk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gcsmrncow.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/galyjkxdo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlrtkulv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gvurjmwmd.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/guktzrgef.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyllwvhu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqobduqvy.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gxcsrjwzi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiuilyko.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/goskndftk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gmbtmizlo.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgrephkd.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/guutfzdna.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoloayfh.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gechbjulb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/glbhoufcp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/goljshbgn.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gpzzqtbwq.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gdagasqyu.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjgbrofts.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrqejzjb.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/glqbwxkpb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gajomnfof.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/ghuevdbdq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggottlobo.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkqlfwdl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrnmyndb.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gemjsmejs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gitaypymx.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/grrmyhxbe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gyahigajc.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldhovexb.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gojsmqkte.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/guzzywkny.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gptqkayme.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggirsprhw.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gctwtccka.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqesyficw.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhejbqcb.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzznvlzf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgrcqefd.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gssjgdvrd.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhwdfryc.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gqysmlrau.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyvztwta.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjywlfkc.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/grgxvrujh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkksxwuvy.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuftwztq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxpqjzkl.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gdxjyebag.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gcpcltdoa.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gdegyjprh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxmsrhai.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwlxttkq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gathzwbjv.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gmwfieavs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjwpzmnb.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvjnkksg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdkrkfpo.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gguokmiod.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gegwwhhgn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxllypmui.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/glkjipilk.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghbrrjeqp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfmduqrc.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/glojplcww.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdslhvyp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpkqbgvx.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gazynifba.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gzupkdqyn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdphcueki.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gietuzqdh.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnipmlngk.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gebyewbgd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkcysahl.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/geoqshqzw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmwuydbo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnafwopov.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gddgxpyrn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmkrycwc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyonfmeya.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gbtmpjcdb.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkbjkpnw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmecragxq.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqdlelsk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gsrjzacfa.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvnautyz.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gknpoaaet.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/geyerhotl.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfrdumcv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhbmrxbq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnlwcsoi.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gahjmmeuy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gngehzyjx.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gojzevjny.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutkpwyjx.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyiprmec.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitaozkuu.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gogqrayjt.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gepbfscwt.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvwlmhyu.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/groxdipvg.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gudwwjcky.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gtekjpzso.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggodfhkfo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqswscpz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqekpaxaq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gncfepfba.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmjeyfcyh.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzedvujfw.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfrxftnb.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxufhotzg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/glxgafygp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/goekigdsd.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeoaynmy.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhdyayuz.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gpnygtuqy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/givwuqttx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gpikgnykt.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/goeflfrff.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdysofdg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gdimmlozx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvrwwnwn.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/geyecnglu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gshgylxdw.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfwwqcpv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpropagda.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvhtsgdah.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidvjafwe.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrdypijb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyywffsg.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/galpxnbeh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpemwdqrq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsoocqxr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjwxwact.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/geerxlfnl.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgolduco.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzujgykln.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzahnuler.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdjyshrw.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdrfjwmw.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvkjupsaa.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbmrbess.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcfesijb.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gwuhlmqan.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gymyyaotu.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gqvspollp.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gwdpszedo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gdawjvxgg.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpftonno.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxxhyjbd.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/glqnsrupv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdrejlve.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlymysfu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/godwjotik.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/guvkudmdj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gohwmvjir.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyoqwhhb.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkwdrdzi.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gdoljgdqm.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmpjzdbc.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/girjsbsel.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gakyminut.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gzjcjnwgx.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gshnfvwko.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulgfqzej.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gduhcwwry.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gygotdncl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoqvsghy.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkbdiilly.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzqbktxmw.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glzlpzggn.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gafbyuqtr.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqghhhxjw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gbsmmdbbu.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gijsdevip.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/grnizbhop.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/ggeyzhslp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyarxrivl.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmjvwnlcv.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/greovovrp.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gpaisqaqs.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/genuwsirm.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/geszkzvnq.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gydwtyefb.sHtML


<!-- 参考信息 -->