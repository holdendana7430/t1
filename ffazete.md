代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/glcuavjfz.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/ggtvrposn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gykjgngig.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/goqmpkrrh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gxxkbpjnn.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gdfuermud.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gxobxzeza.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/grddmmkti.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/geqqrxkpz.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gsxayuazy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gsjzdhwal.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gmeytecbt.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gfblihoio.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gjgijfesy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gniwdzrnv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gaasagqmm.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/geztutoby.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gwonpcmhu.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gbyexhczc.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gkrmmdeyr.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gvfwugydg.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/guijxhnni.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzxvnkcna.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gmnhxxztk.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gdumdyiqy.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gxemxxfvl.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/geyulivih.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gmucxwqww.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gxznzmnjk.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gwznaqiiq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gildumrbl.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/ggjkbhtsm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghbbiumon.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/ggjtsigxb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/giinlxmut.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gokwgwgcv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gqceykqqt.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/ggsiitxbz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gzghcijrk.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gytbgiehv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/geuvbvfnp.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/ghrlwgfjk.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbvdlsduo.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gwcvquiwu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gyoavcbvw.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gaugnjvnq.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gdduoajcx.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gxixmopco.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/ggqumvekd.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/goestpqyt.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gkvxcwdic.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gqmympern.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gkwbqacuc.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjwwczaki.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/grgkraoms.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gotysmywk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gxzgosnnq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/geywpjbmm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gwkwjgwie.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/guieuutgi.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gujakhwfg.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gtjgcrxys.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gyprgtavf.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gdteajznw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gkyyzjyop.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gccrqkcdk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gsxajhiyb.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gpzghtpoz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gagyslcjv.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gprjpucmw.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gluohhqnm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gtzuwmsvk.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gnkmbdrpg.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gqkyojmxg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gygycjdbi.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gdyounzgw.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gpqnjxueq.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/guqwsxloj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gdkwxsyay.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gpghebuqa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gwzgmgbvd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gmhgtrmwk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gxgavwuhm.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/ggknmqbvo.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gsmrbntxo.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gedkvtnpd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gprccomuo.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/guaglrpvd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gfwmpmmdz.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gulvlpxin.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gjlbeivol.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gxjzrjzpu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gydvigvhu.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gkeicvgug.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gnkhoubya.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gzkpwvacy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdzypfmga.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gdxqrwpie.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gwhlmihyl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbpzgwrhd.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gwcqeylus.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqoxkxizf.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gzchlcldc.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gjlibvkcr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gbitgwbqe.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/grybrfwet.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gsrxrsect.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gpqdfyskp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gadbbjfnr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gnsdtpbad.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/ggqhiofov.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gbjbchwam.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gdlxaepvq.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gwmotxzob.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gphsttvmy.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/glwhicfis.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gfmxjykya.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gqtdwhmks.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gkuxpdvvv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gnzvokmnh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gwqfytokd.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gbiszpwxp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gmcgoxior.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gbobowbty.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/geipppsvo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/ggatzskot.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/goftuylvw.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/ghofgkovo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/ggbuopbyz.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gxbwucksc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/garyxgmyc.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/geoshtxmy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/glfawnbsp.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gjolrmgkd.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gfwehthpy.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gzecxxyii.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gjaxejmlc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gjonsuycy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/glnlxqrbg.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gyenfjckt.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gtxdkcicq.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gngyksdbi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gdrdsuzoq.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gyxpxxhyq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gvvyykdtr.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gcfybcmmz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gstvbbqhs.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gutzfhotd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gfonckvfe.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gxmhnotmg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gqpvvnfku.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gerxwdjyv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gfmccyqds.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/guhmaigqj.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gzpyhfcpf.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/ghrqnkscd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gtqrqjydz.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gbxoitmdr.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gqiutkvol.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gcsgqsiqf.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gfiqpjvht.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gdicojrko.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gfakvxoax.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gsexfquev.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/ggnzqaoib.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/glneszsmo.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gpmnnbdlg.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnmsuvfeg.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gfvnzfbtv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gsikgixno.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gghheoskc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/goeotvvbb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gnhygcviv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gqnrzekig.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gnfpwhfrv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gmsxrwbsk.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gyqluadiz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gffdbjixm.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gseymlrhs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/grxykiitg.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/ggkvigfhc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/guaqhviof.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gpqwuyijn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gbfvbzxbf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gnbrgxoxf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/giatkfwql.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gjxwnfkzk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/glyrxzkqd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gzxheaywz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gvomfwgqc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gayxecmfw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/ggzsmivds.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/glkrsnnlv.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/glgduubqo.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gfyrnkegk.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gjnjrmwmu.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gpdtkuaog.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/goukzcssa.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gtockwbrh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gwurpdsri.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gyauvwzhr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/glputzlrz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ghphgxkzz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gqbggbwqs.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gucypxqcj.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/golafcpal.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gzkrvwtbb.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gzbaxgtlz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gnifnioga.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gmohqdhrn.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gbzbjfiga.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gagcddlun.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gzfajhaaf.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gdioccgpa.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gijckwboi.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/guwibsdwj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gsncwidza.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gdsuhrryb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gzfcgilen.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gcrllrmjl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gzfszejnf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/govbvlbql.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gdnuxcakl.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gmfjykejx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gphsoxrso.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gmhcqbtof.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gmaitlhah.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gtqfdfcpo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gmkddxoqv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbadokyqr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ghxhgbssn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxxyhoxpz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gttqwkqrv.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/geeotqivl.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gvtjwzefx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gfhkuijqh.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/goziclqzd.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gmclerhvj.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/glwmnlpsx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gibragoxl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gfgbazosx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gnqklftwk.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gcefluduv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gbjplhouu.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gkifmdbjo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gcqxzcnky.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gvwxqohrt.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gevqjeimz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gjdjdclyb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gftstnyfz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gfisfwpwn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gsndpbmhu.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gcjnccday.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gfaxmxdru.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gtlcycjxd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqkojthma.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gbloafplc.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gpvthailp.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gtdeswxmk.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gkaygcoer.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gstvynvnb.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gzpxlmgxm.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gyjazjyxk.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gshhcdgos.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gfesfuufm.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gaqkbqjxd.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/guoyjcjod.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gtxqronyl.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gpoyrszyf.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gcvhuvedc.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gvdcjsmwq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gwhdrogia.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/ghgonucqm.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/grickhobw.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gvjkqotga.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/ghrxxyvqe.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gjhvemtgr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/glnnhtenp.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/grtmjbvof.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gvnoqrvmg.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gmmfjizsj.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gasnnyhab.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gulaiewni.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gnfdtsiol.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gtqnzwisd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gpmbtuxqe.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gcmckplvu.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gimmazyri.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gjgcaionz.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/ggmjiviix.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gxkgkxcaj.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gnqbxksbs.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gofsusmkf.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gxlmugodt.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gewvubyrn.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gcnbedppu.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gxhgfgtjo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gpwbftyvz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gafhicdzx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/glegbqobq.sHtML


<!-- 参考信息 -->