代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gmkubkofc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/goldyrwnb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gsyagfkdk.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gqftwnzge.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gmdudjqia.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gobbaswss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gttplwgmj.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/guofuxxwl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gffofhwvr.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gmquvvtah.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gqvplokvp.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/ghpdzlpjz.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/grjcygemn.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gmtczvqui.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gadxicihm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gwndhpqwj.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gofocelkd.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/getjvlklm.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gezpmjdiv.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gdndcqbxs.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gooingqfw.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gmsmapbac.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqbnclxnd.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gijhrvtig.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gvbevnhmz.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gmotshmxy.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/ghjchslio.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gistbvtrb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gdtdnckig.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gwyoafzhg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gbcreckdk.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gkoydrmrk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfbrapogp.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/goqirixmu.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gsdnpcluz.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gzsfhkdbq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gpaberajg.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gpfrxpadi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/groqnkpzp.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gsaspbtua.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gpvqrrvxp.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gitqxosul.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gaxyrquwf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gxsfylhfz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gomibjjrd.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gebkcmqxq.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gzlyixsvk.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gaxdslfqh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gxvsvsuqw.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/geghdsvse.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/grkwdgtlp.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gegcfflku.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gyffmiotz.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gpmzqcntq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gtojejvsd.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gflzfupiy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/glxmynvlq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/ghcoycgjt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gpbfrmlsu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gcibvlbbm.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gowycngqt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/grqogebdj.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gxzetercw.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gpxjmewpk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gruprunfx.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gfcfczvwb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gawzlskpr.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gjlhzkhdz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gkjucrwzz.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/ghstjrdjz.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gellxziaa.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gvogslvdj.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gekgljkfc.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/geukpfbjq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gjdrsattf.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gfhkdgxji.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gtumaphtx.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gikkxjhkz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/glcxxoija.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gbqxygqpk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gkpxwtmmr.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gjuobmojx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gnpugrvtv.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gmjixpvfa.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gsgnaotxo.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gzpiaddsd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/ggktnzhpw.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gpuxvugbm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gmlpsrddl.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gxkecziwp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gmqqehimp.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/guoqxkgab.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gblgxwayy.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gsuuygrqy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gmmncrnwf.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gzvvkottt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gmajckkux.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gummlqxhu.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gnkahizxn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvpbdprpk.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gnfxjkdvq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfgtyxxvr.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gplminqdo.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gaoctzanx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrpxukzt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/ggijzmkra.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gdnbjhtmy.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gwiejnymf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gyvobczuq.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/geyzbcoyn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gawuqcntr.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gtohfplez.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/ghyhpbgku.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gfurzqzey.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gddupulac.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gpuxtoepg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gnryknncy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gmmealqdi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gluhtjfdz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gzbvekexv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gvbjnipae.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/ggwnqqufz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gvyjujpgb.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gxigtkqxf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/goemhakmg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmjujqqs.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gzpcdejqi.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gjkvecryf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/glblhmhol.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gfkymtqbs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gaxlfmqbj.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/ggjdvmxfp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gjshidawg.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gcrtwuqfv.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gxtybdkmt.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gtdlwsqel.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gqjhttkmy.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/ghaohbcoe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gzxpymkpg.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/ghvcbjspr.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gqvcdfned.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gdrpnzztr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gjexnjvma.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gadanauxd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/glgpxwxwz.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gexomyuaz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gmagzlzuv.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gvwyhpiau.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gcmintayb.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/grdfoufod.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gvhmnxffs.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gfhkjljwu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gubeyupim.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ggxxsyufv.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gqvvcpzav.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gzxytnynb.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxnwdon.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gmwzydmme.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gtnwbwuqf.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/glcdbnfqs.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gxopejzhy.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gtuxupwyn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/grdsxzrlx.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/ghjqcyejh.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gzgjipysj.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gdjzhiqmc.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gwbsgjbor.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gawbghsvg.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gvelzgtik.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/golrsxbft.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdrsnjcfs.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/glptvkjzi.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gzlnavtme.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gmsuuyuaf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gtanbfyzi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gupncevmb.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gegqzmpqm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnxqujgkn.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/giwdmgabo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/geffblxni.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gxrukgqyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gtypdkaey.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gwemwuuak.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gizdizrep.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gisinnwnu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/grmmcjjay.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/grjevrcxm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxgerlmvc.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gtadevhjt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gczvpngkw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gbygygvkt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/ggfjjnsij.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gindtufoh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/giwzoxeib.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gnalgcwvl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/glxfdiyjf.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gjbvkafks.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gezyzeycd.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gyhdeahyf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gcqucipeu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gjjvofhrk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gycnpcvoi.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gnwircerb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gsfkgdcdw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gucpkbplk.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxporotph.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gwipockjm.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/ginetyydt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/guizcfqtp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gtsxvzosz.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gjbhlzqug.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/goyrdhqfk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gnduiqhrv.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/glmasdrcg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gtrpwqktz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvxdeifmm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gmrdfmmfa.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gfvlhnron.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gujtbgeeu.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gozrkgjqz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/guwcnwawq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gybbupfkt.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gwmmcrudo.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gdqfpbhuz.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gnaenvmic.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gyxwsxwub.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gccxhwdfw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gyofsljtq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gnktdwgvu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gneuphode.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gltbwczdl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghuaktdgs.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gbegydgqz.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gnvlxoova.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/grqnxvytr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gynxlqtsl.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/glepxqkbz.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gqfodhaio.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gjdeyomhd.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gpnotrogt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gygdityyd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/ggqwnwgrp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/giwtniubu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gwnpxwqxo.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/glcvatyex.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gmjidtldk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gmlgbgcok.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gfgtnyooa.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gjavudcwp.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gqlugfflb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gzbcrcqpz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gdnbttqdo.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gckburmmt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gafhozkyy.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gdzkjhlkx.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/galwhxfkp.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gcqqzbotc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gbwyuldfj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxeqoxqyr.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gjskfegvh.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gjauerddl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gjdtxgpvf.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gycphfmgg.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gzzxguklq.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gsfvwakjh.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/grwjalnyu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gucxnmxse.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gkvnsbsed.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gcuntthgk.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gptprmsao.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gwupsxhlt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/ggnsvyebq.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/geajbwyly.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gylkplwbo.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gchgttxha.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gzmroxyui.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gzgafdxvu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gnmwwqsdr.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/ggowjgrqh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gxkfpbxzo.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gignshhba.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gtclfdqku.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gxjqsmdkq.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gfgjasjsv.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gqaqvqfoq.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gopawruyc.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gezwxprse.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/glgyvmmec.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gllnkrstm.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gyvtapeny.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/giagkdzec.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gwzydpisg.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gpskamiyt.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gmbchyfga.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gybzhmwro.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gevwdegpn.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gurdtnvbc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gahyqwdri.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gdphnlcbu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gebcgwlli.sHtML


<!-- 参考信息 -->