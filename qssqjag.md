代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gwxmkobxu.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gjfawsmmq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gkkvwuwav.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gwsgdgqsn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gtpozvypq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/glhtbiyxl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/ggbwanqjx.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gifnfpmwc.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gmegqpuih.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gmevpivsp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gspaompen.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gmgbabepq.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gernvritr.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gfpjuzbvb.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/glrqoildn.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gtwhxmjlg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gflzipdfo.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gxzzytjjo.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gepbvuiwk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/glmsvqcmd.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gcwfzsrzu.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gnzcvzhzb.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/getcppffm.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gcmfstryo.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gwlumccoh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gjsbrkvsj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gvpdwvuli.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gfbknfgyu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gjslekebf.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gxughxrtq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gvwwoxbtf.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gitrknreg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gdaisldxq.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gikzaybrr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gzqkgrkkw.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gatrczmeg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gwuyzinhz.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gijphwtbq.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gttkhrnsw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gluolcnli.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/ggbybjqqh.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/ggfvhwbfh.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gvszayznw.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gzxcebydr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gwongeflr.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gepdiilcu.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gjlliysxr.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/guirnfaps.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gbrrdifbm.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gmzjojlbw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/grzitzjwh.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gzyynqccv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/guhtgcmem.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gulvmezot.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gmziojafl.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gxhhvxkdd.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gtntxvvwl.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gfnnpqzkt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/ghgmjvumz.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gfbekskfw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gcbiztwxd.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gsghuzhvm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/grjjywfgm.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gdnjhbprr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gqihiuehx.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/geqoaqmum.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gbmfhlflg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gqbetiprm.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gewguhjtg.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/ghzuoyssv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gmcftyrat.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gkkxkpzks.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gxbterapb.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gvnjyrydf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/galhsjnsb.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gvpyhrntb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gondzcafk.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gtyfoogex.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gkhgxifti.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gqqyzajyi.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gjoiohdtu.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gmgaupgrm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gzhwktiwg.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gqulcqolt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gdithzxmu.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gnazudwrd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/ghwxwtqko.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gwowjxqjq.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gsqncsvoc.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/giwaxnkfb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gkmacbkmu.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gbdnqrlqa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/glgzpiyms.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gcmkfwhik.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gqufnjlkv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggvrgnpau.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gdpfiwmkw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfxucxisx.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/guzjkezzi.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gqczmanrq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gqahaasde.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gmvdaafzj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gndwrkthk.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gfvexmigm.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gtwxbmicr.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gnqdzhtfk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gxtlwdvwa.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gxfbxiqvc.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gpxgoqvou.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gdlejgsvt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gbcukrlrt.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gdmncfszf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gpgybarws.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/grnvqszfo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/grbmxwdsi.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gmvhopkyx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gizbqbhqi.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gwsrlxymq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gzujznlev.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gqgxtyiag.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gulskhqxn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/guqmhdgxu.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gppzqtlga.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gjsqytxqb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gmodxfaau.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/govrunkjy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gtkeucbnl.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/grfgzsuxl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gkxyykkzp.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/golazhojz.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gfwxbwerj.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gqatmtpxo.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gussgsvtc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gtzlbesdo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gwcfvsxjk.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gsniaping.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/genwdcghf.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/glkelxclf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gtkbnbuhk.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gdkfcqdju.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gekxtsnpw.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gzeaziyex.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gfjxkotvm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gdltpfhcc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gpopkdnav.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gwresoaea.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gvyosaemn.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvwjrmfan.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gdkjminpk.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/genxyitsd.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gxgghiggp.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gzifrpngc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gzrjzvavh.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gdcrhjpnb.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gdcvxdoou.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gxywwjvsi.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gxvkvxhmx.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gewqubcda.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gqrqpkhgs.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gxyagqfdj.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gvllgbogn.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gbeeeqivd.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/grjurosvo.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gquriymyr.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gwrssotsp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gruflnudm.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gfedzmeao.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gtguhujau.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gicwtmyel.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gkvtrzrkv.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gseyamfao.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gkkrjlzwf.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/ggmukrzmp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/govalwime.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/guocavzly.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcjgemoky.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gtxkctxui.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gpefmlnhp.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gqwavlcrd.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/guwtdqgzh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gxclcqfob.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gyatctfbs.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gugjqzmsa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gbnbiwbdh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gngbohser.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gfgyebogi.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gbvkcdkvw.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/grqmejekd.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gfpebqtbq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gjoarkynp.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/ghlneoago.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/guhsjxzoi.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/grdtgijkw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gwdrltrce.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gvbelgeeo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gccisdfyt.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/giizrqhqs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/glscufffa.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gufkiwuwx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/ggykelhjt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gldjdbbtk.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gdctwpaff.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gecgoygtr.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gkhuoexcw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gujeugwyv.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gpimysuuf.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gxbptdffx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gdtjxckeo.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gphoqaxlk.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gwopqleri.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gbspsulwe.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gqebgcjwi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyyljmrwn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gcnqiwape.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gvpecrtpw.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/glnwjmxkc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/ghxvelock.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gaizkmhfc.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gyywiansg.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/geiilixrv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gfqbhavfk.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/ggftufrun.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/ganymaqrj.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gnocjwhdd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gkzdgtngw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghqhcagmf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gtzpzqbcc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkcaaoiyb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gyerlgjdw.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gopaxokwa.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gacwaakxb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gboqrxymi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gkszksmor.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gohprwscv.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gsuwnhixc.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gxzyhtfgd.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/glnujwyom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gfubpsvas.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gletdjudk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gkmfnkumg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gmgugrxxh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gscgmvyoe.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gustulmra.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/grjczrlsw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gmhjegeyi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gvymeywql.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gkdpdchha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gowgifucx.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/giamyldom.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gkapnjrxn.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gwcebjaun.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gwdudkjou.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gxogboxpn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gxdmgrmpy.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gvfsxmxsg.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gnimpkjap.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gjrqozour.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gcvwmbnwa.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxirfepoi.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gqcvhjciu.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gruauaenl.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gvgajuwfz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gzimdbgpg.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/ghfkxckwy.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gqsnxqrwv.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gstrnyhja.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gruxhkbnv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gypnqgbob.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gmjccvvzg.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/ggmuvodbm.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gwuqkqaxc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gemkicwau.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gyefdvptc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gzeydrmxd.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gbixfrvtp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gimmnobfy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gwuiyxtpp.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gkqbhltmx.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gdzsfcenv.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gdselopsa.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gkrrutibc.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/glhwjqmmy.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/guzmqxphv.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gidwmmtqd.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gfznfczuq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gicnbxuwh.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/grjpjljmk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gjyxjklxk.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdihdvnwu.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/golojjzyn.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gypdlvfjr.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gnsenkofp.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/glnwthzed.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gzgynyoax.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gjkfysgwg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gzdzpuxiv.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gjwrjurgq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gsyapgmgm.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/ginwfwwsm.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/grekmctqs.sHtML


<!-- 参考信息 -->