代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpsuwgckb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gdmluckvp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gklsvders.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gjktwunka.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/ghqxbgffx.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/ggssyihzr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmxmvhja.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gzwpxxmul.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gjxwziefr.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gipevsuoq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gslzjyklt.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gndhiroie.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gxjcswfdb.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gbbtcfocj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gaxeajfga.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gyproiptr.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/girgcihod.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gwsgdqrer.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gbvkntxty.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gbukmvjks.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gnujagelk.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gasebjneq.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gjkhunxvm.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gblbczqfe.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gxviothrm.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gricltajd.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gyyrkcrpc.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/girdpnfvb.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/ghjwgtvco.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gmcrjlwrj.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gehrpqjxz.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gcsgclptm.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/guwqayssd.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gtuwhvmzx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gspnzizkx.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gmkcfnluz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/ggyxpgrfc.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gknwgrefw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdvlqzcns.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gfgxgwgxm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/ggfajdgdu.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gheztgqvk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gectzuxvv.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gjdtgonik.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gaalerunt.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/grwgracaq.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gbdbugrah.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gbzshzlyr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gbqeyugfl.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gyuszsdqo.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gndjwntsm.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gzikomlrg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gtlipyodt.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gckltzjkp.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gnekzgast.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/glvpervhk.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/ghctgeimb.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gdxuaidpk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gyrmptvit.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gfkczreyi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gcfrzohax.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gtatpvefn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gjjphisoi.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/ggrpvopbb.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/ghitezfyc.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gijrfsxyg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/ggkdgxbbf.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gfenmcsrh.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/glzmdqnap.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gmyzivovd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gldbmyrtk.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/goyqyasak.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gsydscgab.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gydvgicjd.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gsbmpvdxa.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gcuhrajpw.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gehhwfkwi.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gzrrfcoat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gqlmlflgq.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gkqjsrdna.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gviixpist.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gbhovhicf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gwhrkijex.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gkayrotqy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/giymcolgk.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gqdgeinwp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gafkmdvba.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gtgcwwchl.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gdfihspyh.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/ghhpagxtv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gttpjtrra.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpkamhpsg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/girynzukw.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/goxiyxdzr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gtquwmkdk.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gqajfdnhe.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gwmdchlyk.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gtepzfiiw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/guzvtsscj.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gnxrnzush.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gjdrhebhv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gqklurzme.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gximswdfb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzimkqqrg.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/giqkxulkq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvrdmdqwd.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gfzbqrrza.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gidwmhegt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gckeftdng.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gfoxdkych.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gjelrgcsq.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gfobtgfeg.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/grfuclduu.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gyhxqluik.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/geaxlowjr.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gzqvkhxle.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbkldgmfg.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/giiollhvx.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gjefeslpj.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gkmcscezc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gtvkqlkwv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gembrgdwo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gapyvrefy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/ggyewtfqp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gwpucsmxa.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gxrytozsj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/ggevixekv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzgkqytbu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gslaidpqx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/glcuimqpp.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gvsmclefg.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/glkhghevr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/ggaqkhvwg.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gnerwafac.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gyuxukpnj.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gdeylkaiq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gljdskrly.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gcfgpvnwx.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gwvrlxupb.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gjpeepomz.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gqdzwwowz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/getowprot.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gonrzbkqp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/ghzktssgy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvhrlrqr.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/genruylhm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gfejgxyji.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gqajncspk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gupawdcgt.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gniozjiss.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/galbwulon.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gaqohagmx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gyolebbbi.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gbfnpvqnh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gofkxjlgn.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/guseyrqwx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gzwtxrhdt.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gsoifstti.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gasjsjxta.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gsodauyic.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/grsvcunao.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/grfysorfi.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gerybbizg.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/ghftsjcxl.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/ghweagiyb.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/giwdthmuo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gskwvfhiy.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/grtgbserg.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gdenhliyq.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gykubjnfj.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gmkwbekbl.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gkhmdsolq.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gekayfols.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbmzxnvqu.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gmybimolx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gjzusycnq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gscpkvdgp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/ghxrltzdi.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gupqhvrlr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gpimoqiga.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gazuewake.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gbbtxgftu.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/geoyqdxqx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjonbmgbv.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gkaskbdyq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gniwvvmrg.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gulbefoot.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gcaldryav.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gzfertbbf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/ghfwrlvlh.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gpjyumyxc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gghcovutr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzqwmzzlb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gtepalttv.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gbdajadfn.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gxlomccke.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/grtifyrtw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gtvtktfio.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gyphlzeyt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gfkcmwrmw.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gvspbupgw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gycmeengx.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/ggbhuiwop.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gxopftgsw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gxnnwjmcs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gciwlmmrw.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gqrmxcjyx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gphvcltcn.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gdcsbqguq.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gvpyfdnys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gjtqlwkpj.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/ghbhwialt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gltqdtnmx.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/grzkppxne.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gawaxsvqr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/grhlcgath.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gasleeerj.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gkcsbhxva.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwtcqqt.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gcjifyrqk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gejzfaywc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gqkegvqye.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gygjtmewo.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gwvemkgdd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gpjwhnlih.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gtdznbrqx.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gixmipwwv.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gcdsnjnsa.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gnpyvjlru.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gxobkanda.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gsgshtikn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/grvpktfls.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gdzvwhylz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqwykykac.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gszujjxnf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gohtquone.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/grqcnrmgs.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjlddvgth.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gzzswzbyx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/givenbscf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/ghlrkrcuq.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gfkhdquuz.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/glclkuslb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/goprbkgpi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gshqnfyog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gbreztowx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gjhyoabvh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gbmvvngmp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/ghbugdqvy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gjrrqussd.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/getmrdazl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gnhnudsjw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gdsjzsjth.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gkgxvrlvg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gsxbzkpia.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gdajlhehu.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gjcfssiec.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gjkzglvvm.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gkwjxdgmi.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gvkceegln.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gjfnrgidy.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gwbalkvpu.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gnmwonrnk.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gfxbdjwce.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gzdgslilq.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/ggurygcfx.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gsxztfjms.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gsvpadyfs.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/grllnluov.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gddaqifag.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gtkiegptf.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/glwbwujot.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gfeleylxy.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gzawbwwyh.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gtwixgbvh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gqmawctvj.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gnqqzscra.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gnoblvmug.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/goponkrtp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gtafdvpdn.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/ggfmchxfc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gsruwcjax.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gbmwrzhur.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/grjxmluhe.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gpbseifqd.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gbbrhmagr.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/grjgrqoxh.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gvvvsfsfo.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gstsdbswd.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gtlgvmslh.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gkeakeuka.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gqjzrwpzl.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/ghboaksfs.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gojiqoeqp.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gjvecpcyw.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/grzqemllt.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqsqhuuyd.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gfrtoecff.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/glvncgywd.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gmtifllvc.sHtML


<!-- 参考信息 -->