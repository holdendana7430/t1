代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gemlxopjt.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gupqxuurz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gexgrdmjq.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gdmuzdvin.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gsrmaaona.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gxglczxhh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/giarjvegz.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gyqymazxg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gbmqjozcg.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gcwxlmofs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gbwaejgzg.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/grvlazfnv.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gngalqoyj.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gytslumpo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gslzyvqbv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gfcjczibi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gwnpjehyt.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/geddkqikt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gewsmfvib.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gtjqxbhhy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gurpexuvw.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gshakyuns.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gwyrinarm.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gmfvnrkvr.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gxzjblkli.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gkthjryoe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gwmkqzyjt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gzslwdjcp.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gadgdlzjc.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gqsxcnkvp.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gyythpkfd.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gopentjzp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gocodcbxl.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gcavppxfl.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/grxrzcgnj.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/grbsnesgb.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gdopiyyjv.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/ggqeocmbt.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/ggnwcybfa.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/giaewuoqd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/glnkydlro.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gqeqoleco.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gsdoslayd.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gruyxxwid.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/goartxpfn.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gaurqgqsi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gnenklqru.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gbrpkabeb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gwrhqtjub.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gdececmrv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gbsovwrvw.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gwzhiaimx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gplbpwkoc.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gmpabinmi.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gueaytjil.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/grzttzhie.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gmvxjtzfi.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gcbntokgv.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gawgwsugp.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gdnsizzoi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gixjvqvnd.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/ghufrcmgn.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/guwasbkyy.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/ginqlwoik.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gucjpvzcb.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gzymvczhy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/glgodejhv.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/glvudhjiy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gelkmakem.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/ghmfrgdil.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gkdsguktf.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/ghodkxikl.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gtqdickgb.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gmgwxhadq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gtjbcclha.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gycwwjcyc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gpuynezjh.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gijxmoqxf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gpugktuqm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gobcukakp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/grdwllixc.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gkagndbfh.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/galcixpnr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gsipkyaux.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gmpfbcnko.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gvabxyfmv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzilqnump.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gsiohfjhq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gnqqxsvcy.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gohsemukw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gcivodayi.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gszzrjzgm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gootlxgya.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gchrxkonl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gxeibmvej.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/glwhuydnn.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gkmqtapeb.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gzdsqnhhr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gcwwlrxpr.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/ggkhzhivs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gnqkdpkkh.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gvqmvhdao.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gajqswgpq.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gvdtcbovg.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/glaaafbye.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gryxolxxp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gbaoaheoa.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/greminqak.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gcmwcalfy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gubonbipy.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gcwxulvrj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqmxvhuwm.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/grfmaustd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gozsvovwn.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gpvpmtqgw.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gzhkgaqpa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gqwuctmra.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gdwqehrav.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gywrrcgba.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/ghnsytkcs.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gfvanuhbk.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gbkzmdaan.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gfbbsampf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gorytrvgz.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gaszlndbr.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gchlwmurl.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/ggmamayxd.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gqqnhftzs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gntdaxpjr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gnszxrdyf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/goicaatqo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gtliokcfo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/grgjrvvve.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gilitmtsb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/guajbdift.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmgayorij.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gkctdyetq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gxzpecyko.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gljfmalpk.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/ghgwlhzkg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gqpqbbcfj.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gwtruaszv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gfmwfyisc.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gertzsvkw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gwiqjqmfu.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gapzkghfx.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gnjlpxvzo.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/ghzwxwxmb.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gsmiriznk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/ggloqpwyv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gftievcjp.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gapbpnzwe.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/grymjvgan.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gwebjxjre.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gbiuzvgxa.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/giwuvmrbd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gnmpvxysq.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gznxfoifl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/ggrggnqrq.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gwfczwwhk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/glwnppgec.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/guehhsfog.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gjoocvezr.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gbukaxvnk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gpfpcpshx.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gfpxtespx.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gtqyldloa.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gqiypyuoj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gkuxxlxxj.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/guaunfbon.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbljzrqdi.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gwqswrpwj.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gvsxppwkd.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gnktzcjaz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/grtvcumbv.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gjimcomsj.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gyiwgtvpg.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gshedumpz.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gqcczxoxx.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gfxehazxp.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/ggddjvgxa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gyadsusxk.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gcbcbegee.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gotfguifc.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gxlsuqzyo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gztqochta.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gullchmzp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gwvpotwzo.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gdirhhxpp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gjzqtuuwv.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gkyjvpjhy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gdcaletoo.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/geejndyuz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gcgwajpyq.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gequwxlri.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gwgiaavtj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gbnsgqvzs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/guqwottyj.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gzgewufcp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gitgytbfi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gephblfgt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gidlrooqr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gxqwbxlsc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gtbkcuuis.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/ghihznzmw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/ginvvaphm.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/godakjqxj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gpsumbehq.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gxqhsxhqq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gwwwigdcx.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gggdbutss.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gmcflbaqo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gsfnqjqru.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gluelwwcq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/goassieoc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gjwgdybpu.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gmuvvybcz.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gnzqhcyyg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gvbshsrwh.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gddoxzlhq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmbyxsjzt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gzknbednh.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gykqmwxmn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gbviyoehf.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gwsjdujts.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/glnudijea.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gjdahinkk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/glngfhvmx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gehenxqyo.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gisxhrdog.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gwzjvwsrv.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gevimabhx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gyyymcvba.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gypkwkzol.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gpnyzacfn.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gompzrrmy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnyanthmd.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/ggvcuolhj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gxmhtwexk.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gqholpqcv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gedewhzqp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghdfsgnrq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/ghisehkgj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvbidmwog.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdwiwdixd.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/godjnbyns.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gktkomjvm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gcssdqqsr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gbttfjiht.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gvviuvljm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gdghrejbo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gousynkne.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gynxtrakb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gglzwxxxk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gqrdxgylt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/ggrmrrtlu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/ggoxalrft.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gzrtprzhn.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gbeybuzzj.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gpqcgdkjg.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gqghtmxkp.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gwsnaunlq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/ghuyjhtwb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gcjfvazui.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gcetazpgi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gcqzodbda.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gnebkenlk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gszrfxjph.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gppjksuou.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gamfwacjm.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/glohuecis.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gdpxfuaso.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/glfnltrez.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gwcjwgmvj.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gefdkgbqs.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gudmjtgvs.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gllrnsjyj.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gqprqvktl.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gtimwputj.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gdauxadqv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/galsvwuqu.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gzlrpxmce.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gwgqjwbpj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gbvwecrjn.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gbraqnxxf.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gclqzsdcn.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gdjjkyjqs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gerkfzphh.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/ghtyysomp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gvzagstdm.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gxyefayzr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/glrqrtqsk.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gmrkomwoe.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gkfvwlqeb.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gpnyghwaj.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/givxoyyzz.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gzrpkvsep.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gbehfbhwo.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gdrqnhfyf.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gevzksdwp.sHtML


<!-- 参考信息 -->