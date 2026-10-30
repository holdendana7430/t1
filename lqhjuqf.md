代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/ghezxppvw.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaklslnno.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gzwzzpxuy.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmprhxym.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgcqrsuw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvzzxzgo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqczvkqv.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gggxkajye.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypjsmfzz.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbccgtxd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/grtuptryb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdkrjybo.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gstujepej.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemzmoyua.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/godifaawu.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gwxtbzbos.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzvsxjob.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjfsinyk.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxpabifd.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/guimzptmt.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfmumbom.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/guuykvmdn.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/guzxyiuun.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gdyrmolbq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gbrouzekv.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/glencykap.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/grlikiimb.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gogczrysj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggxdzpeer.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwnbufjr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwffyzxk.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gybdxljow.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrglmujs.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gwmgnhpdj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvjgfzclh.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/grumsjadg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqguytgm.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gtyxutyid.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtfedvisc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbqiokcj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmncgtqwa.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvtxikkx.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtczecbgd.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gfdshdmds.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gjorilmds.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlisecut.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/guwkvcagl.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gwlvklgcp.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gawaypqoj.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gclkrhboj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfghrjnfq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqligkhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdgpdbmj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gfrvmunyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gtvehhldw.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkcgoibj.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gewlambtn.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvlrelvo.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjkmekm.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxvqmuzv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmyfkotm.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxzrzmiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtnoibcf.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gpufnreid.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gckszywys.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gjnnrfeob.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxogderdr.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyeqxutd.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gslazwkye.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlwwhsif.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guywjikjv.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqbfossg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gszwymoqv.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtrdjayi.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gxaujxpgh.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsjxpeeo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gldlowipl.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlrylgdy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwwithvhr.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylpfgrav.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdvuexaf.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gwazgxflz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvzjyshm.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqzauohz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gasraxygo.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gefscuxag.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqvfxxuf.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gvinyrahc.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gvujfrbkk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjmjgmlw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvehnxohe.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gzntdsvcw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grraihfwg.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/geqafwfne.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gntzrwsin.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gucsvxnlp.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubbydafa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikkgojyu.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsbncxhq.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdbyeeba.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcfzktesr.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gtamukpjy.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrdedxdv.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbymtfuln.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqximahd.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdczvzyg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguyvsnba.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtjtpcyz.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmrdswbl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfexzrsha.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/goeeffgzp.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gneqoeryf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/goxhvnhbh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gyvypswma.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gqbgbgqrc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gobvjkuwq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gwryakxqe.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gjtzxepre.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gjoimpqzs.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwodsxtpv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghheklyry.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/guuxbregb.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbndrpigi.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcttbzgh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvbxzcoyw.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gsmypdcye.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqlraejj.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gaywqjcnz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/glmqarpyv.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glmnjydwe.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gmosgbhnh.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gcpbbmrzi.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxnipafs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gakefrzos.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvxzycgv.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfuqynac.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gusalienv.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glqzfrnco.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/guhmwoieb.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gkqhsrrfs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gpmpovgdk.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/grjojxdfd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/griobzrne.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gtopelvqh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbufwmrhw.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxjgyybw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpazcigjz.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtdutjaoy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gsynsjagy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvxwlrjo.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqapyddr.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golbddedy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjggbbejx.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gdilhpvng.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpzjhyww.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfezrkzsu.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gjtekpcws.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gomyknero.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkrzhctl.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gjyncjypi.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gsbrlynbt.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gaigiufeg.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlzrdffx.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdvfjuzy.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gscutznbp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gymwysdyu.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqtgriit.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gcgsbfpes.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/giglyfkrn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxyjubid.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gikbmlkpa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/glvarnxak.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gncdifkav.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdzgxusv.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqubwsgr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gyohxhspd.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gthqylwud.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowjnkmoo.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawdoqvdh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvumrkpg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gobrcprmw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gwabygucu.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gycdzbsec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gtbazytqm.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdtxtmzpa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxjscyzx.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gggpgkgeq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvymjekxq.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpwdfjob.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gheemdasp.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/ggjrhiqzm.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopecfpdh.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/guctzfgnq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghcqzqslo.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/geeanijyk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghpfdyfpo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/glqdhekup.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyyhtizld.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoddmtrg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsrrkxcl.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gchyykelu.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gllphptow.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gswlvewqp.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gittkcmrd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcejfycbs.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlnwqxzd.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gdwbcznnx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizmxqshj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkmsdbhxl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjrqwpec.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpiohufm.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gipktqyhy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gacxjptym.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnfosmob.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmewgmdwo.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gpyxhrzvj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfflppafr.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gshejifdb.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzggslsht.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gocxtrkuv.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gudbxzttf.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfyqyjsg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvkieffw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnarudsj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzywuhoc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gersuuqcx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmffdsodc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubvsvrft.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkltpnhx.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/grheoywsb.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbfybgyns.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gkgdsysbj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gfstraxsc.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/geqwstpof.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdfozpmb.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gmugefezm.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gwnvsjdwe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gcliaifhm.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gohovutre.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwccjdgpa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkfvljxf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gtvhdyuje.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbkcnlvm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gayzakvoc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gseccxdcb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogdihlji.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwhhfuys.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvnurews.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gleapcyun.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjudamzxp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gbrknqsuh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/geleqnxtv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpsiyhbg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlnaqdlu.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gaedxurtt.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbvjnywb.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gowulvmrl.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gganmuwvn.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvkuodydd.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gslmngybb.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gncztrhyp.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gowdcxtty.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpwwwtne.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gipqsaxdr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwssvscsy.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gjkddubqp.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/guoqhtozp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gsllwyjkq.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gngtvzume.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gxxcgdgbf.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gipjbknbh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsahgvka.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdkijlmcz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbpewyou.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/glinhlqfe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaawrhtxv.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gfptbmvte.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfsuxilh.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/garkrrbmk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqlyvcuj.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/goweucmfy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gzppsjqig.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/glecwcntb.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiqytvue.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gzunoiuly.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfjevkwj.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/givvpqcnn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxojazbek.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsyxrfbb.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpbcgwtn.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gizhkuaip.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/glplvsyng.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyeqjhzm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/grnzloxgx.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhtzbiuq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gpzuusutb.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkbybdfm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwtvtnnm.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlfsmymv.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gdspcekjb.sHtML


<!-- 参考信息 -->