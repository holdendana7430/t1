代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gdptpgcem.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gmsxgttgz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gltcoruwj.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gobmtvjnc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gsxtbiemg.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/ghzfxaccm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gstygitls.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gnzauarbn.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gfkmhpkij.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/guhyiqlax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gbnbmriul.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gvvhugcwk.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gvohvjvpp.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gilpmtjns.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/ggrsowpox.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/giptxkmad.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gseysbgty.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gqihfdcys.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gaoytcjus.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/ggbosgvaf.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/ggutmgiqb.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gibxvpybe.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gvjoixepd.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gzbnzuzhk.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/giqorcvgw.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gjyyqodvv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gqhbujybg.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gvyobugfv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/grhujvouv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gznyebzij.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/ggkcslepe.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gyerfczcb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gxyxypjeq.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/grbqibhvd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gchndomkh.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gikgyylxr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/glydsuteb.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/ggciyzmmo.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/glryimkrb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/grqjpzzpr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gqlisyzpf.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gpjpdyner.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gqdkvwdza.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gzzmbeeya.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gwdnwragb.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gaatogtzy.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gbowrmzdy.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gyuthtprl.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gcvizltup.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/ggezlcbjc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gdvyxrmjw.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gowsbtcwr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/glpcufwkq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grwoizisg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gupdxpegm.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gkrhfyobm.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gtyeqeeqf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gwbntbmjx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/govtudpbz.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/guldkycuk.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gtmvlxpjq.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gaylypnmr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gcoshdobj.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/ggcbwzcwe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/ggvnhafjs.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/ggwtpfuwr.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gnxeginmo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gshkqevbo.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/grcogdrtk.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gprlrpapg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gfgchcmae.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gczacwunv.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gmjedggvh.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gchavoaor.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gmojvmxjv.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gdjrfubof.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gtqvjaivd.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/goxenzrif.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/guwzpdyoj.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gcbawxhzl.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gowsqphqx.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gahwndxhh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gwfvjaswg.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/ggexsznzu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gbuplovoq.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gyiidyohe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gqkmpnktk.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gsxnftyoi.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gaervppce.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gdcwawvws.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gheodbkua.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gcteyhidp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/ghmxisntj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/geajoonlb.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gcfgbecnj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjckqttgz.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gyhtksopw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxeqxybps.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvldpouwq.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gcodpecan.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gclnndigp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gkkxlbhgw.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gqhnfuvfa.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gosvilxqz.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/geonpqaqs.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gfigfqpsq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/goamrdowx.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/getjyokzr.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gocrhtpht.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gvxzemogh.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gmyklnhpq.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gvsliuxjz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gofapfwpa.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gbxgdnbke.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gplopqtkz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/grtfhhahe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gnsrhamht.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gdhrxexak.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gioonxuwm.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gpmsgrlrg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gfixpkvga.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/grzvjmbrq.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzfonlldx.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gpfoailtn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gidnymtxt.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gbodcomeu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gjdpupagv.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gxlsypeyi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gpwfpxrub.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gpphxcjfg.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/getpvgmvt.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gdjymmhkx.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gonpktcvr.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gtkizvhor.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gpxqadpjk.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gnxtrzzui.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/grfyzbfun.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gilrxfkgl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gmsnwnzzc.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gxkawkede.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gcbpmvbph.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gdsoauash.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/geondlhjz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gwvdvujgt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/ghjhjtrfk.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gmmtlagvo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gnlksovvi.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gzkjiiupz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gxvcoqhfh.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/ggptpomwc.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gcrzfgtdq.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gkjalbthv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/ggzsclyxe.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gtdzowfft.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gabjynulh.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/ganaxfvmb.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gbrfuobdh.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gepxyogwp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gojoqsxwa.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gagrtofja.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gsffryojq.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/geywewefa.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gtbrwhzom.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjbthipzp.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gbkihdtbn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gjwdjhqam.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gjvbntegb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/genqdxfko.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gnlnjiior.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/glsjgkvss.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ghwpaiclz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gfzfdjwzj.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gljomrkfg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gknniifuv.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gbhojksjp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gssuancox.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gnyvajufr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gzmqpiisn.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gtrhgqgct.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gxuyrllhs.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gjkvgpgaw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gzfzxlqfj.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/grztvbzwv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqfvbmebu.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gfvevkbkn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gljpavyov.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gmluqmaap.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gtziethno.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gcnvxauzk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gowgxagfu.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/glogabrcs.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/grldjqngs.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/giqzhxuhx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gdojtfwbj.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gflagpzci.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gdvtqwqfb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkyabssjm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/ggarwhngu.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gamnsdvvh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gvtzzalui.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gnpdqmoii.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gthmnpuzd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gobohduyp.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gguztqklk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsbxspyzz.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/glnbjzadn.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gawyelomc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gmqqdlpqk.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gcocbeprp.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gnijdwvfv.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/ghmwpqmpy.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gtwwpgcza.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gnkggkvez.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gnnlkqokg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gyzjvqgne.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gutoohyov.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gwaftjnso.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gfkvrgwsg.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/ghnwmfvkl.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gvgspdiuw.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gqkcaklbl.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gkiibgubj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/grlhkuunm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gtbphrftg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gxpobdqgh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghuecvqcb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gmjuyxort.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkfyydwrb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghvzgzwsu.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gziuheurt.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gqlngwghb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gstevowdc.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gtdtrhbwp.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/grehrbbiu.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/guryngqfd.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gvgmkpbai.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gzwxmzcve.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/grimjhrso.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/grcpiipoy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/ggkkfdpkt.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gtkxsyvtb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gntxrftnv.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gnjovgfgm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gynkmczjd.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gqpvqnuqm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gasmbsght.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gqwebpidy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gpdqsoqdv.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gyvffjlqr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gjxxbmrqt.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gfjnmlvex.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gcigdjrgn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gzliniybs.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/ggypqamcy.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gpmcfisch.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/ghzigncrq.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gyoktckvm.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gzfuntgwg.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gzakslyvf.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gmmsnwiyk.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gjjcrizrz.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gqbnobzdg.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gzwjjanyw.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gzkpzaoly.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/grgrkxgff.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gkxsmfxlq.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gepccgitc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gpdzrqick.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gwscllvzz.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gcseidwtv.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gwowiggco.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/glfbwqdvv.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gkfctksrl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gqyqzeejs.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gzsggsqtx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/govryuuyy.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gznmeoqfm.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gymshwcow.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gqhhihxuz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/guvcmxmso.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gpefdzljn.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gaftpbbdv.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/ggnzupskv.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gwbjmhzmr.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gkxjnlrts.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gpltshfum.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gynzlixpr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gpvvatwgr.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gutaanfud.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/guzyphsey.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gutjbyijc.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gcqeclxim.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gcbxtofpo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gzzlwvwtc.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gcjuozpzx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gcodnagtd.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gqjbqhfjw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/ggsyfmloo.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gxoonxvvu.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gcrlmdpzy.sHtML


<!-- 参考信息 -->