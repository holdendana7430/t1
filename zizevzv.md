代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gbnubbrth.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/glpzcqotk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzeadaaz.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtqykakoo.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnoifdqd.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpybjjnv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwogkotm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqrfznel.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapqofxfa.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gufrcaafx.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/glmzcezyf.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvusfqcx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmybqfaky.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkjrjvam.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/galrniljs.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmkkmtnt.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfhponjq.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gnzkakyyl.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsewxpqp.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gsnpmywwf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaxywmgu.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gnwcjfuxa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/ghjwfrcez.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefwarnpl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxdbkvvsq.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/glpdlkwdf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwseyelc.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjgbxcca.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejvzxndu.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiwmcasn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gitjxrfdr.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjcslcdj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguhlnndp.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwgiqshn.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/globripiz.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gphmtdmai.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkjtpgkb.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyspqirgp.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gibvhamfu.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gddsmyhhc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbiursft.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gehzmmjof.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gklvfgbvg.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnbnrhsa.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqsrcroq.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjgjsteaq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gskaxvwax.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwbaagfo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gdjpakarp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcwyszhk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gfyyzcsrs.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyudxoxxy.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gwivzfaga.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpfygvimj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfmzqmmx.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcquukxoc.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/glxbbdusn.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gvtfiwwja.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/giiymnvth.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gucqsjhyy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwulyxyjh.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrwstdny.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/ghoscotih.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/ghxxcyhrr.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkrkwngz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjhkyur.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpilozaco.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/grdkgethm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gywkvuogm.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gwbhdfpdd.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/giexdyqsz.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqogifgd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gexerfrqe.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gqnpagcvx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqunrxayl.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpphbznda.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gmgtxlzzc.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvvktlbd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxupfmap.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/grwzcbzmk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxpxtjuk.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gampnjapi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gydpidtod.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpizujve.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gwcyehjse.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gddhoxckl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwppnximi.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmnwxehb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gferscyzm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gqjwzbsve.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gmfeiheuq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkfkvxsam.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gquptldtg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gogsjnbmf.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqmmpclzc.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gvdifmdej.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggtjglroj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gwmdyadhv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntihpwsb.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gubkbgvjg.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzxlwfbg.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqjvqoyl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/giogtfmvj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizfshiey.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuuvblxj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaovopmue.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gqumizzvh.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/ginbdnfuj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gyymecuin.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gpldkobpe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkovsfano.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gbbdbkohs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gvijjaeot.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/ggxfsmryq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmkjznqb.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxkkrcje.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpyfamoq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggddcynni.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/grzyijvmf.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gukwvxrsp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduoomjau.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdrbsrea.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdzokpsc.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxtjfcqx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdaebdxo.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxulpmgw.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gymhsfzwn.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjbsiuzw.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtmvzstn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjkpworf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gfpyshqdg.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkwsnlaby.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gotqoknoj.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvjvjfbc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfapnuno.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gkhrllybd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnawldopl.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gptxwdbld.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzafrdwnh.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/goybmnybt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gqatjalga.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gowmtyens.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/grfmlnwmg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshedlduv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gkadzfhhp.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsxoruhj.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/guuagpgjf.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/girnkntrk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gjlderlrz.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gpspkpibt.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcspcviv.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzncisjju.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsubhqjvb.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuhbkayu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbtrlwwo.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gmflcqzbp.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwhtpbxj.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gldhmhjeg.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyuskrhy.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghasnryvu.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gfblvnzzr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpzompuzg.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmdlhksmr.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjvxjong.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gwukxemdm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzljqktc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhsxkqnh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbktsues.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gffvwmtcb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjocbomjo.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/glaxpadxh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsonphhhf.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gtbflemod.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gfreivhhg.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/glapeovpc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ghxynerzh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitgoogbv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gfknbfsbw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfxetfwf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gttyvdlvu.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkkbiujml.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwrwyrfa.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimehrnhv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzwfyxcs.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gngrqyilu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gldjhqalu.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/ghouvarkt.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmkwsiwer.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gqolgdvia.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givhtvfio.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gninmkjjk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfmoppfh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gmojkfiju.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhaggjzw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glnetbxqw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gxrgrvuvd.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuvmcrkh.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/geibmkgyk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmhavato.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzdhxnht.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grygutbzh.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gehzikymh.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gboipirpw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gnffzqada.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginzkuvca.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gtelovrxg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gfanwdpuy.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgqfoctk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkgesrxd.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/goegtfvjw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejzcnaqi.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhhfsft.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gooyvdlnl.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjugcwwf.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfvfryoy.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggluxtlnv.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/goedllccf.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnppwobr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gtpmmlqyu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gjleyaoyr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gxkwbbxdi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghtptomrv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqrtpqxv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gscrrsgut.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwfjanaih.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuhevrbv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glenfirmz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknkbioed.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflwwvyfk.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpxkesfa.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfeaxpnu.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggazrvfax.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gcpwrlsxg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwgweufu.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqzqwtjy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glczqawya.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/guzoglczz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gxensvnbr.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpchsehs.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gpjsvmbsb.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjszlbvkz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfgaqzhk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnkuuwin.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxfgngmh.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gjlujqmvm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjumdyri.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjsojfpw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcogrvxai.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gubnavkcf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/guvtbxeao.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gryiwvcpf.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/glnzqejrq.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkwsjtdc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnovcmdxm.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtraxkact.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlhdpqdr.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gceaajjcd.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbhvtxfko.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gbvhuigiq.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsugsagu.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/genwbpicc.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gqmtsaksl.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtaobtpn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjghazaj.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gchzetwnm.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gnvgtnczr.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrqaoadg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gagigvbpi.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehhyvcbu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcqxfowm.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfngwgvr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/glncwvchb.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqegkaxj.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxkkoipg.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gvywwyxir.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gcwkulcij.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gytrbmfpt.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/goqkrknhw.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gysdfssxn.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtezcuaw.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/glrgcxoqw.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmkvagxc.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdfkrrmm.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvlbrytv.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxrmtkzqj.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gubcuktsy.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoothazy.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gejhmzqsd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwuekgal.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gxxsujdwo.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gjrwzzuqr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gznrgwhdm.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gdnvrggxi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxzvtpro.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtakbkcvn.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gzdpcpkcn.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gofvyoyct.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/goopwjbjq.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/givdpekig.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwlnoejn.sHtML


<!-- 参考信息 -->