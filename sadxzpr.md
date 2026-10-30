代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/glipmmqxk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gesejoppn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gmrrzogxv.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geloybsbo.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkfagwfmm.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gboxspnoj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabfywhed.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyqwcmdv.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbchgtxcq.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhwngzzo.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdobmydb.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gaboadexj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjasgfbso.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gqfebuyzc.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvcuvige.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjojzqzdd.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gdybfrtvu.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gwofdqnyn.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gmnhadanw.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjdhgrgim.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvcgpykx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxdwjakp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gzimluhqq.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsakvuxss.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqbyikqw.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ggqgiownx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzlwadgck.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/ggkulmxxg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzxfbbll.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwomuzmi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfntajqwi.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gbydeezfv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjofwufk.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gizyxkorf.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwhvkgkwp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/grpnnnywz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/ghfuqmzur.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbfrwcygs.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gevubyjha.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gsefiedaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gqdtfwyau.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbraiern.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoppfnsg.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gtdhttzld.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmiizynp.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gslcjteao.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/givbvdjut.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/goztbmzah.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/greounelt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkhvzkqe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuwfofrt.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gervtrggb.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdxetzct.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gooudpemw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvycerqv.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gftvjojrg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/giauhnmqe.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunrbjqih.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/ghqjdqzlu.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glafktpsm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gbsazlxnw.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpxixbqn.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gmhkxcjuq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoycldmi.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeqlunxq.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gznqogora.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/geyqsgbbi.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclibphiw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gnzpmszlw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimaypggd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/guuxhkewk.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gwbjmvoog.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gxzajvojy.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/grtpfrbjx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grmdlykov.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvqtifbp.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrnfexcr.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gntgbguzd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmswhjjc.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqauefmr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwbsqxqt.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumsptenb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzsgdxvg.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwxtbjxc.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gfmlcfxqc.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjhtsshu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnkuovdc.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/genqpefer.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiqaoyyz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/guolvqane.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gbzfjewns.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpjvopwef.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsjchmuz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gglrezrue.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsghzlur.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gfsuorpse.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomefybwf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/giejkscor.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gjroygxkf.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gewbnxszd.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gljvwfexy.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzgxaady.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdxpjuls.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmxfaeecq.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaaxdxcq.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gkmjsivmr.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ghxaywyvo.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaopxyni.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqbrcqef.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gqkbaoxdt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjvoffdn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gxevjfxyw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiswttsj.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrlslphe.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gvuqhkpns.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gspeqddli.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gcwvfotul.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gbtynffru.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtakgyqls.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gauxeijwz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gairhwdms.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gbifscaqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfihfarcb.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdmjdklq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gezduvcdh.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gakudpjnm.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiiduxyg.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmmygjxc.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gexvtfgir.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdwdpittb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gwcmzmxbl.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpwviyygv.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaymczwbv.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmkzcoibu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gspjqxerk.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/glccsrsdh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gukoxxasd.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gtkywiibk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjdpcqdm.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjawdasto.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gurqctkee.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdhgrzd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgaklzwa.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gsgaaedna.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/govfpqtnn.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvssxdcb.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gjgtvjcux.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gqninafbq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmawdgtr.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gajugqpga.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gguizuuum.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvityfzfm.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gllzfryqx.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsgepzmb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcodqjlmk.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeuparmz.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gmuvkmaff.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gacabqope.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhzypzec.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhueblxc.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtjjyemf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsxzpyaq.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gehhovfjd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/goqeuliiw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkgvjnuo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihjijvgm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gepxsmamq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzlunksq.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gccoymdmv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghpotdojs.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/giccoszph.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gghoqnhsg.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gmwdrtmwi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gfyezzxhn.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvkqzgwcc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkyjrfgl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbguqdlhj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gfdnyrylc.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/grwucnarp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqdxaumvh.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/goxtyvsos.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwtuhqnw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gglbyhcnu.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/ggzaovvwu.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfjntrxe.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gpgmsxlpx.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gpgigaksd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geexsmabn.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjgsrzns.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkzcimxz.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkxrmuuk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnvsyraip.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gxgudofqi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyjoueaao.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsclabdwj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdehxmdn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gupwlcqbe.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grudugmnb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/geinvvcvy.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlzfsvwo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpgebwjzu.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkoirpif.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujdsashy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaylkbag.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwptgcqi.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbuhcaou.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gghknbgyq.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgivosww.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gusxumdrl.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gsmogexhw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/glbpfnvib.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gtbnnnhae.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyszpogpw.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoalhdrc.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfkuqoke.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gvyrcrvtl.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gkrhrbgjl.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/grdnacvuh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gusrdycrl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/geauthkdu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoxlfdib.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqegrbkfk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/grvxsjowo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtqeiqrj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkneyiya.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsrxejsr.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyvonfcu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gqqhmsfwe.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/godmgpdyx.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gisizafff.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gydenkrtv.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyiqhori.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gvrdpsvxd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqimwczr.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/grctzlapc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/grdchncij.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/glmdduavq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkpwzctz.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoewfrms.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvyqjuur.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqzvstlir.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gnfmmwbxk.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggawqtxnc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gloxgdgio.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxzpawja.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gisncrovr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gaetngsrl.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvdbvugq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gznhdtwum.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwymxhor.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gieaohutw.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtteaoorh.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gvqredeku.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfelixqcu.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmsxmlrf.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gnoszqdaa.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/girwdibfr.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfqaqxagn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/goxbvkhgm.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipcybynt.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfvrccxx.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gknlldvai.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkbtmdbw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcizelrpe.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gbzliwuzz.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/giliapmvb.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gprmovbkz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gikrepymr.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnesvovaj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaqjrcmd.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gitzyljkf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gultxigqn.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnebbtsy.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbqswcuh.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gbaqcdyrz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gefuquzqg.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gwauecpet.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjhamtmn.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/geaoiuaid.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsuwfkug.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwycbwyac.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/guxpubjiv.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoscerov.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/ginrvizwy.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghvphmqwf.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gxycexovq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjxihtxh.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkayernt.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloazrqpc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebixwyco.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsadpnbqp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtakvinul.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaarhvbx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gflkjmdpn.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwunjzpy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxvqitdt.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gnsvtrupa.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnetarypx.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxstnbrgs.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gtuupklts.sHtML


<!-- 参考信息 -->