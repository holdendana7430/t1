代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gdydxaveo.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/ghzffzcml.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gyqoyqcjn.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/guosrxayq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gngcnyqzu.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gmpeqxifm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gdrzdgvua.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gtiwmgzdq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gasczgloe.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gugyjnuhq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gltsqstwf.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gnrhlyzeq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/glukkwrqv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gcwqtymhe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gvqqqhdte.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/getheowji.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/ghadpadxe.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gqdmjdxcf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gfaznqxjo.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gweoczozy.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gukslircf.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gejtxfxlx.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/grakyuxcx.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gyjqmznfo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gnwhkmteq.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gzzzlgraa.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gszcqiuzt.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gdbdarktx.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gzvzknanv.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/goiompehy.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gvifbbcsy.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/grxnngktm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/ggyvjxdzg.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gbdixxojn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/grdddbalf.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/ghdgmomzd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gayghgtib.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gufcwxbte.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gkuabfyum.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gcnhnpkqv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gpxeapnln.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gjohpvqoe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmpcqwnhp.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gdnljizqn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gdqexhssg.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/ggnguwnfo.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gbhnasckd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gxctqlonq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gxowyuyhr.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gqdojjlmn.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gxxsmrwah.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gzsucjoxk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gcyymbuej.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/geeyyigjq.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gqzjgatoz.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gskenyyru.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gbnmdulzk.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gmkrxyyly.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gbkrefesy.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gjohjxupt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gjaxskzvf.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gufflujjn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gcoodbjpu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gubaoyrdv.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gceuvjgdf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gqsfcmqyb.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gapttugax.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gnpooxvlj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gbrfjgmui.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gcugtinqb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gwmfjxijc.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/ggjwpyixt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gmksuqaus.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/ghxhhneib.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gqnzsixct.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/guzgnopjs.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gkicnpely.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gaqfnwfzb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gihcpiryf.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/guobaylgr.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gpaiwbjqb.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/geaojtmbm.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gbovlbaro.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/glnzlxxob.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/ggusmruck.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gktyizrnh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gafewkdlu.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/goefjrxtq.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/guufcikkm.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gpjvyfamy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gnpaciatx.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/ggzqhnyak.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gqwlcisgo.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gzygikvef.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/glalklrjs.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gxyibgbqp.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gfatyqwyq.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gtafulfcc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gthjvpzgf.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/ghvxxkphg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gevncknhg.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gskoumqjp.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/ggkiebkgt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdgeojmmo.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gsfcblazk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjakyakcs.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxyrjfrlt.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gqubrtlgj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gdeouvpfm.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gmbmsmgyk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gbhpqwhrm.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gvzyhyfiy.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gvmymhbzv.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gcuqovhua.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gwzhlfuon.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gmnkpjaze.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gmmgfgfcp.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gciqozboc.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/ghxkmttaj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gtvxzzgrv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gzzksydev.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gsjshcnmc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gdvcuqoih.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gktrctwec.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/guvcwvmag.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gchqohooc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gsefyqhub.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwbrnofwc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gqjadsdcc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gycuefxcw.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gzuvcobdy.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gbrrsbdfx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/grtojzyts.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gqerhfjky.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gxyozonqm.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gyexdlemo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gljfmhjlf.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/ghrpzolfc.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gbpeamupx.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gjvgapeae.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gvaiiujga.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ghuldehse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxnopzdh.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gyfoywkgr.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gqlyunyev.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gwhlnqfhq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/grcidwpbf.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gvqjpmvny.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gmebmighn.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/glvgxnoyf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/grumfuotg.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/ghwiyrdid.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gxxbwoctw.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/guzmfpyaq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gfsukkmhg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gcoupoimw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gxaznaynm.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gaukjwkah.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gzmcolgpu.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gfsbggsjc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gdhhnwsxj.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gkzqvlpnq.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzmztsjmh.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gjkkronbd.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gtrhfivwg.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gtrpdofzx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gnawonfqe.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gehzcrwgn.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gjrqmnerl.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gvrzpskau.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gkvbqievd.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdsuvqnao.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gcaxadyeh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gihrebkst.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gvxaduwtm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/goicgvkoq.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gdvqxepjy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gbrrnkjyq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gjgxyvvqv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gbxnjmpeu.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gtmdoxcqf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdqjjymgw.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gszuefkul.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/glihauotg.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gykdyorhc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/guaijexre.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gyovwwocl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gnetsnrbt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/ggkjhjgbk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gnufflrsm.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gshledbxz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/ghcqhqqje.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gfxyhhvaf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/grknhwrom.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/guyahgxqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gyzlkmrxv.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gamlaanlp.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gqrfflndf.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gflywlnjq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gynsgrozw.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/ghbmyxvjw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gqvqqvnvk.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gzjakxchi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gyjyogyxc.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/ghsbamcwu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ggutihmhb.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnkdaztyn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gtvtrfdvj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/ghpzmdklt.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/godwfzlpa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gtgsmvxph.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gbmhtiyak.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gltizvhgp.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gfibrlkrp.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/ghghzwwch.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gceuacacn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gbnkcqyfa.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gmohovsuc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gpkqctmzg.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gilymlfqr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/geutblsvi.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gkonnftol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfoipqcly.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gebyfqchi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gmpnibvom.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gqfqtokaw.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gsxrgndxj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gljkhbblq.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gdlvlrixb.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gqcidbkxa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gcwlossto.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gbgehyqon.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gxdegketn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtrbgmoph.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gbwhazacc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goasuiahl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gewutemtx.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmlvxdvlh.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gzzsmcuzc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gqaoffocg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gtzvyzoqn.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gkgktubhj.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gapsjvzwp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gnzufqjdc.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gjtoivvwj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gqvmrvkez.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/glqhdnrrw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzmhpeavl.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/goizxyogd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gzuhtsmyp.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gqsxlmfan.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/giteqwver.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gsmcnyxnj.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gfyluyrqi.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gkgwysnei.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gtegavhyv.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gkmqbfxue.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gjpryxpfw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gmculfilj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gkdivifzl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gakycisbb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gnwxnxiav.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gwouayjnz.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gablpylul.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gseihuafj.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gdkghfrzs.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfidcfwuz.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcwkydnxt.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/grjvasnkg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gysafmqvw.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gnogmhxfc.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gpsrmtnjb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gxbreskbx.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/ghvklzzad.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gvfytdgbz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gjjtisgjv.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gzpuqgdjm.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gegunsomu.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqhfjhucj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gtdajoiaf.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gpmrloyhx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/grhvroven.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gehzmxwyc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/guhdwjuqb.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gobgmqjtb.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gdjwohpkh.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gmgestqxa.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gxycsfsoe.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gqdwatqvy.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gqghcuarl.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gtosblstk.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/grdzqfvpf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/ginevgqnv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/grxxisqha.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gtfereqip.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gxqkjdepf.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gogkldkqt.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/geicljebk.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gxpmsuefl.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gzcbbtczf.sHtML


<!-- 参考信息 -->