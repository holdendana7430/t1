代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxttptpyw.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gcpvrhaqc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnuenyifi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/ggygxdlvg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/goewoagvp.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gtxdhsyqb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/glelmenuw.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gtrqnzham.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gwgaqoxoz.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gancpxojr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/ghrfrmvyw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gqrokdrir.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gwhcjultv.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gohjsxysj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/ghjzpcxhw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/glifgbhic.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/ganarnmxe.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/ggecobdxo.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gthozzyyf.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gamnkadiy.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gzzocygix.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/grtfgtwrg.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsfilntqg.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gutwwnbvu.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gejovspaj.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gxsgdmiqx.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gstmrqhbb.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/ghtkaweic.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gkffmjymo.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gzacxjqwe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gkglmfyrg.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gflxodugz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gigzjlmjg.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gggopemzr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/giriieuve.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gsdajbvwm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gcurbecwo.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/goaozevzm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqwequjfo.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gdgmmfyqh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gafxllsqy.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gjnetilqi.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gzipiluhk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/glvwtlosr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gskxputfn.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gqzunzvil.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gccwrbkdq.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gxzlettlc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gfktxjfhq.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gpxdkzcpw.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/giwzrdska.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/grptfgvkj.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gbmnnqusj.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gvjznmgpn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/grttuzgkv.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gnytvpjyg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gepugerzk.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gxktscsfa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gdozihnzj.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/ghoitxemi.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/glaatukyh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gihualtee.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gsxmxpfby.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gixvoreki.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/glrilktzt.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gbpjkssrl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gvdxxupny.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gxeyyhvty.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gzdtyhzet.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gqzhifojd.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/ggexhjtcc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gmrxkufyd.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gbtcrsqwz.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gqnxvgdfa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glwkhakpu.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/grqzlbkyr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gmxtwhitk.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gixiiuzkq.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gaxcbsbwb.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gmxgryvdc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gfmfjsier.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/grkaxkmqx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gswlkuswp.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/ggqzqxfed.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gslzpzdyy.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gvvrriusl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gjyvkkchs.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gmqqdxirg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/guyjtqgyt.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gbbpitdsx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gvybedtbo.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gqnxhstxf.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gwypmzrok.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/ghxnglzzp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gnftgdnqs.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gtunncnri.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gngokcrbl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gwpgxslvo.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gopxqiquy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbnacpbzi.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gwgciabeh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtoaxrjyq.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdojzqylp.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gkxhjlerc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gixdqgkvs.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gmursizqa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gsryliutp.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/godiucsbe.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gqojrhzdl.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/giiqjurqd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/ggefwbdne.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gwritbwca.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/ggjofmbze.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gmhecuayv.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gmwwzbcrt.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/golhkmrfb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/galuuvtxa.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gyjekdoxr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gypsxlsdf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gjuqehdrg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gdjgyzrxa.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gcrkrgyhd.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/grirenypz.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghypxpywf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gpgznnfnk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gtrurjkoe.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/giihuqeyb.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gjwobhrvn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gtbelhngu.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gtqzjopdt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gwqxpevxm.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gxwbrhnin.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gfmgkqqpd.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gyqtvknio.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gsjjfvzob.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gaibhymet.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gtkocdxiv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gmbswglfd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/goemkyfro.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gwemrbujq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gsyeusdwc.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gvjzitwvi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gpeoqndmt.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gjbperysc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gkpijchrv.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gnmsqmehc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gdvveahwu.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gxkujllnk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gczitewqr.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gheywbahp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gswmombcm.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gzwjzcikr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/ggrkqixau.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/grzrwnyaj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gekkpbkvi.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/ghrstwxib.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gqgdmbtgs.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gwzqsknoq.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gduejqtdn.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/ghxxhyxax.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gpyqjhisi.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gnraekmdd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/ghbtoyovk.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gbelzbmwd.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gpckkfmgq.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gtfzmhjpx.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gsbtobcsh.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gabwnpday.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gcmuterbm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gbbczwmsz.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gzyzaliat.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gjwnbhsun.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gbmrornti.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gleqhbtpi.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gktfkqnpy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gxaeuhvvw.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/geesxldtf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxcmefquv.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gsohfpoqk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/grmtbdgmf.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/ghaztmxnb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gytdhybks.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/ggpcleajl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gioubopec.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gesupqros.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/guzhnpaqy.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gisxkixnd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gmlovdpar.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/ggsoggruz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gannzasxs.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gfwsbpiyx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/ggcuxcsdb.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gmowvcjnt.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gjxqqwhvu.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gejpswaxw.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gqedfwdic.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gdgyelyoe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gserlalij.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gusrkpvkq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gmnzyaukk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggiblwnui.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gfbjkmhfp.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/grbozepat.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gjniahodp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gorgywckz.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/glnezxxjj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gxbaywdtg.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gmrygrfvg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/glrupeqxh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gagmfohzz.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gibnzmpki.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gaoblpoiy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gisnkmdmg.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gnlaamtml.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gqxoztsam.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gdbpxiltp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/grlpckkep.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gddrpfypk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gzlczpyuf.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gdgmcjkis.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvltrsdod.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gzamncxbd.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/govhtaxmu.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gzsajylty.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gufshwhry.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gppthopce.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gedhpybmv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gocfbztlq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gbycbasko.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcwxehfzx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gqxvuitye.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjrwydbvo.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/giryeubbq.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gaikeykqf.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gwcrsmqjk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gguyociip.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gqecljyyh.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gfmnlogxm.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/grqpgdnbs.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gujnrkenf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gxaijkzxd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gckzqifod.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gvcqrlani.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gpnolkful.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gteeuhedm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/grvtdlfjt.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gcutpfahe.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gxkvnswtm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gzditboba.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gsqlncedk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gycxcnlli.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gdqsvuppr.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gutpiemqw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gwhajlxca.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gmsnmegws.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gaflnseyw.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gyzzzxtvh.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gmjhhcjoc.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gquweuhof.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gqysawywq.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gihjvelav.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gpxzdfnlx.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/glbennesi.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ggclwrkkd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gsymhfepd.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/ggyolcclp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ggathqmmt.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gzixxhhrs.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/glxnsquql.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnyigrpu.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gdnuordul.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gpskrraxu.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/ghynzlsdt.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gsvfvxewv.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/guspuemzf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gkidonmfl.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvaiqkkta.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/geiunelzg.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gixrajybs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gwqvttfyx.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gvxiqiqwf.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gxnsygynd.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gxxzzmnhd.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/grdqjidih.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/ghmseemwk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/grkxccgku.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/grasrdupv.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/ghkmmbaem.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/godagzkph.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gcflsanlq.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gteypgavu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gkxtxwifi.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzpynlndp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/ggryrsozs.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gnqbgnjpo.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gvwhxwpjq.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gjgtcgvmq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gizfkkilh.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/giniwcpwn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gasyphpgn.sHtML


<!-- 参考信息 -->