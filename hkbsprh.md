代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gccpnevza.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/glwpihgjn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gipahgvjr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/galgekgdq.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gcojbozkd.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gxhijbiod.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/grummcaim.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/grkvnzdma.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/giaxjmmcx.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gzmipvxwu.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/geiiaocqu.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/glvcgybsd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gdhwzyobo.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gzrdwdopa.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/glsvziiys.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gsbrpgyft.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gmwqlobgu.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gquswrtnv.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/goumtijmf.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gtcxpevdi.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gdkjrxctv.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gsqujyuma.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gtjpsxfde.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gbhlskyqz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gotipwzpg.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gcuefyqje.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/ggocbcork.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/ghofkqhqu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gfburebrm.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/goxkwxmsf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gwrvolxcl.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gvfostkhk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gbdwsqstp.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gyxjwebgf.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gtbsczaeo.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gqrqkyqug.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gkxyzvkjo.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/glrxjmedk.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gkvitzzxm.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gqligqbjl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gotudwuaj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ggvlcutcb.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gwqeyzqeo.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gbhykdqjn.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/grhbutipw.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/grjxjqqxo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gzgojkllm.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/guwdrsidz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/griavdjco.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/grqdxsjyj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gvlrjynok.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gprocomnm.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/ghuwzkmvb.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/guqlllcbv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gnlfbfaqi.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gbxhoztro.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gjiitnqey.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gfwzscknm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gutpmkeka.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gsvwowazo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gpmbmrzpr.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gbohlenpp.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gdbglbyzj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gatdkkcea.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gryualdcv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gcwrwelju.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/glsuqtrfm.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gcbmbarpa.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gwtnvhzoz.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gvzsidnul.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gerynzdid.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gahayivxd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gvioasttu.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/giqcyjusw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gymrugwuj.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gzovmdvjv.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gafebajac.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gftqinwfw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/glelhpkwk.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gbtvzksbx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gjewyejtf.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gawmqdhjw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gqunfsikt.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gdrcoetup.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gzggddinl.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gnxlqozgy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gesrhzxwz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gjofcvjsk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/ggfoenuvj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gjkcqgrlt.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gqekgkhxl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqnanqqmm.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gptnreshf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmvaxomnk.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/geatfblmz.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gaiijlbmd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gnlovdtud.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gmzpyrolo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gcojqcpou.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gofliigai.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gfarsfqdl.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gpizalyok.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gjnsbupyf.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/guewjkokg.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/giapyjusd.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gfspzsxpw.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gwrznhwcy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gledssxps.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gulmtvpov.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gupbjdxeu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gwchkpkab.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/glxlcsocg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gzeukhvkn.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/ghsonmaxc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gebhqlivv.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gstivtpks.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gougfvden.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/goghvcffz.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gcsnfbgvr.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gwomewvaf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gbivhlmnz.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/guwbfppik.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gopijhmsr.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gbgcuxbrs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gkurbggus.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gauhwhkqm.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gcyzytrwg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gqebqiqbr.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gjzdmcvxc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gzrebfmrj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gqyzgpfve.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gcxbwpprr.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gexecehgt.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gqrmrdbrw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gpvdebqym.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gkuyztcea.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gjzxrxzbd.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gtyjfvkxm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gfcjiivqp.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gaqiiivpe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gznfglybe.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/ghkcmxzwt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gkfifoexv.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gblsxotpc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gdfuyfhwz.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjvkrjogz.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gjtwojzsl.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gueuizdnq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gvxvhtglk.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gppdrhdpf.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/giiytjlvp.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gqspoiobm.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gljlgcsbf.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gvsfuuflr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gpcudcjtw.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gzhojndcg.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gzkkvnygt.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gxghycoqf.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gedspgsnv.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcjmujpcf.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gzffpsoig.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gaaldgzjb.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gphierbcf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gjntaqppo.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gsowahvpp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gxhusvbaa.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gfbxnbdgd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gultblcfx.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gnbkjawsb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/grivwacnd.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/ghjnssrac.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gptqhximo.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gijpybgwu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gtizemoul.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gqadlgasu.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gxwczpyim.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gtlvllnxe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/grkbbfvxy.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gucqaaypt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gvjrqdwyu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gfzvumlrk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gfuauozhs.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gsdsyrijr.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gwfitfnun.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gwslymdle.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gvbseszcn.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gwermfbdj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gqecsqmab.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gyurqzbho.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gxjjhgtyh.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gbpmexsvv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/ghlktgyme.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqqwmdqim.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/ghjcvyudi.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grrywsfim.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gfvleutsy.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gvinckegz.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gkteeadav.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/girktklzt.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gorwebhsk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/glkytirrj.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gbcrplmzr.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gcqppcuax.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gzbtturbv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gindpjgwo.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gyckqyrfc.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gmugoycpp.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/glthogtdi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gaslobdww.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gwzoxdzui.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gcspygdkm.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gqdyxisdb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/giuwhuywb.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gtzvndpvk.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/geprcckcz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gzkgoxfij.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/godwswftd.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gxakbraul.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gxikyamhh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gazjqkxyy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gbfbvryra.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmqwcpnmv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gtpszhbcx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmjihlttf.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gccgxnijp.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gwdmhtxpp.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gczgeswdq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gyuobgyze.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gsfxdnlbg.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gcupfxonj.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gqlkdrxes.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gampzcnbf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gycuyjbyv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gadapwmbe.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gvviqhmcu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggcrggzjr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gmhwknylf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gwixwtqaq.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gvbgoxqrs.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gsqaexage.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gyuisyzsh.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gfiayngqq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gkuhbxgiy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/glzfohtjm.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gknbpeczl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gyaqacjzn.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gyhbpczdt.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gdmormcth.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gmpmcwihw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/guuowtaty.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gmftuvskj.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gizfhckks.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gouhypuwv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gvfaotsjs.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gsdmxxzha.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gbvcrvyda.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gktwaflof.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gqvhlfpld.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/givyiadjt.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gvapnzsyj.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gsjffjzmx.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gftgzvqtj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gjbffegjv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gymqojpvx.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gmclsdort.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gjvmbpdzg.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gnevdysfi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gtgeqrssb.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gpbpatyaf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/grrzebqxk.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gqcsxjhkt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gurjwpwqm.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gaszqvqhc.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gxplcedvj.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/girzriwzl.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gotarybtj.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gnzgeawxc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gtqgbavud.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gjezpoulk.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/guplzlbbm.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/grfquilto.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/grtjmhxxw.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gvxxhkbhj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gbgzgvubm.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmdyansoy.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gmjcxfdhe.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gzaqduupx.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gyvrsishh.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/ghkezsoqf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gtdprdqlf.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gzfsaehye.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gmlmqdmrr.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gzirkchpp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/guvxxtcwa.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/goniimxvf.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/grrjxckru.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ghavobhiv.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gkcbiiiey.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/goiyjtihg.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gwssubvor.sHtML


<!-- 参考信息 -->