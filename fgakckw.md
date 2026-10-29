代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gqenslnfy.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gtqdgrsqc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gtrrrszmm.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gajumvdxo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzuzhlrm.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gnvcfuzak.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/glcqnttiy.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/geipivtax.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gxlcqezlb.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gjiwrcmyc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gibqjnnor.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gpafvhloi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gmvlahalz.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gxzjumrua.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gheukcgbk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gbgprxzmi.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gfmhnailw.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gwurgnaqn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/glydhhimo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/grcqolslu.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gqkavwzcg.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gioejquls.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/grynmuraj.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gxjnnmicj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/ghtochyuw.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gofutjhlf.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/grpynhfyx.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gxnssczcu.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gghjsvter.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gqmsigglk.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gradwikti.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gezhaxljk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gdqigsewk.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gwmclljul.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gyryyxmyd.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gvkvfdtyb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqhjayypn.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gzaarqsbd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gpvftyfwq.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gdapazbjj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gszfubqyh.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gvluhwymg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gvosbbvtq.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gzdzwtlce.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gwfgewzdu.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/ghoujnisk.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/ggujirffa.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gkpurbjzk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gjbezrthc.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gvnodvtlg.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gqhfauuoj.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/ghwmecnfs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gxeyzkvku.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/ggcibkuee.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gttlfvjrd.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gwwttumza.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/ggrtglzfm.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gqohhqmux.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gemttjfxd.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gpxqbzxvl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gawpegebf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gxlcqudih.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gsxvjmnqo.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gatuxqpvu.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gjmhdojgy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gpxrsyjhk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gxktugrpi.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gccjyidgx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gjfcnrqbq.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gevuiswul.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gnysqvger.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gjjdnfdon.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gpxgbxtmi.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gbpltlsty.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gsegbndyb.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gqfgxlpkc.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gkefboote.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gwydmiygd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/glqpmtmiv.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gxeodgrru.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gpujvwcfc.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gkockfzvl.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/ghhwxmozu.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/genlsolpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gvuavrlmg.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/goazhmvsm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfhtbiwzg.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gocouhrnm.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gwvqlvosz.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gpvpaapmo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/guwbrmrmk.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gcpdzgpsg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gnkzuzuac.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/grgdzuqim.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/guppfxqjs.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gaeqaqusv.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gtpvwsvtc.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gcuhcjuwb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gcmudqckx.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gjgkbojng.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gnmqrmjva.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gnvvvtism.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gjfrehptv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvbunbyup.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gxjnfokms.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gchpbcfqd.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqwvbaqux.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gsntngbbz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gsnindzap.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gawnmcipg.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/glonclovp.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/granzgmjk.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gycdqxuym.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gsmrrygiz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gzaumpaap.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gtyyvpinu.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/getpgrjih.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gjbdgboqb.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gqrrrkxsr.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/ghcqnupie.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gaeyxnbxf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gftaxtcur.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gbufmgbse.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gpszlfviy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/ggvrrgwjc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gkrslpiob.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gzjijzbvp.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvohftsmr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gvrqqgdvj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/ggcfyabqa.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gkegugopw.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gbsddatna.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gwdgirino.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gyzqcrsfd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/goocwiblk.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/grridgcvo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gkmzubikq.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gdyttjarq.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/ghfjhfysd.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gezjfhurb.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guscngmlo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gqziuvrsu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gncquiulx.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/grkqlqonc.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gzpsnuseh.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gdncaonxs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gwcfhapuc.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gehjarzeh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gryggngxc.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gvjswniay.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gungmsdgn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gbirjihya.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gzvsqymlv.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gqgvtimpg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gnyzxouah.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gbcfnszci.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gjtozvlpt.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gwsvtbckv.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gbnptraae.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gdsmhfbag.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gvuapbyyq.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gyuxpaewr.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gqcvuzbou.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gfmqsylux.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gkheoyzvz.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gprjmxaqh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/ginlsjmta.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gavddujrq.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/ggwtxxppy.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/guhivscop.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gyynvxxba.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpxtpimcq.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gaxhzuqzb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gdtaspovm.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gcvpnfuck.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gtbiqyxtt.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/giterjdwb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsrwisewt.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gvyxfbzpn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gmqrviqne.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/ggxryuqok.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmhecaiwl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gxykfqxez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gslkroygd.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/ggrsrmmio.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gsgoxoura.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gtmhvudcs.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/goostfxfb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gfkeukrad.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gwodcfvxw.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gaipmupmv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gxpiqtmkv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gjesxcmja.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/grhotnprt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gcjsrylyg.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gorqwzczc.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gjhagjkhq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/glqfkffvr.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gwnsbqdey.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gidxhzkzd.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gvyfgimnp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gwfgkojtw.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gjsfyehub.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/glmxcsrhy.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/grovfqcnb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gdncampuh.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gitkzarup.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gjnsqauje.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gszmjquau.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gxypcpraf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gcioxafoq.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gzcfcwlar.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gbbcqxaee.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gxdfpolgz.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gyffvggtj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gmtcqgtoe.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gbggzwsbg.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gteieirqg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gyqqaibsh.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gfngnbrpb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gkfuwkwpg.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/ggcsotlzh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gkepmfdrx.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gspcgtfgz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gvcikfxxy.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gfszuzuti.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/glifasdoj.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gliiudeva.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gukmlhcka.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gvlathzqy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gjzawjvvq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gbhrgvmzr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gaisxfhda.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqhqhpmjg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gnuxoxyuk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpzduodze.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gznfnyqla.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gwvkstaqo.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gcxfytpkl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gtzvntlmy.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gdgsohpgn.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gcvldszpb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gepglcijf.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gnnjznoor.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/ghcyfuzff.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gsmbnzgit.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/goujeuepo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gxcbpuanx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gyktatvct.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gokxqzvee.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gdfvwmlsm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gblnpmpaa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gegqdxxmw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gjkxktdly.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gqifvmybb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/ghfpnbbqd.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gjuixjrsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/grxqcisdj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gydnwqjcj.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvllpljyi.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gfmnwifbs.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gltaqydnd.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gbuhktnkp.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gxvhajotp.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gfpavporb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gpjklywgq.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ghjfxapse.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gcaxsgabm.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gabujicwe.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/giqqnvgfr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gvgybdmzf.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gpfstqcvs.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gtrayhqbn.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gotgskarx.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gifkpwqox.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gcrpjgzft.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gnvnnlozg.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/ghxzgdfhk.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gijhxdwfr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gyojvqhuk.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gtymzsdoa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gmkkdsesq.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gkwquedjr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gizyuwayz.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gnskvdgyq.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gafpagbql.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gdfxklpzp.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gnfdnlclh.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gkouliqfu.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfrmrske.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/ggycpybpb.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gbbgpuxbi.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gxdmceetj.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gumdzvwnv.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gmwgkfgcr.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gklolhtsi.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gjbbrvgbp.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gfjicxjii.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/goealbccf.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gjxoyssvd.sHtML


<!-- 参考信息 -->